# Views display

Displays are managed using the bar along the top of the view. You can display the view in  different ways, and each can have a slightly varied configuration.

{% hint style="info" %}
Choosing when a view should have a new display with a few tweaks, versus an entire new view is something learned over time.

In this instance, we're making a few minor filtering tweaks, so keeping it as a single view is the best option.
{% endhint %}

The goal of this section is to show how you can create and configure multiple displays for a view.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-15 at 3.08.14 pm.png" alt=""><figcaption></figcaption></figure>

Select the **Add** button in the **Displays** bar and select **Block**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-15 at 3.29.49 pm.png" alt="" width="364"><figcaption></figcaption></figure>

The **Display** bar will now show a **second display mode**, with the active display being given a darker background.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-15 at 3.41.36 pm.png" alt="" width="310"><figcaption></figcaption></figure>

By default, secondary view displays inherit their settings from the primary view display. If you check the **Fields** and **Filters** sections you can see that it's already set up with the same fields and filters from the page.

However, our original view was set up with an exposed filter for the title, which we don't need in this block, so we should remove it.

Scroll down to the **Filter criteria** and select the **Title field**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-16 at 1.19.49 pm.png" alt="" width="375"><figcaption></figcaption></figure>

**BEFORE** you select the Remove button, in the top left change the **For** dropdown from All displays to **This block (override)**.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2026-07-16 at 1.23.23 pm.png" alt="" width="190"><figcaption></figcaption></figure>

With that option selected, when you remove the Title filter, it will only be removed from this display. Select the red **Remove** button to continue.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-16 at 1.23.53 pm.png" alt="" width="375"><figcaption></figcaption></figure>

You'll see now that the **Filter criteria** heading is italicised. This shows that the Filter criteria section has been modified for this particular view. The non-italic headings represent sections that are fully inherited from the original view.

Lastly, let's change the pagination settings.

Under the **Pager** heading, select **Mini**, and change the pager option to **Display a specified number of items.**

Remember to change the **For** option to **This block (override)** so that you only affect this block.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-16 at 1.28.35 pm.png" alt=""><figcaption></figcaption></figure>

Then select **Apply (this display)**.

Change the number of items to display to 3 and select **Apply**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-16 at 1.30.15 pm.png" alt="" width="375"><figcaption></figcaption></figure>

Again, the **Use pager** item is now in italics, which shows it has been overridden for this display.

**Save the view**, and then using the skills from the [Placing a block section](../blocks-and-menus/placing-a-block.md), place this newly created speaker block on the **homepage**.

{% hint style="info" icon="dumbbell" %}
To further clean this up, you could remove the **Header** and **Biography/Short summary** text fields for the block display.
{% endhint %}
