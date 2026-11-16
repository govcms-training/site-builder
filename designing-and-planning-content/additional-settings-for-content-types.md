# Additional settings for content types

There are also other settings that should be configured whenever you create a new content type.

### Pathauto (URL alias)

When a new content type is created it isn’t given a URL alias pattern, and any new content will be given the default URL of slash node slash the node ID number.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-13 at 12.20.15 pm.png" alt="" width="563"><figcaption></figcaption></figure>

To fix this, go to **Configuration**, **Search and metadata**, and then **URL aliases**.

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

Then, select **Patterns** from the list at the top.

This will display all the existing URL patterns.

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

If there's a pattern you want to add to your new content type, you can select **Edit** from the dropdown list, select your new content type and select **Save**.

However in this instance we're going to add a new pattern. Start by selecting **Add Pathauto pattern**.

Select the **Pattern type** as Content, and in the list of available **Content types** that are displayed, select our new **Speaker content type**. Finally, add a **Label** for Speaker.

Now that our basic information is complete, we'll tackle the **Path pattern** itself.

This is the URL pattern that all new Speaker content will be given.&#x20;

In this example, we want our URL alias pattern to be /speaker/ followed by the name of the speaker, which we know is held in the Title field of the node.

First, click into the **Path pattern text field**, type in speaker/, and then select the **Browse available tokens** link to view all the available dynamic tokens we can include.

{% hint style="info" %}
Clicking into the text field marks that field as the **active recipient** of any tokens, so that you can click the blue token text in the popup and have it automatically populate into the path pattern field.
{% endhint %}

{% hint style="info" %}
As you may remember from the Introduction to Content Management training, a token is a string in Drupal surrounded by square brackets. It's used as a placeholder in configuration settings and then replaced when used in the website.

For example the token of **\[node:title]** is replaced by the **Title** field data when a node is created.
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2026-07-13 at 12.25.41 pm.png" alt=""><figcaption></figcaption></figure>

If you expand the **Nodes** section by selecting the small arrow beside it, we can see all fields that are available in our content type.

Scroll down the list until you find the row for **Title**. Select the blue text **\[node:title]** and that will be populated into your **path pattern field**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-13 at 12.32.46 pm.png" alt=""><figcaption></figcaption></figure>

Once that is complete, you can close the **Available tokens** popup with the X in the top right corner.

Select **Save** to save this pattern.

Now, when any speaker content is saved, it will use the URL alias of /speaker/ the Title of the node, which is the speaker's name.

{% hint style="info" icon="dumbbell" %}
You can browse the **Available tokens** popup to find all the different variables. For example, you could have a URL alias built from the year the article was published, followed by the number of books they have in their profile, and the file name of the image used in the photo field.

Any data from the node can be exposed as a token and used in a URL pattern.

A popular pattern for pages is **\[node:menu-link:parents:join-path]/\[node:title]** as this takes the menu hierarchy of an item and creates a URL path based on it.&#x20;
{% endhint %}

### Workflow

Now let’s look at configuring workflows for content types.

By default, GovCMS comes configured with a standard **workflow**, which allows content authors to save content in Draft, Needs Review or Published, as well as Archive.

However newly created content types are not added automatically to the pre-existing workflow.

To add it in, simply go to **Configuration** then **Workflow**, then **Workflows**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-13 at 1.00.01 pm.png" alt=""><figcaption></figcaption></figure>

From the workflows screen, click on **Edit** beside the **Editorial workflow**.

Scroll down to the **This workflow applies to** section and click on the **Select** button on the Content types row.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-13 at 1.09.58 pm.png" alt=""><figcaption></figcaption></figure>

In the list of **content types**, click on the checkbox for your new content type and select **Save**. On the workflow screen, scroll down and select **Save** again.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-13 at 1.10.56 pm.png" alt=""><figcaption></figcaption></figure>

Now when content authors create new content of this type, they’ll be given the same content approval workflow as the rest of the website.
