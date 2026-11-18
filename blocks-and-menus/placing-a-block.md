# Placing a block

Now that we have created a new block, we can place it in a **region** in our website.

You can place a block via the Block layout screen, by hovering over **Structure** and then selecting **Block Layout**.

First, locate a region to place your block in.&#x20;

In this example we're going to add our block to the bottom of the **Content** region, below the **Main page content** block.

<figure><img src="../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

Scroll down the **Block layout** page until you can see the **Content** region, and then select the **Place block** button beside it.

<figure><img src="../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

Locate the block you want to add, in this case the **Event Call to Action** block, and select Place block associated with the row.

You'll then be asked to configure the visibility options for this block.

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

There are two main ways to display the block on the bottom of each event page.&#x20;

We could either:

* Use the **Pages** section of the visibility settings to show the block on all pages with a URL that begins with /events/\*
* Use the **Content type** section of the visibility settings to show the block on the Event content type

Using either Pages or Content yype are valid approaches, however both approaches also present some edge cases that may cause issues:

* Selecting the **Pages** option means that if an event was given a manual URL alias that didn't use the /events/\* pattern, the block wouldn't be visible for that event
* Selecting the **Content type** approach means that if a content author created a standard _Page_ with the URL alias of  /events/how-to-apply, to inform users how to apply to attend an event, then the block wouldn't display on that page, because we're only displaying it on events.

In this case, let's use the **Content type** option. Additionally we can uncheck the Display title option at the top to hide the title of our block to have it display cleanly.

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

With the configuration options set, select **Save block**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-06 at 1.20.59 pm.png" alt=""><figcaption></figcaption></figure>

In this example our block has been added to the bottom of the list for the **Content region**, however we could use the arrow widget to click and drag to reorder the list, or to move blocks between regions.

If you do make an order change, remember to scroll down and select **Save blocks** at the bottom of the page to save your change, or simply navigate away to discard your change.

With our new **block** added to the **Content** region for all **event** content, we can now open any event and see the block below the page text.

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>
