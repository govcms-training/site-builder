# Configuring Solr

{% hint style="info" %}
If your website doesn't have Solr enabled (if you don't see Lagoon Solr on the Search API landing page) then please raise a Service Desk ticket to have it enabled.
{% endhint %}

<figure><img src="../.gitbook/assets/image (70).png" alt=""><figcaption></figcaption></figure>

In the screenshot above, we can see the **Lagoon Solr server** with no configured indexes for search. To fix this, select the **Add index** button at the top of the page.

Add an index **name** and configure the **Datasources**, which is the entity types we'll be indexing.

Since we're making a general website search, let's call the search **All content** and select the **Content** datasource.

Further down we need to configure the content types to include. First, make sure you select the **Only those selected** option, and then select:

* Event
* Page
* Speaker

Under **Server**, select **Lagoon Solr**.

<figure><img src="../.gitbook/assets/image (71).png" alt=""><figcaption></figcaption></figure>

All other options can stay as the default settings for the moment.

Once configured, select **Save and add fields**.

You'll then have the ability to **Add** fields to the search index. These are the fields that users will be able to target with their queries.

For now, scroll down and find **Title** and select **Add**, and then **Done.**

<figure><img src="../.gitbook/assets/Screenshot 2026-07-22 at 4.44.05 pm.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" icon="circle-question" %}
When you select Add, the screen will not change. This is because the request was completed behind the scenes. If you select Add more than once, you'll be able to remove the additional title fields on the next screen.
{% endhint %}

This will take us to the **Fields configuration page**. Select **Save changes** to save this new index before we continue to make additional changes.

You'll see the following message at the top of the screen.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-22 at 4.46.16 pm.png" alt=""><figcaption></figcaption></figure>

Each time you make changes to the index's settings, Solr **re-indexes the content**. Basically this means any time you change what fields are going to be indexed, or how they're going to be processed, Solr needs to go through your website and refresh its internal database to make sure it has the right settings.

Before we cover re-indexing, select the **Add fields** button so we can add some more fields.

Find and add the following fields:

* Content type
* Changed
* Body

{% hint style="info" %}
You'll notice every time you select Add there's a short loading icon and then the page looks the same. This is because the new fields are being added behind the popup.
{% endhint %}

Select the **Done** button when you're finished adding fields. You should now be able to see the new fields

<figure><img src="../.gitbook/assets/Screenshot 2026-07-22 at 4.50.44 pm.png" alt=""><figcaption></figcaption></figure>

Select **Save changes** again to save these new fields.

Now we have the fields that our users can target with their search queries.

Next we want to add some processors so that we aren't just doing simple text string matches.

Select the **Processors** tab at the top.

This page provides a list of various processors that can be used to subtly alter our users' search queries.

Each item includes a short description. For example, **Boost more recent dates** will boost more recent documents and penalise older documents.

For this example, let's enable **Boost more recent dates**, **Highlight**, **HTML filter** and **Type-specific boosting**.

Once those are enabled, additional configuration will be provided in the **Processor settings** at the bottom of the page.

**Highlight** allows us to configure how long the highlight will be and what tags to use to wrap it. The default options here are fine.

**HTML filter** allows you to provide boosts depending on the text fields in which results are found. For example if two pages both have the phrase "Licence renewal" but one of them has that as a heading 2, and the other only has it in paragraph text, the page with the search term as a heading is probably more relevant to the user, so those results can be boosted. This section allows you to configure that, however the default settings will work fine for us.

We can configure **Type-specific boosting** so that **normal content pages** receive a 1x boost, **events** receive a 2x boost, and **speaker content** receives a .8x boost.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 11.33.26 am.png" alt=""><figcaption></figcaption></figure>

This will mean that **events are twice as important as normal pages**, and speakers are slightly less important than pages.

Once this is configured, select **Save**.

This time, when the alert appears at the top of the page about re-indexing, **select the link** or select the **View** button in the tab navigation.

<figure><img src="../.gitbook/assets/image (72).png" alt=""><figcaption></figcaption></figure>

This page shows the total content on the website, and how much of it has been indexed in the Solr server. In the above example, you can see that there are 11 entities that should be in our search, but Solr hasn't indexed them.

Select the grey **Index now** button.

{% hint style="info" %}
If your website has tens of thousands of items, indexing them all at once can cause massive sever performance issues. In this situation, using the **Queue all items for indexing** option is better, but slower.

When new content is added or content is modified, Solr automatically indexes those changes, so full site indexes are fairly rare.
{% endhint %}

Once the progress bar finishes and the page refreshes, the Solr index has been updated with all the new content and is ready to be queried.
