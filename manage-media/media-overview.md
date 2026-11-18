# Media overview

**Media** is the module responsible for managing all the file uploads on your website - from banner images to publication PDFs and local videos.

By default you’re provided with the following media types in GovCMS:&#x20;

* Audio
* Document
* Image
* Remote video
* Video

{% hint style="info" %}
CivicTheme also includes the Icon media type.
{% endhint %}

However, as with content types, you can create additional media types and customise them with additional fields.

{% hint style="warning" icon="image" %}
It's very rare that you will add additional media types to your website.
{% endhint %}

### Media types

<figure><img src="../.gitbook/assets/image (96).png" alt=""><figcaption></figcaption></figure>

Media entities are similar to **content types:** you can [add fields](../designing-and-planning-content/add-and-configure-fields.md), [change display modes](../designing-and-planning-content/manage-display-and-view-modes.md), display them to the public and so on. The main difference is that each media entity is associated with a single actual **file** that matches its type. This means you can't create a **document** media entity without uploading a DOCX or PDF file, and you can't create an **audio** media entity and try to attach an image file.

Each media asset is created with two components: the **file** itself and the media **entity**.

The **file** is the actual PDF or JPEG that's uploaded to a folder on your website. On its own, it's just a file.

When a file is uploaded as part of a media **entity**, you get additional metadata and the ability to easily embed it in your website.

For example, if you just had a **file** on your website, you could add it to a page and it would display as a standard image file.

But when it's connected to a media entity, you can also capture the username of the person who added it, a full revision history of when it was created or altered, additional metadata such as Alt text, or an image caption. You can also dynamically resize media entities and display them easily in multiple locations around the website.
