# Add your taxonomy to a content type

Now that our vocabulary has been created, we need to add it to a content type so our content authors can start using it.

Hover over **Structure**, **Content types**, **Event** and select **Manage fields**.

<figure><img src="../.gitbook/assets/image (56).png" alt=""><figcaption></figcaption></figure>

To add a new field, select **Create a new field**.

In the popup, select **Reference**, as we will be referencing the taxonomy vocabulary that we have built.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-13 at 3.05.07 pm.png" alt=""><figcaption></figcaption></figure>

Give the field a related **Label**, and select **Taxonomy term** as our field type and then select **Continue**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-13 at 3.14.47 pm.png" alt=""><figcaption></figcaption></figure>

The label field will carry over and you'll be presented with the configuration fields similar to how we added new fields in a paragraph or media entity in earlier lessons.

By default any new reference field can only hold a single value. However, because our events might relate to multiple states, we can change the **Allowed number of values** field to **Unlimited**.

Scrolling further down the configuration screen we need to define which taxonomy vocabulary this field will reference.

Select the **State and Territories** vocabulary you created earlier.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-13 at 3.25.54 pm.png" alt="" width="563"><figcaption></figcaption></figure>

This section also contains the checkbox to **Create referenced entities if they don’t already exist**.

Checking this option will allow your content editors to create new taxonomy terms while editing content. This is useful for general topic taxonomies, but not in this instance where we have a set defined list of Australian states.

After you've selected the taxonomy you're using, select Save to continue. Your field will now be added to your content type.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-13 at 3.26.50 pm.png" alt=""><figcaption></figcaption></figure>

Before we test out the field, we should configure its form display. Scroll to the top of the page and select **Manage form display**.

If you scroll down the page you'll see the state field has probably been added as the final field. However in this instance it would make sense if it was placed near the location field. Using the row widget, click and drag it up to **move** it above the **Location** paragraph field.

We can also change the **widget type** for the field.

Currently it's an **autocomplete** field, which means the user will need to start typing the name of each state to select it.

That might be a useful widget type for a taxonomy with hundreds of terms, but we only have a limited number. In this instance, let's select checkboxes/radio buttons. Because we configured the field to allow multiple values, the field will automatically be configured for checkboxes.

If we could only select one value, it would become radio buttons.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-13 at 3.29.11 pm.png" alt=""><figcaption></figcaption></figure>

Once you've selected your preferred widget, scroll down and select the **Save** button.

Now when a content author goes to create an event, they'll be presented with our new state taxonomy displayed as a **list of Checkboxes**, which allows the content author to select multiple terms.
