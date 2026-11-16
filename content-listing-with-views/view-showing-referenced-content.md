# View showing referenced content

Earlier in the training we created a **Speaker** field on the event to list the speakers attending the event.

Currently, that field is a simple text label link (although it could be expanded using a Rendered entity format). In this exercise we're going to use views to create a rich list of the speakers for an event.

First, we need to create a new view. Go to **Structure**, **Views** and select **Add view**.

<figure><img src="../.gitbook/assets/image (83).png" alt=""><figcaption></figcaption></figure>

Counter intuitively, we're going to create a view of **events**, NOT _speakers_.

{% hint style="info" %}
If we were to create a list of speakers, we wouldn't have any easy way of knowing WHICH speakers we want to display. Instead, we'll create a list of events, and then use relationships to connect the event with the related speakers.
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 1.22.59 pm.png" alt="" width="563"><figcaption></figcaption></figure>

Select **Create a block**, with an unformatted list of fields.

<figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 1.23.40 pm.png" alt="" width="563"><figcaption></figcaption></figure>

Select **Save and edit** to continue.

If we go into **Add a field**, you can select **Biography** (Formatter: Trimmed. Trimmed limit: 256) and **Photograph** (Formatter: Thumbnail. Image style: Medium), which are the fields we want for our speakers. But if you **view the preview**, all you can see is the trimmed Body field from the event, because that field is shared (as you can see from the **Description** in the **Add fields** UI screenshot below). However **Photograph** is unique to speaker, so we don't see anything.

<figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 1.35.08 pm.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 1.38.29 pm.png" alt="" width="563"><figcaption></figcaption></figure>

We need to tell the view that the **Title**, **Biography** (Body) and **Photograph** field should actually be sourced from the speaker, even though we're viewing the event.

To do that, in the advanced column, select **Add** beside **Relationships**.

<figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 1.40.16 pm.png" alt="" width="375"><figcaption></figcaption></figure>

Search for speaker and select the row stating we want a relationship to content that is r**eferenced from the field\_speakers** field. Select **Add and configure relationships** to continue.

<figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 1.40.34 pm.png" alt=""><figcaption></figcaption></figure>

This relationship doesn't require any configuration, so select **Apply** on the next screen.

We now have a relationship to the content that's referenced in that field on our nodes. This allows us to pull field content from the speaker content and display it on the event.

Go back to the **Fields** column, and for each of the fields change the field to use our new **Relationship** and select **Apply**.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 1.49.36 pm.png" alt="" width="213"><figcaption></figcaption></figure>

Now in preview, the speaker content is visible, even though we're technically viewing events.

<figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 1.51.44 pm.png" alt=""><figcaption></figcaption></figure>

As it stands, we have a **view** creating a **block** that shows **all the speakers** for **all events**.

The last thing we need to do is add a **Contextual filter** for this view so that it only shows speakers for the event we're looking at, and then embed this vlock on all event pages.

Select **Add** beside **Contextual filters**, and add the **ID** filter. Configure it to provide the default value of the **Content ID from URL**.

It's important to note that we don't want to use the relationship here, as we want to use the event ID, not the speaker.

<figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 1.58.22 pm.png" alt=""><figcaption></figcaption></figure>

Finally, using **Block layout**, place the block on **all Event content type** pages.

<figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 2.00.10 pm.png" alt=""><figcaption></figcaption></figure>

Now when viewing an **event**, we can see our view of **Our speakers**, which shows more field information than was available with the basic field.

<figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 2.02.15 pm.png" alt=""><figcaption></figcaption></figure>
