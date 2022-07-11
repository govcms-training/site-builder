# Exercise 6.6: Build the related content block

Next we’ll add the related content block, as per the screenshot below.

![Image of Related content menu](<../.gitbook/assets/115 (1).png>)

## Check content tags

Make sure you have some content tagged with the _State/Territory_ terms.

**Create the View**

**Click Save and edit.**

## Add dynamic "contextual" filter

The contextual filter allows us to show a list of the content with the same tags as the current content.

## Place the block

1. Go to **Structure** → **Blocks** and scroll down to the “Sidebar” area.
2. Click the **Place block** button.
3. In the pop-up, filter by text “Related content” in the **Lists (Views)** category.
4. Place block.
5. Under Visibility settings, configure block to display on all pages except the homepage. Remember to use the \<front> token as the homepage identified. You may also use “/”. In addition, filter the block to only show on the following content types:

* **Job Posting**

1. Click Save block.

## Review and test

Go to the frontend of your site and check that the Related content block has been added, as in the below screenshot.

![Image of Related content menu](<../.gitbook/assets/115 (1) (3).png>)

Check that you have some content in certain states/territories, so you can see how the block works.

* When you click on a state (tag) on a specific article you should see a list of related content, listed by the taxonomy term. You should not see the block.
* You should see the Related Content block when you view a job posting or News and Media article.

## Filter out currently displayed page

While testing the Related content block, did you notice anything unusual?

The **Related content** block displays the article title of the currently displayed page:

![Image of Current page in menu lust](../.gitbook/assets/41.png)

Let’s remove it by adding one more _Contextual Filter_.

1. Return to editing the _Related Content_ view.
2. Expand the _Advanced_ pane and you should see the _Contextual Filter_ **Content: Has taxonomy term ID** that we created earlier.
3. Add another contextual filter
4.  Search for ID.

    <img src="../.gitbook/assets/42.png" alt="Image of ID content" data-size="original">
5.  Select _Provide default value_ in the When the filter value is NOT available pane → Content ID from URL.

    <img src="../.gitbook/assets/43 (1).png" alt="Image of Provide default value - Content ID from URL" data-size="original">
6. Under the **More** pane, select **Exclude**
7. **Apply** the changes.
8. Save the View.
9. Test your block from the previous example. Now it shouldn’t display the current page in the block.
