# Add and configure fields

### Add and configure fields

By default all content types are empty and we need to **add the fields** we need.

<figure><img src="../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

You can add **new** or **existing** fields, and customise them.

### Reusing an existing field

If you select **Re-use an existing field**, you’ll be able to insert any pre-existing field from other content types.

You should always re-use fields when possible as it lowers database size and prevents double handling when theming the field output.

Finding the balance between what should be a generic, re-used field, and what should be a specific field for your content type is something you gain with experience.

### Create a new field

If no existing field suits your needs, you can create a new one.

For this lesson, select the **Create a new field** button.

This will show you a list of all the currently available field types. The list on your agency's website may vary as some optional modules provide their own field types.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-06 at 4.50.53 pm.png" alt=""><figcaption></figcaption></figure>

In this example, we're going to add a Photo field for our speakers. After checking the reusable fields, I decided this required a new field.

After selecting **Create a new field**, select the **Media** option from the second column.

Every field requires a **Label**. You should note that when creating a field label, it also creates a machine name. While the label can be changed afterwards, the machine name can never be changed, so ensure your spelling is correct before selecting **Continue**.

<figure><img src="../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

You'll then be presented with the various **field options** for this media field.&#x20;

Just like when configuring blocks, there are some generic settings required for all fields, and then some that are unique to your selected field type.

The first section is always **Field storage**.

Field storage allows you to configure how your field will be configured in the database. The options you select here cannot be changed once the field has been used.&#x20;

For all field types you can choose the **Allowed number of values**, which allows you to specify how many items this field can store.&#x20;

If this was a gallery, we could change the value to **Unlimited** and allow our content authors to upload an unlimited number of photos. In this instance, we only need one photo, so let's leave it as **Limited: 1**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-06 at 4.55.52 pm.png" alt=""><figcaption></figcaption></figure>

The other option in field storage for a media field is confirmation that you want to reference media items. For other fields such as text fields this would allow you to configure the maximum length of the field.

Below **Field storage** we have **Help text**. This is an unformatted text area where you can provide help text that will appear below the field for your content authors.&#x20;

{% hint style="info" %}
Content authors are the users that will be using your website the most. It's best practice to make their experience as easy as possible.&#x20;
{% endhint %}

Below **Help text** we can set if the field is **Required** or not. If this checkbox is checked, the user can't create new content without filling in this field.

Underneath the **Required** checkbox is the **Reference type** section.&#x20;

{% hint style="info" icon="image" %}
This specific section is shown for the media field type. Other fields will have different options here.
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2026-07-06 at 5.06.17 pm.png" alt=""><figcaption></figcaption></figure>

Since we want this to be a speaker's photo, we're going to limit this field to **Image**.

Once all your options have been configured, select **Save settings**.

You'll be returned to the **Manage fields** page, showing your newly added field.

<figure><img src="../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

### Re-use an existing field

We also want the speaker's **biography**.  For this we'll need a standard rich text field. While we could create a new field, other content types already have a text field, so we'll re-use that.

Select **Re-use an existing field**, and scroll down the list to find the field named **field\_c\_n\_body** and select **Re-use**.

<figure><img src="../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

The field will be added with the default options that have been used in this field before, however we want to modify them for this instance of the field.

We can change the **Label**, **Help text** and **Allowed text formats** options to suit us.&#x20;

<figure><img src="../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

After making the changes, select **Save settings** and you'll then see this field added to your content type.

<figure><img src="../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

At this point, your content type has been created to a minimum requirement and it can start to be used.

{% hint style="info" %}
Now that we have our basic fields established, create a few test pieces of content and see how your **Speaker content type** looks before we continue.
{% endhint %}

However, there are a few extra configuration settings that you **SHOULD** take into account each time.
