# Search overview

There are two backend search options provided in GovCMS: **Apache Solr** and the default **Drupal Database**. Both of these options are free and are open-source search engines.

### Database or Solr

Your search engine of choice depends on the scope and requirements of your website. For a simple brochure-style website with under 20 pages, low traffic and low content complexity, a simple Database search will work.

This method uses the website's database for search queries. This means it has limited scope and features.

The alternative is to enable **Solr search**. This creates a self-contained, third-party server that your website gets indexed into, which can be used to support additional features such as autocomplete, document indexing, advanced filters and more.

To check your search options, select **Configuration**, **Search and metadata** and **Search API**.

<figure><img src="../.gitbook/assets/image (69).png" alt=""><figcaption></figcaption></figure>

In the screenshot above, we can see the default Database search, as well as the Solr server enabled but not configured.

Each search requires two components, the **Server** and the **Index**.

In the above example we have the Database Server with an index called Content, and a Solr Server with no configured index.

You can configure **multiple indexes**. For example you could have a search index built for the entire website content, and then another built just for publications.

Because the Database search is quite simple, we won't cover it in the training. Instead, we'll focus on the Solr server option.
