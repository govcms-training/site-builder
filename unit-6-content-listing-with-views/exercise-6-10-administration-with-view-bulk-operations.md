# Exercise 6.10: Administration with View bulk operations

In this exercise, we'll create a way for content approvers to view all content waiting for approval, so they can quickly and easily review and publish new content.


## Prepare the site

In the current setup, content editors can create and publish job postings. We’re going to change this, so that new job postings must be reviewed by a Content Approver before being published. To do this, we’ll introduce a moderation workflow.

1. Go to _Configuration_ → _Workflow_ → **Workflows**.

    ![Image of Workflows](../.gitbook/assets/Ex-6-10-Workflows-1.png)
    
2. Edit the existing “Editorial” workflow. We’re going to reuse the existing workflow states and transitions as-is, to match the moderation workflow of the rest of the site.
3. Scroll down to **This workflow applies to** section and press **Select** in the **Content types** row.

    ![Image of This workflow applies to](../.gitbook/assets/Ex-6-10-Workflows-2.png)
    
4. Select the **Job Posting** checkbox, **Save** the changes.

    ![Image of Select Job Posting](../.gitbook/assets/Ex-6-10-Workflows-3.png)
    
5. Press the **Save** button in the Edit Editorial workflow page. 

## Add the view

1. Create a new View with the following settings:

    | View name | Admin: Submitted job postings |
    | :--- | :--- |
    | Show | Content of type: Job Posting |
    | Page title | Submitted jobs |
    | Page path | admin/submitted-jobs |
    | Display format | Table |
    | Items to display | 50 |
    | Use a pager | Selected |
    | Create a menu link | No |
    | Create a block | No |
    
    > **Hint**: Go to _Structure_ → _Views_ → **Add View**.
    
    ![Image of Add view](../.gitbook/assets/Ex-6-10-Workflows-4.png)

2. Click **Save and edit**.

## Add fields

> **Tip:** Select multiple fields at a time and configure them sequentially.

1. Add these fields:
   - Content: **Node operations bulk form**
   - Content: **Authored on**
   - Content: **State**

2. Configure the **Bulk operations**: Available actions:
   - Delete content
   - Save content
   - Update URL alias

    ![Image of Add fields](../.gitbook/assets/Ex-6-10-Workflows-5.png)
    
    ![Image of Configure Bulk operations field](../.gitbook/assets/Ex-6-10-Workflows-6.png)

Note that we did not select the “Publish content” and “Unpublish content”. Since we have a moderation workflow in place, these actions won’t work on our site.

![Image of View](../.gitbook/assets/Ex-6-10-Workflows-7.png)

Keep other defaults for the remaining fields. Remember to **Save** your changes to the View.

## Rearrange fields

Click the dropdown next to the **Add** button in the _Fields pane_ and select **Rearrange**.

![Image of Rearrange fields](../.gitbook/assets/Ex-6-10-Workflows-8.png)

![Image of Rearrange fields](../.gitbook/assets/Ex-6-10-Workflows-9.png)

## Remove unnecessary filters

The filter **Content: Published (= Yes)** can be removed as we will be replacing it in the next section.

![Image of Remove unnecessary filters](../.gitbook/assets/Ex-6-10-Workflows-10.png)

![Image of Remove unnecessary filters](../.gitbook/assets/Ex-6-10-Workflows-11.png)

## Add moderation workflow filter

To only see Job Postings that are pending approval, add the **Content: Moderation state** filter. Configure the following options:

![Image of Add moderation workflow filter](../.gitbook/assets/Ex-6-10-Workflows-13.png)

> **Tip:** Hold down the Command key \(Control for Windows\) to select multiple options.

## Configure the format settings

![Image of Configure the format settings](../.gitbook/assets/Ex-6-10-Workflows-14.png)

Edit the table settings. Ensure any column that can be sortable is selected. Set the default order for _Authored on_ to Descending.

![Image of Edit sortable settings](../.gitbook/assets/Ex-6-10-Workflows-15.png)

## Add a "no results" message

Adding a “no results” message will clearly show that the view IS working properly if/when there isn’t any content waiting for approval.

1. In the middle column, under **NO RESULTS BEHAVIOR**, click **Add**.
2. Select Global: Text area

    ![Image of Add text area](../.gitbook/assets/Ex-6-10-Workflows-16.png)

3. Then set the message “There are no job postings currently waiting for review!”.

    ![Image of No results message](../.gitbook/assets/Ex-6-10-Workflows-17.png)
    
4. **Apply** the changes.

## Change access settings for this view

Lastly, we will change the access/permission settings for this new view, from **View published content** to **Administer content**.

![Image of View - Access](../.gitbook/assets/Ex-6-10-Workflows-18.png)

![Image of Change access settings](../.gitbook/assets/Ex-6-10-Workflows-19.png)

## Save and review

Save the view and review. Go to admin/submitted-jobs. If there are no Job Listings in Draft status you should see the screen below:

![Image of No jobs waiting for review](../.gitbook/assets/Ex-6-10-Workflows-20.png)

