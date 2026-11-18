# Media types

### Creating media types

While you can **technically** create new media types, this is often not required.

The pre-bundled media types in Drupal/GovCMS cover all the available file types, and any further refinement of type could **better be done in a content type**.

For example, if you want to upload an annual report, you could either:

* Create a new media type for annual reports
* Create a new content type for annual reports and **reference** the document media type as a field.

In the above example, if you made an annual report a media type, you'd need to add additional fields such as rich text fields and taxonomy terms. This effectively makes it a content type that's being managed via the media library UI.

So while it can be done, and in some edge cases might be the best method, the out-of-the-box media types cover the vast majority of use cases.

### Why customise a media type

While creating new media types may be overkill, you can **customise existing** media types to provide additional information in them, to help your content authors and website visitors.

You can do this by [adding fields](../designing-and-planning-content/add-and-configure-fields.md) and [managing the form](../designing-and-planning-content/manage-form-display.md) and [display modes](../designing-and-planning-content/manage-display-and-view-modes.md) just like content types and paragraphs.

By adding text fields to the image media type, you could allow content authors to upload additional information such as the photographer, the image’s copyright status or a caption.

Centralising this information inside the media asset allows you to easily re-use all the information anywhere on your website. The information is held centrally in the media asset, without having to manually re-add it each time.

### Customising a media type

{% hint style="info" %}
In this example we're going to add a text field to our image media type so that we can capture the photographer/image credit for the photo source.
{% endhint %}

Go to **Media types** by hovering over **Structure** and selecting **Media types**.

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

This page lists all your current media types. Rather than adding a new one, we'll use the dropdown on the right and select **Manage fields** against the **Image** media type.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 1.10.48 pm.png" alt=""><figcaption></figcaption></figure>

Here we can see the fields that are added to the image media entity.

We want to know who the photographer/source is, so that we can properly credit them every time the image is used across the website without having the content author manually enter it each time the image is used.

Select **Create a new field**, then **Plain text**, enter a label and select **Text (plain)** and then **Continue**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 1.15.56 pm.png" alt=""><figcaption></figcaption></figure>

Accept the standard field settings and select **Save**.

Next, open **Manage form display** and move the field to your desired position.

Media types often have multiple [View modes](../designing-and-planning-content/manage-display-and-view-modes.md) out-of-the-box, so when you select **Manage display**, you'll see them listed along the top.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 1.20.27 pm.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
We will [customise a view mode](customise-view-mode-for-media.md) in an upcoming lesson.
{% endhint %}

In each of these **view modes**, the field we added will appear automatically in the **Disabled** area. This is useful because it means the photographer's name won't display in the media library (which would created a cluttered UI).

Instead, we're going to create our own custom view mode with an image style that embeds this image on our speaker pages to display the images correctly, and provide proper credit.
