# Exercise 7.3: Breadcrumbs

Now that we’ve added a custom URL alias and all job postings inherit the common URL pattern, let’s link our breadcrumb to the URL alias and explore how we can improve the user interface by manipulating breadcrumb links.

In Unit 6 we created a View called _Job Posting_ and added a link to the top Main Navigation menu ([Exercise 6.2](broken-reference)).

![Image of Job posting View](../.gitbook/assets/Ex-7-3-Breadcrumbs-1.png)

The _Breadcrumb_ link **Job Postings** was added by GovCMS for you.

At the moment, when we access any of the **Job Posting** content, the _breadcrumb_ does not show the link to the **Job Postings** page. This creates a UX problem as site visitors don’t have a visual guide of the site section they’re currently in:

![Image of Breadcrumb to Home](../.gitbook/assets/Ex-7-3-Breadcrumbs-2.png)

We want to change the breadcrumbs so that when a **Job Posting** page is displayed, the _breadcrumb_ shows the link to the parent **Jobs** page:

![Image of Breadcrumb to Jobs page](../.gitbook/assets/Ex-7-3-Breadcrumbs-3.png)

The _Breadcrumb_ links are constructed from the URL of the current page and checking if the sub-path matches any page on the site. If it does, the system pulls the title of that page and creates a breadcrumb link.

Our parent page (**Jobs**) URL is **/job-postings** and our **Job Posting** _content_ URL pattern is **/jobs/\[node:title]**. To get the **Jobs** page link added to the _breadcrumb_, all we have to do is to change its URL from /job-postings to /jobs. This way it will natively flow into the existing URL pattern for Job Posting content type and the link will be automatically generated in the breadcrumb.

1. Navigate to the **Structure** → **Views** and edit our _Job Postings_ view.
2.  Locate _Path_ under _Page Settings_ (middle top section).



    <figure><img src="../.gitbook/assets/Ex-7-3-Breadcrumbs-4.png" alt=""><figcaption></figcaption></figure>
3. Edit the _Path_, change it to **/jobs**.
4. **Save** the view
5. Test the _breadcrumb_ by navigating to any _Job Posting_ content. You should now get the **Job Posting** link in the breadcrumb.

![Image of Breadcrumb to Jobs page](../.gitbook/assets/Ex-7-3-Breadcrumbs-5.png)
