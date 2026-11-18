# Cross referencing content

A great feature of Drupal is the ability to **cross reference content** using entity references fields. We'll cover this again when we create a taxonomy reference, but for now we have **events** and **speakers** who will be speaking at the events, but currently no way to know which speaker will be at which event.

To fix this, let's create an **Entity Reference field** on the **event** to list our associated speakers.

Go to the Event content type's **Manage fields** page by hovering over **Structure**, **Content Types**, **Event** and then **Manage fields**.

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

Select **Create a new field**, and select **Reference**.

<figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 12.30.45 pm.png" alt=""><figcaption></figcaption></figure>

Add a field **label** and select the reference type of **Content**.

<figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 12.31.19 pm.png" alt=""><figcaption></figcaption></figure>

Under **Field Storage**, we want to change the allowed number of values to be Unlimited so that we can reference as many speakers as we want. And under **Reference type** we want to limit this field to only reference **Speaker** content.

<div><figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 12.34.37 pm.png" alt="" width="375"><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 12.34.47 pm.png" alt="" width="375"><figcaption></figcaption></figure></div>

Once the field is configured, select **Save**.

Since we've added a new field, we should confirm the settings in **Manage form display** and **Manage display**.

On **Manage form display** the field is being presented as an Autocomplete field, which in this use case is what we want, because then content authors can search for authors by their name.

<figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 12.36.45 pm.png" alt=""><figcaption></figcaption></figure>

On the Manage display tab, ensure that the **Speaker** is in the **Enabled** section.

<figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 1.10.18 pm.png" alt=""><figcaption></figcaption></figure>

By default the display format will be a simple referenced **Label**, however you could change this to a **Rendered entity** with a specific [View mode](manage-display-and-view-modes.md) to embed a small version of the speaker content on your event page. Alternatively the entity reference field can be used in a view to create a block, which will be covered later.

To confirm our field is working, simply edit an event, scroll down to where the field is located and type in the name of one of the speakers on your website.

<figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 12.41.21 pm.png" alt=""><figcaption></figcaption></figure>

We can add additional speakers by select the **Add another item** button and entering another name.

Once you've selected at least one value, **Save** the node and **view it**.

<figure><img src="../.gitbook/assets/Screenshot 2026-08-10 at 12.52.20 pm.png" alt=""><figcaption></figcaption></figure>

In the screenshot above you can see automatic links have been created to our two speakers for this event. When a user selects those links, they will be taken directly to the speaker's page.
