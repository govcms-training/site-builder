# Menus and site navigation

Menus are a collection of links primarily used to navigate around a website.

The core **Menu UI module** provides an interface to control and customise the menu system. Menus are usually displayed as a hierarchical list of links.

The GovCMS installation profile contains five default menus:

* **Administration**, which contains administrative task links
* **Footer** for basic site information links
* **Main navigation**, which is usually used for your main site content
* **Tools**, which is primarily used by modules to provide useful tool links
* And **user account** menu, for links related to the active user account.

However, Administrators can easily create new menu containers. You may want a new menu for a number of reasons, such as:

* A standalone menu per business area in your website
* A reusable related links menu to place on your website
* Multiple footer menus for ease of layout.

To begin, hover over **Structure** and then select **Menus**.

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

Here we can see a list of all of the menus currently in the website, and we can also add a new menu by selecting the **Add menu** button at the top of the page.

After selecting the button, type a name for your new menu in the **Title** field. The **Administrative summary** is optional and only displayed on the Menu administration landing page.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-06 at 2.33.48 pm.png" alt="" width="375"><figcaption></figcaption></figure>

Select **Save** to create the new menu.

You'll be presented with a new empty menu.

<figure><img src="../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

Now that you’ve created the custom menu, you need to add in some links. You can do this in one of two ways:

1. By manually adding link items via the menu interface
2. By adding links to the menu when you edit specific content pages or sections.

{% hint style="info" %}
[Adding Menu link via the Add link button](https://app.gitbook.com/s/zAp101XNX82HnyCe3C9U/menus-and-navigation/using-the-menu-screen) is covered in the Introduction to Content Management guide.
{% endhint %}

So instead of adding links directly with the button, let's add this new menu as an option when a content editor is editing content.

Go to **Structure** and then **Content types**.

<figure><img src="../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

Find the content type you want to add to your **menu** to, then select the dropdown arrow and select **Edit**.

Scroll down and you will see the **Configuration tabs** (we'll cover all of these more in the next section).

Select **Menu** settings and check the box beside the menus you want this content type to be able to be added to.

<figure><img src="../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

Select **Save**.

Now, when you create or edit content of that content type, in the **Menu settings** area on the right you can select the new menu from the **Parent link** dropdown list.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-06 at 2.57.54 pm.png" alt="" width="375"><figcaption></figcaption></figure>

### How to display a menu

When a menu is created, Drupal automatically creates a block for it, thus it can be placed anywhere a block can be placed.

We covered [how to place blocks](../functional-overview/blocks-in-govcms.md) in our previous section.

However menus have a few additional settings you can configure.

In addition to the standard block configuration options such as visibility and region, menu blocks also allow you to configure how the menu itself will appear.

In the below example we've gone back to the **Block layout** page, scrolled down to the **sidebar top left region**, selected **Place block** and scrolled down in the list to the menus. Our newly created Important links menu is there automatically. &#x20;

Selecting **Place block** will embed this menu in the sidebar region.

<figure><img src="../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

This will present you with the **Configure block** popup for your new block.

There will be three collapsed accordion of options that are unique to all menu blocks:

* Menu levels
* Advanced options
* HTML and style options.

#### Menu levels

<figure><img src="../.gitbook/assets/Screenshot 2026-07-06 at 3.03.06 pm.png" alt=""><figcaption></figcaption></figure>

To start, we can expand the **Menu levels** accordion and see the following options.

*   **Initial visibility level**. This allows you to toggle the visibility of the menu depending on the current page's position in that menu.\
    If you select a visibility of one, then all menu items will always be visible, however if you select a level of three, then this menu will only be visible when you're viewing pages that are at or below your menu's third level, and will not be visible when on higher level pages.<br>

    <figure><img src="../.gitbook/assets/Screenshot 2026-09-14 at 12.35.18 pm.png" alt="" width="375"><figcaption></figcaption></figure>
* **Number of levels to display**. This option allows you to configure how many levels deep the menu will display items. If you have a very heavily structured menu, with many levels, you may need to lower this from Unlimited to create a usable menu.
* **Expand all menu links**. Enabling this will ensure that all menu child items are included in the menu, even when you're viewing content in a different section of the site. This is often useful for [Mega menus](https://www.navbar.gallery/blog/what-is-a-mega-menu).

The best way to understand how these options work is to create a menu with multiple levels of content, embed a menu block, and then configure the menu with different options and navigate around the pages to see how it actually behaves.

#### Advanced options

**Advanced options** allows you to configure some additional display options.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-06 at 3.17.41 pm.png" alt=""><figcaption></figcaption></figure>

* **Fixed parent item**. This allows you to set which item in the menu should act as the root-level parent item. This can be handy if you're creating multiple blocks for the one menu, but want different options depending on the top level item.
* **Use as title**. If your block title is set to display, you can dynamically change it based on what item in the menu is being viewed.
* **Hide on pages not included in menu**. As it says, will hide the block (including the title) from the user if the page they're viewing is not included in the menu at all.
* **Make the initial visibility level follow the active menu item**. If the page the user is viewing is deeper than the initial visibility level set in the menu levels section, the initial visibility level will be relative to the active menu item. Otherwise, the initial visibility level of the tree will remain fixed.
* **Display empty block**. This is only useful if your CSS or JavaScript requires a specific number of elements in your HTML to target correctly.

#### HTML and style options

Finally the **HTML and style options** section allows you to define a specific HTML template file name to be used for this menu.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-06 at 3.18.02 pm.png" alt=""><figcaption></figcaption></figure>
