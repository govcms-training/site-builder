# Views data export

The Views Data Export module allows us to create views that export content into portable formats like CSV, JSON or XML.

This can be useful for exporting lists of content for auditing purposes, or for importing into other third-party platforms.

In this example, we're going to export a full list of every taxonomy term on the website.

To start, go to **Structure**, **Views**, and then **Add view**.

<figure><img src="../.gitbook/assets/image (77).png" alt=""><figcaption></figcaption></figure>

Enter a **View name**, and under **View settings**, select **Taxonomy terms**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-28 at 11.42.00 am.png" alt="" width="563"><figcaption></figcaption></figure>

We won't be creating a page or a block, so just continue down to **Save and edit**.

Using the display bar, we can add a **Data export** display to the View.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-28 at 11.47.32 am.png" alt="" width="375"><figcaption></figcaption></figure>

The first thing we need to do is add a **path** via the **Path settings** section.

Select **No path is set**, and enter a path name ending with **.csv**, then select **Apply**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-28 at 11.54.08 am.png" alt=""><figcaption></figcaption></figure>

This will set the path for our CSV export file. However, we still need to tell the view to output as a CSV file. In the first column under **Format**, select **Settings**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-28 at 12.17.29 pm.png" alt="" width="375"><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot 2026-07-28 at 12.24.39 pm.png" alt=""><figcaption></figcaption></figure>

Select **CSV** and then **Apply**.

{% hint style="info" %}
Other formats are available for other use cases. For simple data export for auditing purposes, CSV is the best choice.
{% endhint %}

### Configuring the fields

Now we need to configure what **fields** will be included in our data export.

For that, we simply add and modify our fields, [just like a normal view](configure-the-view.md).

First, we need to alter the default field that was added to the view to remove the link format and make this a simple text list. Under **Fields**, select **Taxonomy term: Name**, and uncheck **Link to the Taxonomy term**, and then select **Apply**.

Then **Add** a new field, and check **Vocabulary** and select **Add and configure fields**.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2026-07-28 at 12.10.47 pm.png" alt=""><figcaption></figcaption></figure>

Uncheck **Link label to the reference entity** and select **Apply**.

Now that the view is complete, save it, and then select the **View Data export** button in the top right. This will trigger a **download of the CSV file**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-28 at 12.29.44 pm.png" alt=""><figcaption></figcaption></figure>

As you can see from the screenshot below, the CSV file is a simple way to view and audit our taxonomy terms.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-28 at 12.31.29 pm.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" icon="rotate" %}
While Views Data export is a fairly simple and easy way of exporting data from Drupal, it cannot be used to import or alter data already inside Drupal.
{% endhint %}
