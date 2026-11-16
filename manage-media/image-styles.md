# Image styles

Drupal contains the **image style** feature, which allows you to upload an image once as a media asset, and then have that image **automatically resized** and adjusted depending on your needs.

This means the system can automatically adjust file sizes to decrease page size and load times.

{% hint style="info" icon="weight-hanging" %}
The average photo from a digital camera is over 6000 pixels wide and 15 megabytes, when the average news thumbnail only needs to be about 400 pixels wide and 0.020 megabytes.
{% endhint %}

### Why image styles are beneficial

Image styles let you resize images on-demand so they're optimised for each display use case on your website.

Multiple image styles are provided out-of-the-box. However, Site Administrators can define additional styles.

Having a robust array of image styles allows content editors to focus on sourcing the right image once, rather than having to get a designer to resize an image in multiple formats for banners and thumbnails.

Image styles allow you to present images across the website in a preconfigured way and avoid inconsistency between image sizes.

### Create an image style

Start by opening **Configuration**, **Media** and selecting **Image styles**.

<figure><img src="../.gitbook/assets/image (41).png" alt=""><figcaption></figcaption></figure>

This page lists all the existing image styles on your website. To create a new one select the blue **Add image style** button.

This image style will be for our speaker, so add a title and select **Create new style**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 4.11.13 pm.png" alt=""><figcaption></figcaption></figure>

The style page will show you an **example source image**, and a **derivative image** (what it will look like once this style has been applied to it). At the moment there are no styles being applied, so both images are the same.

Below that, under the **Effect** area, you can see all the effects we’re currently applying, which is none.

<figure><img src="../.gitbook/assets/image (42).png" alt=""><figcaption></figcaption></figure>

Using the **dropdown menu**, select **Focal Point Scale and Crop** and then select **Add**.

<figure><img src="../.gitbook/assets/image (43).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
The **focal point** effects are only available on websites with the **Focal Point module** enabled. This module allows you to set the focal point of an image so that if it's cropped by an image style, Drupal will try to keep the focal point in the middle of the image.
{% endhint %}

On the following screen, specify a target width and height, and then select **Add effect**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 4.24.48 pm.png" alt="" width="294"><figcaption></figcaption></figure>

The example derivative image is now showing as a resized image.

<figure><img src="../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" icon="images" %}
There are a number of effects that can transform your image. Feel free to play around with a selection.
{% endhint %}

Now that the new image style has been created, you need to implement it on your website.

This is where we will create a new **View mode** for image media entities.

### Focal point

The **Focal Point module** allows you to set the centre (focal point) of the image when it's resized or cropped in an image style.

Each image has its own focal point, which can be set by editing an image from the media library, selecting the focal point, and then saving.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 5.25.41 pm.png" alt=""><figcaption></figcaption></figure>

In the above example, if this image was cropped to be tall and thin, the person's arm would remain in the centre of the frame, and her face might be cut off.

By selecting a new focal point by clicking on the image and then saving, we can ensure that her face remains intact during any image style effects.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 5.27.05 pm.png" alt=""><figcaption></figcaption></figure>
