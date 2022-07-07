# Exercise 3.2: Add and configure a media field

In this exercise you will add an Image media field to a content type and learn how to configure it. There are four steps involved:

1. Create an image style
2. Configure an Image Media entity view mode to use an Image style
3. Check permissions
4. Add image field to content type

Image styles are set and configured in the _Image styles admin page_.

## Create an image style

1. Go to Configuration → Media → Image styles.
2. To create our new image style, click on the **Add image style** button at the top of the page. 

    ![Image of Add image style](../.gitbook/assets/60%20%281%29.png)

3. Name it **Job Posting Image** given the image style will be applied to the “Job posting” Featured Image field.
4. Click the **Create new style** button to save the new image style. You’ll then be taken to the “Edit style Job Posting Image” page. 

    ![Image of success notification](../.gitbook/assets/61.png)

5. The next step is to add the Scale effect. Under **Effects** select **Scale** from the dropdown menu. Click **Add**. You’ll then be taken to the “Add scale effect” page.
6. Enter the following settings:
  * **Width**: 1200
  * **Height**: leave empty This allows you to have a flexible image height and keep the original proportions of the image.
  * Leave the **Allow Upscaling** checkbox unselected Image upscaling usually leads to poor image quality.
  * Click Add effect. 

    ![Image of success notification](../.gitbook/assets/62%20%282%29.png)

7. Your _image style_ has been saved. You can make additional changes and then click the **Save** button to save those changes.

![Image of success notification](../.gitbook/assets/63%20%281%29.png)

## Configure an Image Media entity view mode to use an Image style

1. Navigate to the _Structure_ → _Media types_ → I_mage_ → _Manage display_ \(/admin/structure/media/manage/image/display\). You should see some out-of-the-box available view modes. 

    ![Image of Media types menu](../.gitbook/assets/64%20%282%29.png)
    
2. Scroll to the bottom of the page and expand the **Custom display settings** pane. You can see a few _View modes_ preselected by default. Each selected checkbox here represents an enabled _View mode_ at the top of the page.

    Since we need to apply our custom _Image style_, we have to create a new _View mode_ so that we don’t affect the display of existing images that are configured to display with other _View modes_.
    
    ![Image of create new view mode](../.gitbook/assets/65.png)

3. Open the **Manage view modes** link \(see the previous screenshot\) in a new tab/browser window. 

    ![Image of Manage view modes](../.gitbook/assets/66%20%281%29.png)
    
4. Locate the Media and click **Add new Media view mode** link.
5. Give it a name “Job Posting featured” and click the **Save** button.
6. Return to the previous browser tab/window - go back to step 2b above and refresh the page to get the updated list of _View modes_.
7. Repeat step 2b above by scrolling down and expanding the _Custom display settings_ pane. You should now see the Job Posting featured _view mode_ as a checkbox option. Select it and save the page.
8. Note, that the **Job Posting featured** tab is now available at the top. Click it to navigate to the view mode configuration page.

    ![Image of Job Posting featured link](../.gitbook/assets/67.png)
     
9. At the moment, the Image field is the only one available for display and it is set to show as the originally uploaded image, without any _image style_. We need to change it to apply our custom _Image style_. 

    ![Image of Open image link](../.gitbook/assets/68.png)

10. Click the gear link on the right to change from the Original image to the _image style_ **Job Posting Image.**. Press the **Update** button to save the changes.
   
   ![Image of apply new image style](../.gitbook/assets/69%20%281%29.png)

11. Confirm the image style option has changed: 

    ![Image of confirm new style](../.gitbook/assets/70%20%281%29.png)

12. Press the **Save** button to save the changes.

## Check permissions

1. Go to **People** → **Permissions** and double check the permissions for the content type: _Job posting_.
2. Make sure the _Content Author_ role has permissions to _Create_, _Edit_ any and _Delete_ any _Job posting_. 

    ![Image of check permissions for Job posting](../.gitbook/assets/71.png)
    
3. Click Save permissions


##Add image field to content type 

Go to Administration → Structure → Content types → Job Posting → Manage fields page. Add a field following these steps:

1. Click the **Add field** button.
2. In the “Reuse an existing field” selector, choose **Entity reference: field\_featured\_image**.

    ![Image of reuse existing field](../.gitbook/assets/72%20%281%29.png)

3. Ensure the label reads “Featured Image”.
4. Click the **Save and continue** button.
5. In the next page, select the “Create referenced entities if they don't already exist” checkbox in the Reference type fieldset.

    ![Image of Create referenced entities checkbox](../.gitbook/assets/73%20%282%29.png)

6. Select Image as **Media type**.
7. Leave the remaining values to their defaults and **Save settings**. This will take you back to the **Manage fields** page.
8. Navigate to the **Manage form display** \(secondary tabs\).
9. Locate the **Featured image** field, set the _Widget_ to **Entity Browser**
10. Change the Widget for the field as displayed below:

![Image of field Widget config](../.gitbook/assets/74.png)
