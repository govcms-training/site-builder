# Discussion

Thinking of our sample Government Jobs Portal, what content types do you think we’ll need? Do we need to change any of the existing GovCMS content types to suit our needs?

![](.gitbook/assets/30%20%281%29.png)

#### **Exercise 2.2:** A content type in minutes

In this exercise you’ll design your own content type for the Government Jobs Portal \(not a Job Posting content type\).

1. Use the blank area below to sketch the content entry form. Think about what fields you’ll need and what widgets you might need. Sketch how the content would be displayed on the listing page versus a full page.

Sketch how the content might be displayed in two different conditions.

Full page display \(**Full content** _view mode_\)

Listing display \(**Teaser** _view mode_\)

### 2.3 Create a content type

Different content types meet different content requirements while ensuring consistency across a type of content. Content types are set up with text boxes and structured through pull-down menus and check boxes.

https://www.drupal.org/docs/user\_guide/en/structure-content-type.html

#### **Exercise 2.3:** Create a content type

In this exercise you’ll create a Job Posting content type. The screenshot below shows the form and what the posting will look like on the website.

| Create job posting form | Individual job posting |
| :--- | :--- |
| ![](.gitbook/assets/31%20%282%29.png) | ![](.gitbook/assets/32.png) |

As the name suggests, the _Job Posting_ content type will be used to post jobs on the website. There are three stages involved:

1. Create content type
2. Review your content type
3. Adjust the permissions for your new content type
4. **Create a content type**
5. Go to Structure → Content types. Click **Add content type**
6. Next, type in the content name and description:

* **Name**: Job Posting
* **Description**: Post a job to the jobs section of the site. \(The description needs to explain the content type.\)

1. Next, scroll down to the configuration tabs. Under **Submission form settings** follow these:

* Title field label: _Job title_
* Preview before submitting: Disabled
* **Explanation or submission guidelines**: Leave this empty. This field lets you put in any specific instructions for the content type.

![](.gitbook/assets/33%20%281%29.png)

1. We want jobs to be published by default, but not automatically promoted to the front page, so under **Publishing options** use these settings:

* **Published**: Leave selected
* Promoted to front page: Deselect

**Note:** Some Content Authors \(depending on their permissions\) will be able to override these defaults when creating content.

1. We don’t want the author’s name or the content publish date displayed, so under **Display settings** deselect the _Display author and date information option_.
2. We also don’t want job listings being added to the menu navigation, so under the default **Menu settings**, deselect Main menu.
3. Click _**Save and manage fields**_. This brings you to the Manage Fields admin page - admin/structure/types/manage/job\_posting/fields. Review the default fields that were created for your new content type. ![](.gitbook/assets/34.png) 
4. **Review your content type**

Go to **Content** → **Add content** and select Job posting. Review the form for your new content type.

1. **Adjust permissions for your new content type**

Go to **People** → **Permissions** and change the permissions to match the other content types.

#### **Challenge exercise 2.4:** Plan a new content type

Looking back on what you’ve learnt so far during this unit, think about how you’d add a new content type, such as ‘Media conference’. What fields would you need to include? Plan out the process you’d follow to create the new content type.

