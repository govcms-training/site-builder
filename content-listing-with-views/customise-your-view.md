# Customise your view

Next, let's turn this simple listing view into a **basic** search view.

{% hint style="info" %}
Views can be used for very simple site search functionality, however it's only useful for small or specific datasets. For larger, more complicated searches you should [use Solr,](../search/search-overview.md) which is covered in a later section.
{% endhint %}

Back on our **Speaker view**, we're going to include a simple name search. Select the **Add** button beside the **Filter criteria** label.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-15 at 1.16.47 pm.png" alt="" width="375"><figcaption></figcaption></figure>

Using the filter, search for **Title**, check the box beside it and select **Add and configure filter criteria**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-15 at 1.50.39 pm.png" alt=""><figcaption></figcaption></figure>

Select the **Expose this filter to visitors, to allow them to change it** checkbox.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-15 at 1.53.29 pm.png" alt=""><figcaption></figcaption></figure>

**Required** would configure it so the view only displays items once a search has been triggered.

**Filter type** allows you to select single or grouped filters. Single filters are your standard field options, however the grouped filters lets you group multiple taxonomy terms together into a single search option. For this example let's leave it as a single filter.

The text in the **Label** field is displayed to the user, so ensure it’s concise.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-15 at 2.03.46 pm.png" alt=""><figcaption></figcaption></figure>

Under **Operator** you can select the type of filter you want.

For certain filters such as for taxonomies or lists, a simple “is one of” is the best option. This allows the view to return an item if it contains that term, but not exclude it if it also contains other terms.

For a text search like this, **Contains** is the best option.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-15 at 2.29.17 pm.png" alt="" width="563"><figcaption></figcaption></figure>

The filter identifier should always be customised to be a short machine name. This is shown in the URL when someone filters your page, and long unnecessary URLs appear unprofessional.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-15 at 2.35.24 pm.png" alt=""><figcaption></figcaption></figure>

Once you've configured the options and selected **Apply**, **Save** the view and **refresh** your view page.

You can now see the exposed filter at the top of the page, allowing users to filter the total list to only items that have a title (speaker's name) that match their input.

### Tweaking the search

There are a few simple actions we can take to enhance the search functionality.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-15 at 2.40.26 pm.png" alt="" width="255"><figcaption></figcaption></figure>

If your website has the Better Exposed Filters module enabled, you can select **Basic** and switch to [Better Exposed Filters](better-exposed-filters.md). This provides additional configuration options.

In this example, select **Settings** and check the **Include reset button** box. You can also alter the names of the buttons.

<figure><img src="../.gitbook/assets/Screenshot 2026-08-24 at 12.33.58 pm.png" alt=""><figcaption></figcaption></figure>

Let's also scroll down and select the **No** beside **Use AJAX.** Check the box and then select **Apply** to enable AJAX for our search page.

<figure><img src="../.gitbook/assets/Screenshot 2026-08-24 at 12.38.42 pm.png" alt="" width="268"><figcaption></figcaption></figure>

Save the view and revisit the **Speakers' listing page**.

When you perform a search the entire page won't refresh, only the content in the search area. A reset button will appear once a search has been made.

### Adjusting the pager

You can adjust the pager to be a mini pager (only showing previous and next arrows) or full pager (showing arrows as well as a full count of available pages).

You can also customise the number of items per page as well as the button labels and an offset, allowing the view to only display items from a certain index onwards.
