# Exercise 6.1: Build the employment news view

In this exercise we’ll build an Employment news page/listing by creating a new view. This view page will list all job posts.

## Create the view using the wizard

1.  Go to **Structure** → **Views** to see the _Views_ admin page - /admin/structure/views.\


    <figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption><p>Add view</p></figcaption></figure>
2.  Click the **Add view** button at the top of the page to access the view creation wizard. To create the Employment news view, enter the below details:

    * **View name**: Employment news.
    * **Description**: “Displays a list of news about Employment on the site.” This allows _Site administrators_ to easily see what the view does.
    * **Show**: _Content_.
    * **of type**: _Job Post_.
    * **sorted by**: _Newest first_.

    These dropdown selections set up the page with the _Job Post_ content displaying, showing the most recent job first.\


    <figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption><p>View settings</p></figcaption></figure>
3.  Next, check the _Create a page_ checkbox to create the new views page. Leave the Page title and Path fields as-is - they should already contain _Employment news_ as the name of our view.

    <figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption><p>Page settings</p></figcaption></figure>
4. In the page display settings area, select:
   * Unformatted list and teasers.
   * Items per page: 10.
   * Use a pager.
   * **Create a menu link** to expand options.
   * **Menu**: Main navigation.
   * Leave default **Link text** as Employment news.
   * Click **Save and edit**.
   * Review your changes.

<figure><img src="../.gitbook/assets/image (22).png" alt=""><figcaption><p>View settings page</p></figcaption></figure>

## Review your changes

After saving the view, navigate to the frontend of the site. Check if the _Employment news_ appears in the main navigation at the top. If the menu does not initially appear in the primary navigation section, it can be due to caching. You can either ask your developer to clear the cache or wait 24hrs for the cache to be automatically cleared.

Click on the new menu to explore any _Employment news_ that you may have published on your site.

<figure><img src="../.gitbook/assets/image (23).png" alt=""><figcaption><p>View results</p></figcaption></figure>

If you only see one Job Post, create additional Job Posts to see how Views takes care of listing them automatically.
