# Exercise 3: Assign the related links menu block to a region

When you create a new menu, GovCMS automatically creates a menu block for the menu. Now we need to assign this menu block with an area on the website.

Go to Structure → Block layout \(/admin/structure/block\)

Find the Postscript 2 area and click the Place block button

Filter the list - Related Links. Select Menus block “Related Links” → Place block

Click Save block

Now check your site to make sure the Related Links menu block is in the Footer

Next, we’ll restrict visibility so it doesn’t show throughout the site

#### **Exercise 1.9:** Configure the related links menu block

The last step is to configure the new menu block.

1. Go to _Structure_ → _Block layout_ and find the **Related Links** block. Click **Configure**.
2. Configure the **Title.** We’ll leave it at the default, but this is where you can:

* Enter a new title
* Unselect the **Display title** checkbox to remove the block title

1. In the _Visibility settings_ you’ll notice three options:

* **Pages** - display the block on specific pages
* **Content Types** – display the block alongside specific content types
* **Roles** – display the block to specific roles

You’ll often need to alter a block’s _Pages visibility_ settings_._ For this exercise, we want the **Related Links** menu to appear _only_ on the _About us_ page we created earlier, and the _homepage_ of our site.

1. Under **Pages** → **Show for the listed pages**, enter the URL paths of the pages that we want to display the block, e.g. /about-us-0
2. On a new line in the **Pages** _text area_, enter _&lt;front&gt;_. This will ensure your Related Links menu block is displayed on the front \(home\) page of your site.
3. Click Save block.

![](../.gitbook/assets/23%20%282%29.png)

The **Related Links** menu will only be displayed on the front and About us pages.

