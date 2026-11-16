# Adding a Solr search page

Now that the Solr search server and index are configured, let's create a user interface so that our public users can query it.

To do that, we use **views**. Return to the Views listing page (**Structure**, then **Views**), and then select **Add view**.

This time, rather than selecting show **Content**, we'll select the index we created.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-22 at 5.16.29 pm.png" alt="" width="563"><figcaption></figcaption></figure>

Then select **Create a page**, and select **Save and edit**.

By default, all views are given a views cache. However, this isn't compatible with Solr searches, and a warning will appear that the cache mode has been changed automatically. This will disappear once we save the view.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-22 at 5.22.28 pm.png" alt=""><figcaption></figcaption></figure>

First, let's add in the fields that we indexed earlier.

Beside **Fields**, select the **Add button**.

In the **Search field**, search for the string **(indexed field)**. This will return just the fields that we have indexed in Solr.

Select the fields we want to display, which is the **Changed**, **Content type** and **Title** fields.

We won't select the **Body** field. Instead, search for the field **Excerpt**. Selecting this field instead will allow us to display a highlighted excerpt from the body content that will show the searched for phrase in-situ.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 11.52.28 am.png" alt=""><figcaption></figcaption></figure>

**Select the fields** that we added to the Solr configuration and select **Add and configure fields**.

Now we need to configure each of the fields.

For the **Changed** field, choose a **date format** that you like:

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 11.13.27 am.png" alt="" width="375"><figcaption></figcaption></figure>

For the **Content type** field, uncheck the **Link label to the referenced entity** field:

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 11.11.31 am.png" alt="" width="375"><figcaption></figcaption></figure>

For **Title**, check the box **Link to the Content** so our users can navigate to the content:

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 11.12.26 am.png" alt="" width="375"><figcaption></figcaption></figure>

For **Excerpt**, we want to ensure **Use highlighted field data** is checked, and **Allow safe HTML only**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 11.55.47 am.png" alt=""><figcaption></figcaption></figure>

Use the **Rearrange** option and drag the items into a better display order.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 11.16.10 am.png" alt="" width="375"><figcaption></figcaption></figure>

The view is now set up with a very basic field display, but currently it's not searching any content.

For that, we need to add an exposed **Filter criteria**. In this case, we'll add a single search text field.

Select **Add** beside Filter criteria and check **Fulltext search** and select **Add and configure filter criteria**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 11.20.26 am.png" alt=""><figcaption></figcaption></figure>

Start by checking the box for **Expose this filter to visitors**, and providing a user-friendly **Label**:

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 11.21.23 am.png" alt="" width="375"><figcaption></figcaption></figure>

Change the **Operator** from Contains all of these words, to **Contains any of these words**:

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 11.21.58 am.png" alt="" width="563"><figcaption></figcaption></figure>

Finally, we need to add the **Sort criteria** so the items appear in the correct order. Select the **Add** button beside Sort criteria, check **Relevance** and select the **Add and configure sort criteria** button.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 11.23.28 am.png" alt=""><figcaption></figcaption></figure>

Select **Sort descending**. This will ensure the most relevant item is at the top.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 11.24.05 am.png" alt=""><figcaption></figcaption></figure>

Finally, select **Save** to save the view, and then **View page** to test it out.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-23 at 11.58.37 am.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" icon="rotate" %}
This lesson give you a very basic Solr search. Configuring a more complicated, visually complex and engaging search function is a complex task that requires a lot of constant tweaking to ensure it works as expected.
{% endhint %}
