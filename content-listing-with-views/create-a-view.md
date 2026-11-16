# Create a View

In this section, we’ll build a simple listing of all the Speakers.

{% hint style="info" %}
Before creating the view, create some sample content that we can use when testing the view.
{% endhint %}

Once you have your content created, go to **Structure** and then **Views** to see the **Views administration page**.

<figure><img src="../.gitbook/assets/image (62).png" alt=""><figcaption></figcaption></figure>

This page lists all the existing views, both public and administrative.

Select the **Add view** button.

On this first page you can set up the basic information for the view.

For the view name we’ll use **Speakers**. Adding a name automatically creates the machine name. You can customise this or leave it.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-14 at 2.33.24 pm.png" alt="" width="563"><figcaption></figcaption></figure>

Next choose what you want the View to contain. In this example, let’s select the content type Speaker, sorted by newest first.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-14 at 2.34.26 pm.png" alt="" width="563"><figcaption></figcaption></figure>

We want it to display as a page, so we check the **Create a page** box.

The page title will pre-populate with your view name, and a default path will also be provided. You can change these at any time.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-14 at 2.36.35 pm.png" alt="" width="563"><figcaption></figcaption></figure>

Next, configure the **Page display settings**.

This defines how the content will be structured. An **unformatted** or HTML **list** is usually the most logical option, however other options might suit your specific use case.

For the output, we have selected **fields**. This allows us to choose which fields from the content type we want to display in our list.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-14 at 2.36.45 pm.png" alt="" width="563"><figcaption></figcaption></figure>

Below that we can define how many items will display in the list. By default this is 10, with any items over 10 being available via a simple **Pager**. You can set this to zero if you want all items to be displayed.

{% hint style="info" icon="cards-blank" %}
Any page with large lists containing hundreds of items can cause performance and caching issues.
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2026-07-14 at 2.42.18 pm.png" alt="" width="237"><figcaption></figcaption></figure>



Once you’re happy with the settings, scroll down and select **Save and edit.**

<figure><img src="../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>

Let’s now look at how you can configure your view.
