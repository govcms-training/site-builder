# Exercise 6.10: Administration with View bulk operations

In this exercise, we'll create a way for content approvers to view all content waiting for approval, so they can quickly and easily review and publish new content.

## Prepare the site

In the current setup, content editors can create and publish job postings. We’re going to change this, so that new job postings must be reviewed by a Content Approver before being published. To do this, we’ll introduce a moderation workflow.

1. Go to Configuration → Workflow → Workflows
2. Edit the existing “Editorial” workflow. We’re going to reuse the existing workflow states and transitions as-is, to match the moderation workflow of the rest of the site.
3.  Scroll down to **This workflow applies to** section and press **Select** in the **Content types** row.

    <img src="../.gitbook/assets/58.png" alt="Image of This workflow applies to" data-size="original">
4.  Select the **Job Posting** checkbox, **Save** the changes

    <img src="../.gitbook/assets/59 (2).png" alt="Image of Select Job Posting" data-size="original">
5. Press the **Save** button in the Edit Editorial workflow page.

## Add the view

1.  Create a new View with the following settings

    | View name          | Admin: Submitted job postings |
    | ------------------ | ----------------------------- |
    | Show               | Content of type: Job Posting  |
    | Page title         | Submitted jobs                |
    | Page path          | admin/content/jobs            |
    | Display format     | Table                         |
    | Items to display   | 50                            |
    | Use a pager        | Selected                      |
    | Create a menu link | No                            |
    | Create a block     | No                            |
2. Click Save and edit.

## Add fields

> **Tip:** Select multiple fields at a time and configure them sequentially.

1. Add these fields:

* Content: Node operations bulk form
* Content: Authored on
* Content: State

1. Configure the Bulk operations:

Available actions:

* Delete content
* Save content
* Update URL alias

Note that we did not select the “Publish content” and “Unpublish content”. Since we have a moderation workflow in place, these actions won’t work on our site.

Keep other defaults for the remaining fields.

## Rearrange fields

![Image of Rearrange fields](../.gitbook/assets/60.png)

## Remove unnecessary filters

![Image of Remove unnecessary filters](<../.gitbook/assets/61 (2).png>)

## Add moderation workflow filter

To only see Job Postings that are pending approval, add the **Content: Moderation state** filter. Configure the following options:

![Image of Add moderation workflow filter](<../.gitbook/assets/62 (1).png>)

## Configure the format settings

![Image of Configure the format settings](<../.gitbook/assets/63 (2).png>)

Edit the table settings. Ensure any column that can be sortable is selected.

![Image of Edit sortable settings](<../.gitbook/assets/64 (1).png>)

## Add a "no results" message

Adding a “no results” message will clearly show that the view IS working properly if/when there isn’t any content waiting for approval.

1. In the middle column, under **NO RESULTS BEHAVIOR**, click **Add**.
2. Select Global: Text area
3.  Then set the message “There are no job postings currently waiting for review!”.

    <img src="../.gitbook/assets/65 (2).png" alt="Image of No results message" data-size="original">
4. Apply the changes

## Change access settings for this view

Lastly, you want to change the access/permission settings for this new view, from "View published content" to "Administer content".

![Image of Change access settings](../.gitbook/assets/66.png)

**Save and review your changes**
