# Manage form display

Now that a new field has been created, we should check the form display to see how it will be displayed to content authors.

Select **Manage form display** from the tab menu located near the top of the page content.

The Manage form display page allows you to customise how the form will display for content authors. As content authors spend more time on your website than any visitor, it’s important to make a user-friendly interface for them.

The Manage form display page allows you to customise the order of the fields. Depending on the field, it also allows you to change the input method presented to the user.

<figure><img src="../.gitbook/assets/image (49).png" alt=""><figcaption></figcaption></figure>

### Reorder elements

You can reorder the fields using the row control widget to the left of each label. Simply click and drag the row to your preferred order and select the **Save** button.

You can also drag elements into the Disabled section if the field is not required.

The only caveat for field reordering is that some items listed in this form can't have their order changed as they are core components of the form:

* Authored by
* Authored on
* Published
* URL alias
* URL redirect
* Moderation state

These items (Except for **Published** and **Moderation state** which appear directly above the **Save** button) will all appear in the right-hand **Properties** column when editing content.

### Field widgets

In Drupal, a widget is the name given to the type of form input a field has. For example a field allowing you to select a list of items could be given a field widget of checkboxes, radio buttons, select list (dropdown) or autocomplete text field.

Each field widget has its unique user behaviour, and you can use the **Form Display** page to configure these.

For example, if you have a taxonomy field with hundreds of items, and the user can only select one item, then a select list would be more user-friendly than a radio button, which would require every single term listed out on the page.

Whenever you change a field widget, you need to scroll to the bottom of the page and select the **Save** button for it to take effect.

### Field group

If your website has the **Field Group module** enabled, you can also group fields together with headings or tab navigation, to make the interface easier to use.

If you select the Field Group button you'll be presented with a select list allowing you to add a new display element to your form.

You can select from Details, Details Sidebar, Fieldset, Tabs, Tab or HTML element.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-13 at 11.39.40 am.png" alt="" width="292"><figcaption></figcaption></figure>

Once you select an element you'll need to enter a name and select **Save and continue**.

In this example, we've selected a Fieldset. We can now add additional information such as a description and any additional CSS IDs or classes you need.

<figure><img src="../.gitbook/assets/image (50).png" alt=""><figcaption></figcaption></figure>

Once this is configured, select **Create group**.

All new field groups are created in the **Disabled** section at the bottom of the page.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-13 at 11.42.20 am.png" alt=""><figcaption></figcaption></figure>

You‘ll need to scroll to the bottom of the page, select the toggle for the new field group and drag it up to the active section.

Then use the toggles to drag in any fields you want to display inside that field group.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-13 at 11.46.04 am.png" alt=""><figcaption></figcaption></figure>

Once you've organised your fields, scroll down and select **Save**.

This will turn your editing interface into the following:

<figure><img src="../.gitbook/assets/image (51).png" alt=""><figcaption></figcaption></figure>

Other field groups, like Tabs and Details, require specific nested layouts to work correctly.
