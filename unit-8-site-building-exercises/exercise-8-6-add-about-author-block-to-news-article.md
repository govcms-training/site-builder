# Exercise 8.6: Add About author block to News article

In this exercise we’ll create an author block.

![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2Fgovcms-site-builder%2F-LzEeysPiuilE7VSaStD%2F-LzEfAJUmyaoiKMb8l4\_%2F115.png?generation=1579737221013347\&alt=media)

#### **Exercise 8.6:** Create the author block

## Prepare the site

To maximise this exercise, make sure user accounts have profile images. Out-of-the-box, GovCMS does not have a profile image available. Let’s add it.

1. Navigate to **Configuration** → **People** → **Account settings** → **Manage fields**. You’ll notice that this interface is exactly the same as for _content types_.
2.  Add an Image field, using your previous experience adding fields. Make the Image field match the following criteria:

    <img src="../.gitbook/assets/116 (1).png" alt="Image of blank profile image" data-size="original">

* **Field type**: Reference > Image
* **Label**: Profile Image
* **Machine name**: field\_profile\_image
* File system type: Public files
* Upload a default generic profile image (you may Google for “user profile placeholder” and get an image you like) --------->
* Allowed number of values: 1
* Required field: yes
* **File directory**: profile\_photos
* Minimum image resolution: 150x150px
* Maximum upload size: 1MB

1. Configure Manage Display:
   1. Place the **Profile Image** above all fields
   2. Hide the field label
   3. Apply _Image style_: Medium

Add images to the profile of some website users. Alternatively use the _Generate users_ function (**Configuration** → **Development** → **Generate users**).

Next, change the authors of existing content so we have a variety of authors. Edit the “Authoring information” tab in the existing _News and Media_ and _Job postings_.

Alternatively use the _Generate content_ function (**Configuration** → **Development** → **Generate content**). Select News and Media, Job posting content types.

**Note:** If the _Generate content function_ was used, make sure you publish your _News_ and _media_ posts. Remember, they’re not published by default due to the _Moderation workflow_ in place.

![Image of Authoring information](../.gitbook/assets/117.png)

## Add a new View

1. Go to Structure → Views and click + Add new View
2. Use the following information to fill out the form:

* View name: About the author
* Show “Users” sorted by “Unsorted”
* Select “Create a block”
* Ensure display format is _Unformatted list_ or _Fields_.
*   Change items per page to 1. Use the defaults for everything else (ensure the settings are as shown in the image below)

    <img src="../.gitbook/assets/118 (1).png" alt="Image of Block settings" data-size="original">

1. Click Save and edit

This loads the full Views editing screen. This illustration correlates to the steps outlined below.

![Image of full Views editing screen](../.gitbook/assets/119.png)

## Add fields to the View

Notice the “Advanced” options available in Views.

1. In the left column, find and edit fields by clicking **Add**
2. Select User: Profile image
3. Apply the changes
4. On the next configuration popup screen, apply the _Image style_ **Medium (220x220)**.
5. Make the image linking to **Content**.
6. Apply your changes.
7. Rearrange the **User: Profile Image** field to stay above the **User: Name** field

## Make display dependent on author of content (contextual filter)

1. On the right-hand side, click **Advanced** to expand the settings.

* Next to Contextual filters click **Add**.

1. In the next screen, type “**ID**” into the search field.

* Select “User ID”.
* Click Add and configure filter.

1. In the next screen, select “Provide default value”. This opens extra options.

* Under type: Select “User ID from route context”
*   Select “Also look for a node and use the node author”

    <img src="../.gitbook/assets/120 (1).png" alt="Image of Provide default value" data-size="original">

1. Select _Specify validation criteria_ under “When the filter value IS available or a default is provided” and select **User ID** as **Validator**.
2. Click **Apply**. The window will close.

## Check the preview

When you check the preview you’ll notice nothing is displaying. To fix this:

1. Type 1 and click **Update preview**. This pulls in the profile of user/1.
2. Click **Save** at the top of the Views editing screen.
3. Place the block and test.

Now we can configure the block to display on News and Media articles. The News and Media content type is set up by default to use Panelizer view. The Panelizer view replaces the default GovCMS page layout and provides a way to build a “layout within layout”.

Check the _Manage Display_ page of the _News and media_ content type:

![Image of News and media Manage display](<../.gitbook/assets/121 (1).png>)

You’ll see that the page has multiple View modes activated. The Full content view mode overrides the page display for our content type. Let’s explore it.

![Image of Display configuration page](<../.gitbook/assets/122 (1).png>)

Notice that this display configuration page looks completely different to our Job posting content type. Instead of fields and display modes we see Displays here. By default, the Sidebar right display is used to render our News and Media content.

You may also notice that the Content Editors are allowed to select which display to use. This flexibility provides alternative display options for showing our News and Media articles, but introduces some extra complexity in configuring it.

## Review Panelizer content configuration

Let’s review how the Panelizer content is configured. We’ll practice placing the Content Author block in our News and Media articles.

1.  Click the **Edit** button in the Sidebar Right (2:1) row

    <img src="../.gitbook/assets/115 (1) (1) (1) (1) (1) (2) (1) (1) (1) (2).png" alt="Image of Edit Sidebar Right" data-size="original">
2.  Click the **Content** vertical tab on the left:

    <img src="../.gitbook/assets/124 (1).png" alt="Image of General Settings - Content" data-size="original">
3.  Explore the Content page. See how it has their own regions defined

    <img src="../.gitbook/assets/125 (1).png" alt="Image of Content page Regions" data-size="original">
4. Click the **Add new block** button at the top of the page
5.  Under the Lists (Views), locate the block we prepared earlier:

    <img src="../.gitbook/assets/126 (1).png" alt="Image of About the Author lists view" data-size="original">
6.  Select **Sidebar** region and **Add block**

    <img src="../.gitbook/assets/127 (1).png" alt="Image of Add block to Sidebar" data-size="original">
7.  Position the About the author block below other blocks within the Sidebar region

    <img src="../.gitbook/assets/128.png" alt="Image of Position block" data-size="original">
8. Click Update and Save

Test it by navigating to a published News and Media article. You may update the content of the page and the Authoring information, to check how the display changes.

Logout and test: Can anonymous users see the block?

At the moment, anonymous users can’t see the block. The final step is to set up permissions so anonymous users can see user profiles.

1. Go to People → Permissions
2. Scroll down to “View user information”
3.  Select to allow _Anonymous_ and _Authenticated users_ to View user information

    <img src="../.gitbook/assets/129.png" alt="Image of block Permissions" data-size="original">
4. Scroll down and click **Save permissions**

Now when you go back and check the site as an anonymous user you’ll see the author information.
