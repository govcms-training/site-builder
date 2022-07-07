# Exercise 6.1: Build the “Employment News” view

In this exercise we’ll build an Employment news page/listing by creating a new view. The screenshot below shows what the employment news page will look like after we’ve created the new Employment news view.

![Image of Employment news view](../.gitbook/assets/8.png)

## Create the view using the wizard

1. Go to **Structure** → **Views** to see the _Views_ admin page - /admin/structure/views.
2. Click the **Add view** button at the top of the page to access the view creation wizard. To create the Employment news view, enter the below details:
3. **View name**: Employment news.
4. Select **Description** and type: “Displays a list of news about Employment on the site.” This allows _Site administrators_ to easily see what the view does.
5. To show _News and Media_ content follow the steps below:
6. Show _Content_ _**of type**_ _News and Media_ sorted by _Newest first_. These dropdown selections set up the page with the news and media content displaying, showing the most recent article first.

    ![Image of View settings](../.gitbook/assets/9%20%281%29.png)

7. Next, check the _Create a page_ checkbox to create the new views page. Leave the Page title and Path fields as-is - they should already contain _Employment news_ as the name of our view.
8. In the page display settings area, select:
 * Unformatted list and teasers
 * Items per page: 10
 * Use a pager
 * **Create a menu link** to expand options
 * **Menu**: Main navigation
 * Leave default **Link text** as Employment news
 * Click Save.
 * Click Edit and review your changes.

![Image of Page settings](../.gitbook/assets/10%20%281%29.png)
 
## Review your changes

After saving the view, navigate to the frontend of the site. Check if the _Employment news_ appears in the main navigation at the top. Click it to explore any _Employment news_ that you may have published on your site.

![Image of Employment news frontend](../.gitbook/assets/12%20%281%29.png)

If you only see one article, create additional employment news articles to see how Views takes care of listing them.
