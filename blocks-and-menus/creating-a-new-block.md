# Creating a new block

While some blocks such as **Main page content** and **menu-**&#x62;ased blocks are created automatically as part of Drupal's core functionality, you can also create your own blocks.

Since blocks can be configured to display in a certain region of the website based on visibility rules. They're useful for consistent, repeated content.

For example, automatically adding a block to every event page to provide a link to a newsletter signup, or adding a **Quick exit button** to all pages in a sensitive topic space.

In this example we're going to add a simple call to action on every event page.

To start, hover over **Content** and then **Blocks** and select **Add content block**.

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

Here you can select from various **Block types** that have been created for your website. Block types are editable field entities, similar to content types that we will cover in the next section.

Content types are things like 'Pages' or 'News' constructed using fields, and a user views them at a set URL. Block types are also made of fields, but are placed as structural elements across a website.

For this example let's add a **Component** block type.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-06 at 12.36.04 pm.png" alt="" width="375"><figcaption></figcaption></figure>

This allows us to place a CivicTheme-styled component as a block.

Enter a **Block description** (Block title) and any CivicTheme content component we want, in this case a Promo component.

<figure><img src="../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

Once all fields are filled in, select **Save**. This takes us back to the Block library page and we can see our new block added to the top of the library.

<figure><img src="../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

Now that the block has been created it's saved in the database as a block. However, it's not currently configured to display anywhere.

Next we need to place it in a region.
