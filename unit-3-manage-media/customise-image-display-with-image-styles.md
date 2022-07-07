# Customise image display with image styles

The Image module allows you to display and manipulate images on your website. It exposes a setting for using the Image toolkit, allows you to configure image styles that can be used for resizing or adjusting images on display, and provides an image field \(using the Field API\) for attaching images to content.

Image Styles is a feature of GovCMS that allows to resize and crop images within the predefined dimensions, ensuring the file size of the image does not increase page size unnecessarily.

Multiple image styles are provided out of the box and Site Builders can define additional image styles. Having image styles allows content editors focus on image uploading, where resizing is done automatically by GovCMS. In addition, Image styles allow to present images across the site in a preconfigured way and avoid inconsistency between image sizes.

By default, anyone who can add articles can upload images. However, to ensure a consistent layout, during _content analysis_ of our client we identified that all images in our content need to be within 480×480 pixels.

![](../.gitbook/assets/55%20%281%29.png)

The diagram above outlines how Media types are referenced by Content Types via the Media entity reference field. To apply an Image Style to an image field, we have to select a View mode of the Image media. The Image media display configuration has the Image style selection.

