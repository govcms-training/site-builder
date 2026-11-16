# Context

Context allows you to set **conditions** and **reactions**. This can be used to manage your blocks in bulk rather than individually via the Block layout page.

For example, you can have a **condition** set of **content type**, with a **reaction** to **disable the header and footer regions** entirely, and then move all the blocks into the **Content** region to create a single column page layout.

Or you could create a new theme entirely for a certain section of your website, and then use **context** to switch the theme based on the URL path.

To view your **contexts**, select **Structure** and then **Context**.

<figure><img src="../.gitbook/assets/image (79).png" alt=""><figcaption></figcaption></figure>

To create a new **context**, select the blue **Add context** button.

Enter a **Label** and select **Save**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-30 at 11.45.00 am.png" alt="" width="563"><figcaption></figcaption></figure>

At the bottom of the next page we can select the **Conditions** and **Reactions**.

<figure><img src="../.gitbook/assets/image (80).png" alt=""><figcaption></figcaption></figure>

Select **Add condition**, scroll down and select **Content type (node)**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-30 at 11.46.46 am.png" alt="" width="375"><figcaption></figcaption></figure>

When the popup closes, check the **Event** checkbox in the **Content type list**.

Then select **Add reaction** and select **Regions**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-30 at 11.48.15 am.png" alt="" width="375"><figcaption></figcaption></figure>

Expand the **Disable Regions in GovCMS Training (Default)** and check every **region** in the **Header**, **Sidebar** and **Footer** to disable them.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-30 at 11.50.09 am.png" alt=""><figcaption></figcaption></figure>

Select the **Save and continue** button at the bottom of the page, then use the **Content list** to browse to an **Event node**.

{% hint style="warning" %}
If you do not see the change immediately, you may need to clear your Drupal cache. On GovCMS this is done using the Lagoon Dashboard. Contact your developers for help with this.
{% endhint %}

<div><figure><img src="../.gitbook/assets/image (81).png" alt="" width="375"><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/image (82).png" alt="" width="375"><figcaption></figcaption></figure></div>

Above you can see a comparison of an event node with the context enabled or disabled.

{% hint style="danger" icon="hand-point-up" %}
If you use context to manage block layout for a certain criteria, make sure you document it, otherwise you might be trying to troubleshoot the layout in the future, and end up in the Block layout screen unable to work out why certain blocks are displaying in certain regions.
{% endhint %}

### Available conditions

**Require all conditions** is a checkbox above the Conditions list that allows you to define if every single condition must be active for the context to be active.

There are 24 different available condition checks in GovCMS. Below is a list of the most commonly used conditions, however feel free to explore the full list in your own time.

**Language (language)** - Handy if you're building a multi-lingual website and need different blocks or templates depending on the selected language.

**Request Path (system)** - A simple method of switching context depending on what page or section of the website the user is viewing.

**User Role (user)** - Could be useful if you want to provide additional blocks with editor-specific information or guidelines to users with the Content Approver role.

**Content type (node)** - Most commonly used to provide layout differences based on what content type the user is viewing.

### Available reactions

**Regions** - As demonstrated above, regions allows you to disable theme regions.

**Menu** - This is not available in the training environment.

**Page title** - Override the page title with a set string.

**Body class** - Adds an additional string to the \<body> HTML element. Can be handy for section-specific styling.

**Page template suggestions** - Allows you to provide additional page template suggestions for the page.html.twig template file.

**Theme** - Switch entire themes based on conditions.

**Blocks** - Configure custom block layouts for set conditions. Can act as additive to the default blocks defined in your block layout, or be an entire replacement option.
