# URL Redirects

URL Aliases are generally the best URL for site visitors to use. However, sometimes site visitors may need an alternative URL. This may be because an incorrect URL was published in print or on another website or because you want to create a shorter URL for a marketing campaign.

Redirects are also created by GovCMS to make sure only one (usually the latest) URL alias is functional and to ensure previously created URL aliases do not return “404 Not Found” response.

!\[A close up of a logo

Description automatically generated]\(../.gitbook/assets/72.png)\
_Illustration of how Redirects are forwarding all traffic to the latest Alias_

**Tip:** Redirects are generally a better option because extra URL aliases can mean you end up with duplicate content issues, which has a negative impact on SEO.

Out-of-the-box, GovCMS sites may not handle redirects the way your client would expect. Navigate to the **Configuration** → **Search and metadata** → **URL Aliases** → **Settings** and explore how the update action of URL aliases is handled

![](<../.gitbook/assets/73 (1).png>)

In this default configuration the old alias will be deleted. This may not be the best way to handle changes of URL aliases in content.

A better way to handle URL aliases is to create a redirect automatically when an URL alias is getting updated. This will ensure that links to content stay valid whenever the URL alias of a content page is changed.

#### **Exercise 7.2:** Configure redirects

In this exercise we configure automated content redirection when content alias changes.

1. Navigate to the Configuration → Search and metadata → URL Aliases → Settings
2. Scroll down to the **Update action** section
3. Select the option Create a new alias. Leave the existing alias functioning
4. Save configuration
5. Test it out. Navigate to a Standard page of your choice – go to _Content_
6. Note the page URL alias – you’ll need it in the next step

Change the page title and publish the page.\
This should change the URL alias of the page

Confirm that the URL alias of your page changed.

Manually enter the previous URL alias – from step 6

Confirm the page redirected to the latest URL alias – as noted in the step 8.

#### **Exercise 7.3:** Breadcrumbs

Now that we’ve added a custom URL alias and all job postings inherit the common URL pattern, let’s link our breadcrumb to the URL alias and explore how we can improve the user interface by manipulating breadcrumb links.

In Unit 6 we created a View Job Posting and added a link to the top Main Navigation menu (Exercise 6.2).

![](<../.gitbook/assets/74 (2).png>)

The _Breadcrumb_ link **Job Posting** was added by GovCMS for you.

At the moment, when we access any of the **Job Posting** content, the _breadcrumb_ does not show the link to the **Job Postings** page. This creates a UX problem as site visitors don’t have a visual guide of the site section they’re currently in:

![](../.gitbook/assets/75.png)

We want to change the breadcrumbs so that when a **Job Posting** page is displayed, the _breadcrumb_ shows the link to the parent **Jobs** page:\
![](<../.gitbook/assets/159 (1).png>)

The _breadcrumb_ links are constructed from the URL of the current page and checking if the sub-path matches any page on the site. If it does, the system pulls the title of that page and creates a breadcrumb link.

Our parent page (**Jobs**) URL is **/job-postings** and our **Job Posting** _content_ URL pattern is **/jobs/\[node:title]**. To get the **Jobs** page link added to the _breadcrumb_, all we have to do is to change its URL from /job-postings to /jobs. This way it will natively flow into the existing URL pattern for Job Posting content type and the link will be automatically generated in the breadcrumb.

1. Navigate to the **Structure** → **Views** and edit our _Job Posting_ view.
2. Locate _Path_ under _Page Settings_ (middle top section)
3. Edit the _Path_, change it to **/jobs**.
4. **Save** the view
5. Test the _breadcrumb_ by navigating to any _Job Posting_ content. You should now get the **Job Posting** link in the breadcrumb. ![](<../.gitbook/assets/159 (2).png>)
