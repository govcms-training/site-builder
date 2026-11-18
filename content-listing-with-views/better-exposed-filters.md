# Better exposed filters

Better Exposed Filters (or **BEF**) is a module recently added to the GovCMS distribution that adds additional options when setting up a simple view with exposed filters.

While not as feature-rich as [Facets](../search/facets.md), it provides more configuration options.

In the below example we're using a view with the following settings:

* A simple list of every node on the website as an HTML table
* Exposed filters for **Title**, **Authored on** and **Content type**
* Exposed **Sort by** changed
* Pager enabled and exposed

{% hint style="info" icon="filter-list" %}
Better Exposed Filters alters field display settings and templates, which may or may not be compatible with your theme. The Training website uses CivicTheme, so some changes made to BEF options are not reflected in the CivicTheme templates.
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2026-07-30 at 12.28.00 pm.png" alt=""><figcaption></figcaption></figure>

Go to configure the view, and under **Exposed form** select **Basic**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-30 at 12.25.02 pm.png" alt="" width="260"><figcaption></figcaption></figure>

Select **Better Exposed Filters**, and then **Apply**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-30 at 12.25.13 pm.png" alt="" width="375"><figcaption></figcaption></figure>

In addition to the basic settings such as reset button, input required, etc., we also have options to configure our exposed sort settings, pager and filter settings.

### Exposed sort settings

This section allows us to change aspects of our **sort** controls, such as **labels.** The advanced options let you include a **Reset** button just for the sort control.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-30 at 12.30.23 pm.png" alt="" width="563"><figcaption></figcaption></figure>

### Exposed pager settings

This allows you to change the exposed widget, from the default dropdown to radio buttons or a links list.

<div><figure><img src="../.gitbook/assets/Screenshot 2026-07-30 at 12.33.51 pm.png" alt="" width="346"><figcaption><p>Default</p></figcaption></figure> <figure><img src="../.gitbook/assets/Screenshot 2026-07-30 at 12.33.21 pm.png" alt="" width="342"><figcaption><p>Radio buttons</p></figcaption></figure></div>

### Exposed filter settings

For **text** inputs (such as page title), you can control the **Placeholder text**, hide the field label and add additional CSS classes for styling.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-30 at 12.38.54 pm.png" alt="" width="375"><figcaption></figcaption></figure>

For **date-**&#x62;ased fields, BEF allows you to swap exposed **Date filters** from text fields to **Date picker** calendar options.

<div><figure><img src="../.gitbook/assets/Screenshot 2026-07-30 at 12.35.44 pm.png" alt="" width="342"><figcaption><p>Default widget</p></figcaption></figure> <figure><img src="../.gitbook/assets/Screenshot 2026-07-30 at 12.36.09 pm.png" alt="" width="344"><figcaption><p>Date picker widget</p></figcaption></figure></div>

For **list-**&#x62;ased options such as **taxonomy** or **select lists**, you can **rewrite values** before they're output, which can be useful if your terms were originally designed to only be internally facing.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-30 at 12.42.05 pm.png" alt="" width="531"><figcaption></figcaption></figure>
