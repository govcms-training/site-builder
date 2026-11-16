# URL redirects

All content in Drupal is accessed via a URL alias, as covered [earlier when we set up a content type](../designing-and-planning-content/additional-settings-for-content-types.md#pathauto-url-alias), and in the previous lesson when we [configured URL settings](url-aliases.md).

URL aliases are generated automatically for your website, and are the URL that users will see in the address bar.

However, sometimes site visitors may need an alternative URL.

This may be because an incorrect URL was published in print or on another website, or because you want to create a shorter URL for a marketing campaign.

For this, you can create a **URL redirect**.

Redirects can also be used to ensure previously created URL aliases do not return a **404 not found** response if a page is renamed or moved.

Out-of-the-box, GovCMS websites may not handle redirects the way you expect. Let’s take a look.

First we can re-confirm by checking the **URL alias settings** that when a URL alias is updated (for example if a page title is changed or the page moves in the menu structure) that a new alias is created, and the old one is deleted.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-22 at 2.15.19 pm.png" alt=""><figcaption></figcaption></figure>

Without a URL redirect, this would mean that anyone trying to access the page from the old URL would be given a 404 not found error. URL redirects fixes this issue.

Navigate to the **Configuration**, **Search and metadata**, **URL redirects** and then **Settings**.

<figure><img src="../.gitbook/assets/image (67).png" alt=""><figcaption></figcaption></figure>

Here we can see that the **URL Redirect module** will automatically create a redirect when a URL alias is changed.

This ensures that all content retains a single URL alias, but users can still access the content through any legacy URLs.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-22 at 2.33.40 pm.png" alt="" width="563"><figcaption></figcaption></figure>

We covered the [manual creation of URL redirects](https://app.gitbook.com/s/zAp101XNX82HnyCe3C9U/url-aliases-and-redirects/redirects) in the Introduction to Content Management manual.

The settings provide a few other options, however these are mostly left as default.

**Retain query string through redirect** allows you to have redirects for pages with filters on them. Filters often add query strings to the end of the URL, such as ?search=licences and having this setting enabled keeps that included when the user is redirected.

**Default redirect status** allows you to configure the default redirect code when new redirects are created. By default a **301 moved permanently** is the best choice for a default setting. Per-redirect overrides can be selected when they're created.

Under **Global redirect settings** you should enforce clean and canonical URLs as this will automatically redirect to the canonical URL of any page. That includes redirecting to an alias if existing, removing trailing slashes and similar clean-up. This creates a clean user experience.

Ignoring redirections on admin paths and check access should both be disabled. They can cause unexpected behaviours, and the majority of GovCMS websites have a clear distinction between authenticated users and public visitors, so these checks are not required.

{% hint style="info" %}
Please be aware that you cannot use the Redirect module to redirect any **file paths**, only Drupal content paths.

If you want to provide redirects for files, you need to use the redirects-map.conf approach outlined below.
{% endhint %}

### Bulk redirects

Every GovCMS project is provided with a [redirects map configuration file](https://github.com/govCMS/scaffold/blob/develop/redirects-map.conf) that supports the ability to manage bulk redirects as well as dynamic redirects.

```
## Path redirects
##
## This file provide the ability to redirect paths, this will redirect all paths
## to the incomming host.
##
## @see http://nginx.org/en/docs/http/ngx_http_map_module.html
##
## 1. This will match $uri (uri will always be at least '/')
## 2. Destination of the redirect (must always be prefixed with '/')
## 3. Destination supports external hostnames for full redirects

## Redirect old-paths from the host to new paths.
## ~^/old-path/(.*) /new-path/$1;

# Redirect patterns to a new host.
## ~^/old/(.*) http://other-domain.gov.au/$1;
```

Dynamic redirects are handy if you rename an entire section of your website, but the pages themselves remain the same. In this case, you can set up a dynamic redirect so that any visitor trying to access the old section will be automatically redirected to the new section.

Or, as mentioned above, if you need to create a redirect for a specific file URL.

As this can’t be done via the Drupal UI, and can only be actioned by a developer, it’s out of scope for this training. Guides on how to use it can be found in the [GovCMS Knowledge Base](https://www.govcms.support/support/solutions/articles/51000289483-log-in-to-access-the-govcms-knowledge-base).
