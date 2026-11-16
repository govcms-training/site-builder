# Views showing related content

For this example, we'll use the Event content type and the state or territory field that we created earlier, and create a list of geographically related events.

{% hint style="info" icon="earth-oceania" %}
If you haven't already, create some test event content with different states selected.
{% endhint %}

To start, we will need a view of events.

Using what we learned when [creating a view](create-a-view.md), create a view with the following:

* **View name**: Related events
* Show: **Content** of type **Event**, sorted by **Newest first**
* Block settings: Check **Create a block**
* Display format: **Unformatted list**, output as **fields**
* Items per block: **3**

Then using the [place a block](../blocks-and-menus/placing-a-block.md) lesson, place that block on the event page in the bottom of the content region.

This will display the latest three events on the bottom of every event item.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-16 at 5.23.44 pm.png" alt="" width="326"><figcaption></figcaption></figure>

However, our goal is to only list events with the same state or territory.

To do this, we need to add a contextual filter. Unlike a normal filter, contextual filters are dynamic and change based on variables.

In the view, beside **Contextual filter**, select the **Add** button.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-16 at 5.26.04 pm.png" alt="" width="375"><figcaption></figcaption></figure>

Using the filter, we can limit the list to find the field we want to filter by, in this instance it's the **State or Territory** field.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-16 at 5.34.40 pm.png" alt="" width="563"><figcaption></figcaption></figure>

The second row is fields delta. Delta allows you to filter based on one specific term. For example, only filter on the second selected taxonomy term. We won't be using that.

Select the checkbox for the first row and then **Add and configure contextual filters**.

On the next page we need to configure how we're going to use this filter.

In the radio list, select **Provide default value**. This is set up so that when a filter value isn't automatically provided (such as via theme code or URL variable) then the view should provide a value.

Selecting this provides additional options we need to configure.

For **Type**, select **Taxonomy term ID from URL.**

Then uncheck **Load default filter from&#x20;**_**term**_**&#x20;page**, and check **Load default filter from&#x20;**_**node**_**&#x20;page**, and **Limit terms** **by vocabulary** and then check the specific vocabulary, in this case, **State and Territories**.

And finally, select **Filter to items that share any term**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-16 at 5.39.27 pm.png" alt="" width="375"><figcaption></figcaption></figure>

To summarise what was just configured:

* The default value will be a **Taxonomy term ID from the URL**. This doesn’t mean we get an actual ID from the URL alias, it means we're going to load all taxonomy terms from the node we're viewing, which is determined by the current URL
* Then, to ensure we're only showing content that shares our state or territory term (and not subject or site sections), we check the options that allow us to **limit terms by vocabulary**, and select **State and Territories**.
* Finally we select that this filter can **share any term**, not all terms. This means that if the page has at least one matching state it will show.

Select **Apply** to save the filter, and then **Save** to save the view.

Now, if we go back to an **event**, the items listed under **Related events** will only be items that share a state or territory taxonomy term with the event you're viewing.

You may notice that the node we're currently viewing is also included in the list, because it matches the criteria for the view.

We need to clean this up by returning to the view, and adding another contextual filter.

This time, use the filter for **ID**, scroll down and select the row called just **ID**, and then select **Add and configure contextual filter**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-16 at 5.57.41 pm.png" alt=""><figcaption></figcaption></figure>

\
Select **Provide default value**, and then **Content ID from URL**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-16 at 6.00.37 pm.png" alt="" width="327"><figcaption></figcaption></figure>

This filter is now filtering based on the **Node ID** of the page we're viewing at any given time.

Scroll to the bottom, expand **More** and select **Exclude**.

This will exclude the **current node ID** from being returned as a valid node in the list of related events.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-16 at 6.03.56 pm.png" alt="" width="563"><figcaption></figcaption></figure>

Select the **Apply** button and then **Save** the View.

Now, when we **reload the event page**, we can see that the **list doesn't include itself**.
