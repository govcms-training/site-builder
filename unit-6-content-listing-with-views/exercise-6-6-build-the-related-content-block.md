# Exercise 6.6: Build the related content block

Next we’ll add the related content block, as per the screenshot below.

![Image of Related content menu](../.gitbook/assets/Ex-6-6-Related-Content-Block.png)

## Check content tags

Make sure you have some _Job posting_ content tagged with the _State/Territory_ terms.

## Create the View

Follow the process outlines in [Exercise 6.5](exercise-6-5-make-a-list-of-states-territories-block.md) to create a new View called **Related content**.

![Image of Related content View](../.gitbook/assets/Ex-6-6-Create-View-1.png)

Your view should look like the following screenshot on the edit View page. Note that the **Advanced** section has been expanded, as it is used in the next steps

![Image of Related content View](../.gitbook/assets/Ex-6-6-Create-View-2.png)

## Add dynamic "contextual" filter

The contextual filter allows us to show a list of the content with the same tags as the current content.

1. Expand the **Advanced items** on the right hand side.
2. Click **Add** next to **Contextual filters**.
3. Search for "Has taxonomy term ID" then select the checkbox.
4.  Click **Add and configure contextual filters**.

    <img src="../.gitbook/assets/Ex-6-6-Add-Contextual-Filter-1.png" alt="Image of Related content View" data-size="original">
5.  Under "When the filter value is NOT available" select the "**Provide a default value"** option.\
    For the Type, select "**Taxonomy term ID from URL**".\
    Also check "**Load default filter from term page**" and "**Load default filter from node page, that's good for related taxonomy blocks**"

    <img src="../.gitbook/assets/Screenshot.png" alt="Image of Related content View" data-size="original">
6. Click **Apply**.
7. Click **Save** on the View page.

## Place the block

1. Go to **Structure** → **Block layout** and scroll down to the “Sidebar” area.
2. Click the **Place block** button.
3.  In the pop-up, filter by text “Related content” in the **Lists (Views)** category.

    <img src="../.gitbook/assets/Ex-6-6-Place-Block-1.png" alt="Image of Related content View" data-size="original">
4. Click **Place block**.
5.  Under Visibility settings, configure block to display on all pages except the homepage. Remember to use the \<front> token as the homepage identified. You may also use “/”. In addition, filter the block to only show on the **Job Posting** content type.

    <img src="../.gitbook/assets/Ex-6-6-Place-Block-2.png" alt="Image of Related content View" data-size="original">
6. Click **Save block**.

## Review and test

Go to the frontend of your site and check that the Related content block has been added, as in the below screenshot.

![Image of Related content menu](../.gitbook/assets/Ex-6-6-Related-Content-Block.png)

Check that you have some content in certain states/territories, so you can see how the block works.

* When you click on a state (tag) on a specific article you should see a list of related content, listed by the taxonomy term. You should not see the block.
* You should see the Related Content block when you view a **Job posting**.

## Filter out currently displayed page

While testing the Related content block, did you notice anything unusual?

The **Related content** block displays the article title of the currently displayed page:

![Image of Related content menu](../.gitbook/assets/Ex-6-6-Related-Content-Block-2.png)

Let’s remove it by adding one more _Contextual Filter_.

1. Return to editing the **Related Content** view.
2. Expand the _Advanced_ pane and you should see the _Contextual Filter_ **Content: Has taxonomy term ID** that we created earlier.
3. Add another contextual filter.
4.  Search for ID (in Category _Content_).

    <img src="../.gitbook/assets/Ex-6-6-Add-Contextual-Filter-3.png" alt="Image of ID content" data-size="original">
5.  Select _Provide default value_ in the **When the filter value is NOT available** pane → **Content ID from URL**.

    <img src="../.gitbook/assets/Ex-6-6-Add-Contextual-Filter-4.png" alt="Image of Provide default value - Content ID from URL" data-size="original">
6. Under the **More** pane, select **Exclude**.
7. **Apply** the changes.
8. **Save** the View.
9. Test your block from the previous example. Now it should not display the current page in the block.

![Image of Related content menu](../.gitbook/assets/Ex-6-6-Related-Content-Block-3.png)
