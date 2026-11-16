# Customise the content administration experience

The Content administration page (/admin/content) is also a view, which means we can customise it using views.

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption><p>The Content administration landing page.</p></figcaption></figure>

To do this, go to the **Views** landing page and search for the view named **Content**, and select **Edit**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-22 at 12.20.06 pm.png" alt=""><figcaption></figcaption></figure>

If you scroll down to the preview area, you an see that it's the same Content admin view that we see at /admin/content.

We can **edit the Fields and Filter criteria** to modify this core part of Drupal.

In this example, let's go to **Filter** and select **Add**, and search for **State** and select **State or Territory** and select **Add and configure filter criteria** button.

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

When configuring a taxonomy filter we need to specify what settings are used. In this case, let's **select the Vocabulary** and the **selection type** and then select **Apply and continue**.

{% hint style="info" %}
While Drupal _should_ already know what taxonomy Vocabulary we're using for the State or Territory field, we still need to select the Vocabulary when adding it as a filter.
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2026-07-22 at 12.40.42 pm.png" alt=""><figcaption></figcaption></figure>

Once added, we can check the box to **Expose the filter**, and update the **Label** to be more concise:

<figure><img src="../.gitbook/assets/Screenshot 2026-07-22 at 12.48.52 pm.png" alt="" width="375"><figcaption></figcaption></figure>

And finally, under **Filter identifier**, shorten that so the URL doesn't get cluttered.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-22 at 12.49.43 pm.png" alt=""><figcaption></figcaption></figure>

Select **Apply** and then **Save** the view.

If you return to the **Content** admin page, you can see the new **State or Territory filter**.

<figure><img src="../.gitbook/assets/image (65).png" alt=""><figcaption></figcaption></figure>

