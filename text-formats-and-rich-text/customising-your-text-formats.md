# Customising your text formats

To start, hover over **Configuration**, **Content authoring** and select **Text formats and editors**.

<figure><img src="../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure>

This will show you a list of the current text formats and which text editor they use.

The text editor is the toolbar that you see at the top of text fields. In GovCMS this is provided by the CKEditor module, and that's the only option for GovCMS SaaS websites.

{% hint style="info" icon="dumbbell" %}
In this example we're going to create a limited text format for a summary field.
{% endhint %}

### Create the format

To create a new text format, select the **Add text format** button.

Give the new next format a name. In this case let's call it **Summary editor**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-14 at 11.15.58 am.png" alt=""><figcaption></figcaption></figure>

Next we need to select the **roles** that will have permission to use this format. Let's select Authenticated user, as this includes all of my content authors and administrators, and excludes the public users.

Finally I’m going to select a text editor of CKEditor 5.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-14 at 11.19.17 am.png" alt="" width="179"><figcaption></figcaption></figure>

This will load a toolbar configuration section.

Now that we've entered the basic settings for our text format, it's time to configure its various options and settings.

The **Toolbar configuration** section is broken into two sections: **Available buttons** and **Active toolbar**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-14 at 11.22.53 am.png" alt=""><figcaption></figcaption></figure>

Currently we only have the **heading** selector dropdown, **bold** and **italics** in the available toolbar.

You can add in new options by clicking and dragging icons **from the available** section **into the active** section.

For the use case of a summary field let's disable **Heading** by dragging it out of active, and enable **Underline** and **Remove format** by dragging them into the active toolbar area.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-14 at 11.27.12 am.png" alt="" width="306"><figcaption></figcaption></figure>

{% hint style="info" %}
You can enable any button you want. Each button may require additional configuration, which will appear below. A full overview of these options is available on the [Available toolbar buttons](available-toolbar-buttons.md) page.
{% endhint %}

### Available filters

Below the plugin settings is the list of available filters.

Filters are a series of checks and balances that can run against a text field when the user tries to save. Filters clean up any mistakes and prevent issues.

In this example we're going to check **Limit allowed HTML tags and correct faulty HTML**, because we want a filter to ensure that if a content editor has been writing HTML directly in the source mode that the website corrects any mistakes they may have made.

### Filter processing order

Below the filters is the filter processing order.

Some filters must be processed before others. For example you might want to convert URLs into links before correcting faulty HTML. Since we only have one plugin, we can ignore this for now.

### Filter settings

For filter settings, because we’ve selected that we want to limit the allowed HTML element, we can now define which HTML elements we want to limit.

As you can see from the screenshot below, it's inherited the settings from the style plugin, allowing the line break, paragraph, strong, emphasis and underline tags that the active buttons will use.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-14 at 11.38.46 am.png" alt=""><figcaption></figcaption></figure>

The more buttons you enable, the more tags will be automatically populated in this list.

With all of the options configured, select **Save configuration**.

Now that we've created our new format, we need to enable it to be used somewhere.

For this, we'll use the same steps we completed earlier when [adding a new field](../designing-and-planning-content/add-and-configure-fields.md), and create a new **formatted text** field in the **Speaker** content type called **Short summary**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-14 at 11.41.11 am.png" alt=""><figcaption></figcaption></figure>

After selecting Continue, scroll to the bottom and select your new format under Allowed text formats.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-14 at 11.42.06 am.png" alt=""><figcaption></figcaption></figure>

As the help text suggests, selecting multiple text formats will allow the content editor to choose which one they want to use. Having just a single option will only allow that option to be used.

{% hint style="info" %}
Don't forget, we're adding a new field so ensure you check the [Manage form](../designing-and-planning-content/manage-form-display.md) and [Manage display](../designing-and-planning-content/manage-display-and-view-modes.md) pages to customise them.

In this instance we're going to use the **Short summary** in any listing or search results, so you can set the field to be **Disabled** in the Manage display screen.
{% endhint %}

{% hint style="info" icon="lock" %}
If only a single option is selected and a user doesn’t have permission to use that format, then they will be presented with a disabled field.
{% endhint %}

Now when you edit or create a Speaker, you can see the new field using the new toolbar, and it's configured with the options we selected.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-14 at 11.45.20 am.png" alt=""><figcaption></figcaption></figure>

