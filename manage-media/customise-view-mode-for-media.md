# Customise view mode for media

As covered in previous sections we have [media types](media-types.md) with [image styles](image-styles.md), and media can also have [view modes](../designing-and-planning-content/manage-display-and-view-modes.md).

In this section, we'll take a **media entity** and display it on our website using a custom **view mode** and **image style**.

We'll update the **Speaker content type** so that the photo of the speaker is better formatted for our needs.

At this point we have:

* A Speaker content type with an photo (media/image) field
* Our image media type has an additional text field for photographer that isn't displaying anywhere yet
* An image style that will format our photo into a vertical portrait resolution

We need to combine all of those using a **view mode**, and then enable that view mode for our speaker photo field.

### Create the view mode

Go to **Structure**, **Display modes**, **View modes** and select **Add view mode**.

<figure><img src="../.gitbook/assets/image (46).png" alt=""><figcaption></figcaption></figure>

We need to select the entity type we want this view mode enabled for. We want to create a custom view mode for an image media entity, so select **Media**.

We'll then need to define the settings. In this case, it's going to be called **Speaker** photo, and applied to the **Image** media type. Once the configuration is complete, select **Save**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 5.08.48 pm.png" alt=""><figcaption></figcaption></figure>

You'll be returned to the **View modes** landing page, however you can use a shortcut to go directly to the Image view mode and start customising it.

Select the link in the status message, or go to **Structure, Media types, Image, Manage display**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 5.10.13 pm.png" alt="" width="563"><figcaption></figcaption></figure>

Here we can see that we're editing the **Speaker photo** View mode for the **Image media type**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 5.11.34 pm.png" alt=""><figcaption></figcaption></figure>

In the fields section below, configure the fields to display for this view mode.

First, select the new **Image style** that we configured.

Select the cog on the far right of the Image row, and change the **Image style dropdown** to the new image style we created. Once that's finished, select **Update**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 5.12.54 pm.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Selecting Update on any field will only temporarily save that field settings. To make changes permanent, you need to select the **Save** button at the bottom of the page.
{% endhint %}

In our use case, we don't want the **Caption** or **Media** **tags** fields, but we do want the new photographer/source field.

So we can use the **drag controls** to drag those items out of the Disabled section. And finally, we want to hide the **Label** for the new field.&#x20;

You'll end up with a screen that looks like this:

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 5.16.15 pm.png" alt=""><figcaption></figcaption></figure>

Scroll down and select **Save** to make these changes permanent for this view mode.

Now we have a custom **View mode**, we need to set the **Speaker content type** to use it.

Start by opening any speaker content. If you've followed the exercise from earlier, it will look something like this:

<figure><img src="../.gitbook/assets/image (47).png" alt=""><figcaption></figcaption></figure>

Select the **Manage display** tab to go to the Manage display section for the Speaker content type. Then scroll down and find the photo field.

Select the **cog** associated with that row, and change the **View mode** to our newly created **Speaker photo** view mode.

Select **Update** and then **Save**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 5.19.25 pm.png" alt=""><figcaption></figcaption></figure>

You'll be returned to the page, but now the new **View mode** and subsequent **Image style** will be enabled, and our text field will be displayed below it.

<figure><img src="../.gitbook/assets/image (48).png" alt=""><figcaption></figcaption></figure>

### In review

The **image style** sets how the image will be displayed. A **view mode** then implements that image style. And finally the **content type** is configured to display that view mode.

<figure><img src="../.gitbook/assets/Screenshot 2026-08-24 at 2.19.33 pm.png" alt="" width="563"><figcaption></figcaption></figure>
