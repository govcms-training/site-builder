# Facets

Facets are more complicated and advanced **exposed filters**. A simple exposed filter could be a dropdown list of items, while facets allow the list to include a count of how many items are going to be filtered. It's also dynamic, so items that provide no additional filtering are removed from the list.

There are a few different types of facets. In the example below, we'll implement a simple checkbox facet for content type.

To add a facet to a search, go to **Configuration**, **Search and metadata** and then **Facets**.

<figure><img src="../.gitbook/assets/image (73).png" alt=""><figcaption></figcaption></figure>

This page lists all your facet **sources**, which are any views that were created based on search API. In the screenshot above, we can see the default CivicTheme search that comes bundled with the Training environment, and then the **site search** that we created in the last lesson.

Select the **Add facet button.** Select the **Site search facet source** and add a **Name** and then select **Save.**

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 12.20.21 pm.png" alt="" width="563"><figcaption></figcaption></figure>

This will display an error message, but the page will then display a field dropdown where you can select what **Field** you want this facet to filter on. Select **Content type** and then select **Save**.

The next page/screen includes a lot of configuration options for the facet (way more than a simple exposed view filter).

<figure><img src="../.gitbook/assets/image (74).png" alt=""><figcaption></figcaption></figure>

For our use case, we're going to configure:

* **Widget**: List of checkboxes
* **List of links settings**: Show the amount of results, Show reset link and Hide reset link when no facet item is selected.
* **Hide non-narrowing results**
* **List item label**

And select **Save**.

If selecting Save **does nothing**, you need to scroll back up, change **Empty facet behaviour** from **Do not display facet** to **Display text**, and then **select a Text format**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 12.28.56 pm.png" alt=""><figcaption></figcaption></figure>

Then **switch it back to Do not display facet**.

And then select **Save**.

{% hint style="info" %}
This is because the text format field is mandatory, so it requires a value, even if no empty text is being provided. It's a known bug - annoying, but with a workaround.
{% endhint %}

Now that the facet has been created, we need to display it.

As the message noted at the top of the facet configuration page, **the facet is a block** and can be placed just like any other block.

Since we've [already covered how to place a block](../blocks-and-menus/placing-a-block.md), go ahead and **place this block** on your search page, in the **Sidebar Top Left** region.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 12.32.27 pm.png" alt=""><figcaption></figcaption></figure>

You'll notice a new **Visibility** option that lets you set the visibility of this block depending on if we're on a **view page**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 12.33.33 pm.png" alt=""><figcaption></figcaption></figure>

And now when you visit the search page again, you can see **in the sidebar**:

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 12.35.28 pm.png" alt="" width="282"><figcaption></figcaption></figure>

Although we configured this to be **checkboxes**, they're appearing as a text list. This is a **quirk of the CivicTheme** display.

We can see that the **facet filter** is showing the number of items for each content type, and selecting a content type allows us to filter the search results based on that content type.

Selecting an item narrows the list of search results.
