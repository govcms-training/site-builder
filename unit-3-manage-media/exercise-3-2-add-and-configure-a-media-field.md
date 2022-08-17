# Exercise 3.2: Add and configure a media field

In this exercise you will add an Image media field to a content type and learn how to configure it. There are four steps involved:

1. Create an image style
2. Configure an Image Media entity view mode to use an Image style
3. Check permissions
4. Add image field to content type

Image styles are set and configured in the _Image styles admin page_.

## 1. Create an image style

1. Go to _Configuration_ → _Media_ → **Image styles**.
2.  To create our new image style, click on the **Add image style** button at the top of the page.

    <img src="../.gitbook/assets/Ex-3-2-Image-Styles-1.png" alt="Image of Add image style" data-size="original">
3. Name it **Job Posting Image** (given the image style will be applied to the “Job posting” Featured Image field.)
4.  Click the **Create new style** button to save the new image style. You’ll then be taken to the **Edit style Job Posting Image** page as seen below.

    <img src="../.gitbook/assets/Ex-3-2-Image-Styles-2.png" alt="Image of success notification" data-size="original">
5. The next step is to add the Scale effect. Under **Effect** select **Scale** from the dropdown menu.
6. Click **Add**. You’ll then be taken to the **Add scale effect** page.
7.  Enter the following settings:

    * **Width**: 1200
    * **Height**: leave empty This allows you to have a flexible image height and keep the original proportions of the image.
    * Leave the **Allow Upscaling** checkbox unselected Image upscaling usually leads to poor image quality.
    * Click Add effect.

    <img src="../.gitbook/assets/Ex-3-2-Image-Styles-3.png" alt="Image of success notification" data-size="original">
8.  Your _image style_ has been saved. You can make additional changes and then click the **Save** button to save those changes.

    <img src="../.gitbook/assets/Ex-3-2-Image-Styles-4.png" alt="Image of success notification" data-size="original">

## 2. Configure an Image Media entity view mode to use an Image style

1.  Navigate to the _Structure_ → _Media types_ → _Image_ → _Manage display_ (/admin/structure/media/manage/image/display). You should see some out-of-the-box available view modes.

    <img src="../.gitbook/assets/Ex-3-2-Image-Styles-5.png" alt="Image of Media types menu" data-size="original">
2.  Scroll to the bottom of the page and expand the **Custom display settings** pane. You can see a few _View modes_ preselected by default. Each selected checkbox here represents an enabled _View mode_ at the top of the page.

    Since we need to apply our custom _Image style_, we have to create a new _View mode_ so that we don’t affect the display of existing images that are configured to display with other _View modes_.

    <img src="../.gitbook/assets/Ex-3-2-Image-Styles-6.png" alt="Image of Manage display / create new view mode" data-size="original">
3.  Click on the **Manage view modes** link (see the previous screenshot) in a new tab/browser window.

    <img src="../.gitbook/assets/Ex-3-2-Image-Styles-7.png" alt="Image of Manage view modes" data-size="original">
4. Click the **Add view mode** button.
5. Select **Media** from the list.
6. Give it a name “Job Posting featured” and click the **Save** button.
7. Return to the previous browser tab/window - go back to step 2b above and refresh the page to get the updated list of _View modes_.
8.  Repeat step 2b above by scrolling down and expanding the _Custom display settings_ pane. You should now see the Job Posting featured _view mode_ as a checkbox option. Select it and save the page.

    <img src="../.gitbook/assets/Ex-3-2-Image-Styles-8.png" alt="Image of Manage view modes" data-size="original">
9. Note, that the **Job Posting featured** tab is now available at the top. Click it to navigate to the view mode configuration page.
10. At the moment, the Image field is the only one available for display and it is set to show as the originally uploaded image, without any _image style_. We need to change it to apply our custom _Image style_.

    <img src="../.gitbook/assets/Ex-3-2-Image-Styles-9.png" alt="Image of Open image link" data-size="original">
11. Click the gear link on the right to change from the Original image to the _image style_ **Job Posting Image.**. Press the **Update** button to save the changes.

    <img src="../.gitbook/assets/Ex-3-2-Image-Styles-10.png" alt="Image of apply new image style" data-size="original">
12. Confirm the image style option has changed:

    <img src="../.gitbook/assets/Ex-3-2-Image-Styles-11.png" alt="Image of confirm new style" data-size="original">
13. Press the **Save** button to save the changes.

## 3. Check permissions

1. Go to **People** → **Permissions** and double check the permissions for the content type: _Job posting_.
2.  Make sure the _Content Author_ role has permissions to _Create_, _Edit_ any and _Delete_ any _Job posting_.

    <img src="../.gitbook/assets/71 (1).png" alt="Image of check permissions for Job posting" data-size="original">
3. Click Save permissions

## 4. Add image field to content type

Go to _Structure_ → _Content types_ → _Job Posting_ → **Manage fields** page. Add a field following these steps:

1. Click the **Add field** button.
2.  In the “Reuse an existing field” selector, choose **Entity reference: field\_featured\_image**.

    <img src="../.gitbook/assets/Ex-3-2-Image-Styles-12.png" alt="Image of reuse existing field" data-size="original">
3. Ensure the label reads “Featured Image”.
4. Click the **Save and continue** button.
5.  In the next page, select the **Create referenced entities if they don't already exist** toggle in the Reference type fieldset.

    <img src="../.gitbook/assets/Ex-3-2-Image-Styles-13.png" alt="Image of Create referenced entities checkbox" data-size="original">
6. Select Image as **Media type**.
7. Leave the remaining values to their defaults and **Save settings**. This will take you back to the **Manage fields** page.
8. Navigate to the **Manage form display** (secondary tabs).
9. Locate the **Featured image** field, set the _Widget_ to **Entity Browser**.
10. Click on the cogs icon to configure the Entity Browser.
11. Change the Widget for the field as displayed below, then click on **Update**.

    <img src="../.gitbook/assets/Ex-3-2-Image-Styles-14.png" alt="Image of field Widget config" data-size="original">
