# Exercise 7.1: URL aliases - Patterns

In this exercise, we’re going to automatically assign a URL alias pattern to the **Job Posting** _content type_ so that all Job posting nodes will be assigned the URL alias format - http://example.com/jobs/\[node:title\]

## Add a new path alias pattern

1. Go to Configuration → Search and metadata → URL aliases → Patterns 

    ![Image of URL alias Patterns](../.gitbook/assets/71%20%282%29.png)

    Our new content type Job posting is not listed yet, so let’s create a new _Pathauto_ _pattern_. 
    
2. Click the **Add Pathauto pattern** button.
3. Select **Content** in the **Pattern type** selector.
4. Select the **Job Posting** checkbox in the **Content type** selector.
5. Enter **Job Posting** in the **Label** field.
6. We need to find out which token to use in the **Path pattern** field so that it automatically takes our **Job posting** title and converts it into a safe URL. To explore available tokens, click the **Browse available tokens** link. In the **Available tokens** pop-up, expand **Nodes** and find **Title** field. Copy the token provided \(\[node:title\]\) and update the **Path pattern** field with **jobs/\[node:title\]**
7. Review the values and **Save** the form.

## Update existing paths

Now that we’ve created the new path alias, we also want to apply this new pattern to existing content, in this case **Job Posting** nodes. To do this, we’ll update all nodes on the site.

1. Click on the **Bulk generate** tab at the top of the **Patterns** admin page.
2. Select **Content** paths
3. Select Generate a URL alias for un-aliased paths only
4. Click **Update**

The new URL alias pattern has now been applied to existing content on your site.

To test it out, create some new **Job Postings** and you’ll see _Pathauto_ automatically adding the new URL alias pattern to the pages when they’re saved.

