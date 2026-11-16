# Creating a taxonomy vocabulary

In this example we're going to create a vocabulary for Australian states and territories, and then apply it to our **Event content type** so that users can find events near them.

Hover over **Structure** and **Taxonomy** and select **Add vocabulary**.

<figure><img src="../.gitbook/assets/image (53).png" alt=""><figcaption></figcaption></figure>

Enter in a **Name** and an optional **Description** and select Save.

{% hint style="info" %}
The description is only shown on administrative landing pages.
{% endhint %}

You'll be presented with your new empty taxonomy vocabulary.

<figure><img src="../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>

Vocabularies are similar to content types, in that **they can have fields** and **custom display modes**.

By default all taxonomy terms are given a **Title** field and a **Description** field.

In this example of Australian states, we don’t need a Description field, so we'll remove it by selecting **Manage form display**.

Using the field row widget, move the **Description** and **URL alias** fields to **Disabled**.

These fields will retain their default values, but we won't ask content editors to manually add them.

Once the fields are under the Disabled heading, select **Save**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-13 at 2.54.51 pm.png" alt=""><figcaption></figcaption></figure>

Now when a user adds terms to this vocabulary, they'll be presented with just the fields we need them to fill in.

Select **List** to return to the list of terms.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-13 at 2.56.50 pm.png" alt=""><figcaption></figcaption></figure>

Now, we'll add some individual **terms** to our vocabulary **container**.

Select the **Add term** button.

Thanks to our work on the Manage form display page, we're presented with a minimal interface.

Enter a **term name** and select either **Save** to add the term and reload the page so you can quickly add a new term, or **Save and go to list** to add the term and return to the vocabulary list.

Once all the terms are added, return to the vocabulary to see the full list of terms.

<figure><img src="../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure>

You can reorder them using the click and drag row widget, making sure you select the **Save** button located at the bottom of the page when you're finished.

The order of the items appear on this screen is the order they'll appear in when displayed as lists to content authors.

{% hint style="info" icon="rectangle-plus" %}
In addition to adding terms directly to a vocabulary, you can also set up your content type so users can define new terms on the fly when adding content. This is covered later.
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2026-07-13 at 3.55.08 pm.png" alt="" width="237"><figcaption></figcaption></figure>

### Adding custom fields to a vocabulary

You can also add custom fields to your vocabulary just like content types and paragraphs.

This can be useful to pull additional information through to pages with a term applied.

To expand on our current example of events and states, you might have a different primary contact per state to help with organisation, or you might have a different logo for each state.

You could customise your taxonomy vocabulary and add an email and a media (image) field, so that each term requires additional data.

Then you can set up the page template for an event so that it displays not just the label of the state, but it also pulls through the additional information added to the term and display the email address and image.

In addition, because the taxonomy term is reused across multiple pieces of content, if the image changed or the state contact changed, you could update the taxonomy term itself once, and all events that referenced that term would be updated as well.
