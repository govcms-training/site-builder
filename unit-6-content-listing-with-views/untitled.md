# Related content by term



Site visitors would like to see content related to a specific state/territory. To do this, we need to set up an automatically generated **list of States/Territories in a block** with the following features:

1. When we click on a term such as “ACT” we go to a term listing page that shows all content tagged or categorised with that term.
2. If we then select a specific article such as “Volunteering” we see the full content page.
3. In the sidebar of the “Volunteering” full node page we also see a “related content” block. This will pull in a list of content that’s been tagged or categorised with the same taxonomy term.

In the following exercises we'll make a “list of terms” block and then we'll make the related content block.

#### **Exercise 6.5:** Make a list of States/Territories block

In this exercise we’ll add a list of the **States and Territories** in the sidebar, so the page looks like the screenshot below.  
 ![A screenshot of a cell phone

Description automatically generated](../.gitbook/assets/31%20%281%29.png)

1. Go to **Structure** → **Views**. Click **+ Add new View**. Add in these settings:

* View name: States/Territories
* Select to enable **Description**: A list of State and Territory terms
* Show _Taxonomy_ terms of type _State/Territory_ sorted by _Unsorted_
* Select Create a block
* Block title: States/Territories
* **Display format**: _HTML list_ of _Fields_
* Items per block: 0
* **Use a pager**: Leave unselected
* Click Save and edit

1. Go to Structure → Block Layout.
2. In the _Sidebar_ area click the **Place block** button.
3. Find **States/Territories** block in **Lists \(Views\)** category and click the **Place block** button.
4. Configure block visibility settings to only display it on the **Job Posting** _content type_.
5. Click Save block.
6. Navigate to a _Job posting_ content page and locate your block.

#### **Exercise 6.6:** Build the related content block

Next we’ll add the related content block, as per the screenshot below.

![](../.gitbook/assets/32%20%281%29.png)

1. **Check content tags**

In the exercise 4.3 we added the **State/Territory** taxonomy reference field to the _Job Posting_ content type.
Make sure you have some content tagged with the _State/Territory_ terms.

2. **Create the View**
2.1. Go to Structure → Views. Click + Add new View. Add in the below information:
2.1.1. View name: Related content
2.1.2. Show “Content” of type “All” sorted by “Title”
![image](https://user-images.githubusercontent.com/2966198/115509489-2a5db100-a287-11eb-8adb-2fe1a57d0132.png)
2.1.3. Select “Create a block”
2.1.4. Leave defaults except for Display format, which should be changed to “HTML list”.
![image](https://user-images.githubusercontent.com/2966198/115509585-482b1600-a287-11eb-832d-8a717add7ef2.png)
3. **Click Save and edit.**
4. **Add dynamic "contextual" filter**

The contextual filter allows us to show a list of the content with the same tags as the current content.
4.1. Add the contextual filter. Click to expand “Advanced” options to the right of the Views screen
4.1.1. Under **CONTEXTUAL FILTERS** click **Add**. This opens a pop-up window.
4.1.2. Search to filter the options for **taxonomy**.
![image](https://user-images.githubusercontent.com/2966198/115509810-8fb1a200-a287-11eb-9d9c-39d7bd4362c8.png)
4.1.3. Select “Has taxonomy term ID
4.1.4. Click Apply and configure contextual filters.
4.2. Configure filter
4.2.1. Under When the filter value is NOT available.
4.2.2. Select "Provide default value", which expands the options.
4.2.3. Under type choose "Taxonomy term ID from URL",  "Load default filter from node page, that's good for related taxonomy blocks" and “Load default filter from term page” as below:
![image](https://user-images.githubusercontent.com/2966198/115509978-d43d3d80-a287-11eb-9f69-87de222fca45.png)
You may also specify the Vocabulary filtering, to limit terms to the **State/Territory** only.
4.2.4. In the “Multiple-value handling” area select "Filter to items that share any terms". This picks up content with one item matching, rather than a 100% match.
![image](https://user-images.githubusercontent.com/2966198/115510086-f8991a00-a287-11eb-9cc4-ec0bfe18f4dd.png)
4.2.5. Scroll down to When the filter value IS available or a default is provided and select “Specify validation criteria”.
4.2.6. Validator: Taxonomy term ID
4.2.7. Vocabularies: State/Territory
![image](https://user-images.githubusercontent.com/2966198/115510207-1bc3c980-a288-11eb-9019-4c29e769961b.png)
4.2.8. Configure “Multiple arguments” as per the screenshot below and select “Reduce duplicates”.
![image](https://user-images.githubusercontent.com/2966198/115510247-28e0b880-a288-11eb-927e-d646c7c52926.png)
4.2.9. Click **Apply (all displays)**
4.2.10. **Save** the view
5. **Place the block**
5.1. Go to **Structure** → **Blocks** and scroll down to the “Sidebar” area
5.2. Click the **Place block** button.
5.3. In the pop-up, filter by text “Related content” in the **Lists \(Views\)** category.
5.4. Place block.
5.5. Under Visibility settings, configure block to display on all pages except the homepage. Remember to use the &lt;front&gt; token as the homepage identified. You may also use “/”. In addition, filter the block to only show on the following content types:
6. **Job Posting**
6.1. Click Save block.
7. **Review and test**

Go to the frontend of your site and check that the Related content block has been added, as in the below screenshot.  
![](../.gitbook/assets/40%20%282%29.png)

Check that you have some content in certain states/territories, so you can see how the block works.
* When you click on a state \(tag\) on a specific article you should see a list of related content, listed by the taxonomy term. You should not see the block.
* You should see the Related Content block when you view a job posting or News and Media article.
8. **Filter out currently displayed page**

While testing the Related content block, did you notice anything unusual?

The **Related content** block displays the article title of the currently displayed page:

![](../.gitbook/assets/41.png)

Let’s remove it by adding one more _Contextual Filter_.

8.1. Return to editing the _Related Content_ view.
8.2. Expand the _Advanced_ pane and you should see the _Contextual Filter_ **Content: Has taxonomy term ID** that we created earlier.
8.3. Add another contextual filter
8.4. Search for ID. ![](../.gitbook/assets/42.png)
8.5. Select _Provide default value_ in the When the filter value is NOT available pane → Content ID from URL. ![](../.gitbook/assets/43%20%281%29.png)
8.6. Under the **More** pane, select **Exclude**
8.7. **Apply** the changes.
8.8. Save the View.
8.9. Test your block from the previous example. Now it shouldn’t display the current page in the block.

