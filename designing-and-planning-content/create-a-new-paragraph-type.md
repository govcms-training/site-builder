# Create a new paragraph type

To create a new paragraph type, go to the **Paragraph types** landing page by hovering over **Structure** and selecting **Paragraph types**.

{% hint style="info" %}
This lists out all the existing paragraph types. Just like content types, it's important to investigate if what you want to build can already be achieved without having to create a whole new configuration.
{% endhint %}

Then select the blue **Add paragraph type** button at the top of the page.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 10.31.46 am.png" alt=""><figcaption></figcaption></figure>

Similar to building a new content type, we need to provide a **Label** and **Description**.

{% hint style="info" %}
Paragraphs also allow you to add an icon that's displayed when a user is adding a new paragraph to a page, depending on the user interface.
{% endhint %}

In this example we're going to create a new paragraph type called **Book**. This will be a paragraph we add to our **Speaker** content type that lists all the books our speakers have written.

<figure><img src="../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

Enter in the name and description and select **Save and manage fields**.

Like content types, we can now choose to **Create a new field**, or **Re-use an existing field**. You may notice that when you select Re-use existing field, the available fields are different to those when creating a content type.

This is because although paragraphs and content types both use **fields**, they're saved in the database slightly differently, and thus are not shareable.

{% hint style="info" %}
In the CivicTheme training environment you can see this because fields starting with field\_c\_n\_ are for **fields** in **C**ivicTheme built for **n**odes.

Whereas here we have field\_c\_p\_ for **fields** in **C**ivicTheme built for **p**aragraphs.

This naming convention is only used by CivicTheme.
{% endhint %}

For the Book paragraph type we want a **title**, **summary** and **thumbnail**.

Because the training website has many paragraphs, there are existing fields that suited our purpose. We can simply change their field display name using the exact same steps as [adding a field to a content type](add-and-configure-fields.md).

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 10.54.55 am.png" alt=""><figcaption></figcaption></figure>

Now, just like a content type, we can [customise the Form display](manage-form-display.md) and [View mode](manage-display-and-view-modes.md) of the paragraph.

Once that's done, the last thing is to add this new paragraph as an option when content editors edit the **Speaker content type**.

Go back to the **Speaker** content type's **Manage fields** page.

<figure><img src="../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>

We'll **re-use** another field, this time the **Components** field.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 11.45.22 am.png" alt=""><figcaption></figcaption></figure>

And when configuring the field, scroll down the **Paragraph types** section and check only **Book**. Then select **Save settings**.

This way we can reuse the **existing Components** field, but customise it for this instance to just have the Book type.

Now when you go to add or edit a speaker, the Components field is available with our new Book paragraph.

Select **Add Book** and you can see the fields that we configured inside our **Paragraph** type.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 11.47.56 am.png" alt=""><figcaption></figcaption></figure>

We can add as many books as we need for the speaker, because the components field inside the **Speaker content type** is configured to allow unlimited added components.

{% hint style="info" %}
If you create a standard page that also has the components field, you'll see that Book is NOT available for it. This is because when we added components to the Speaker content type, we only modified the settings on THAT content type, other instances were not altered.
{% endhint %}
