# Views - Part 2

## Views displays – multiple views in one

Views allows you to reuse existing configuration in a good way. If you create a page listing of your content and need to provide a block of page titles or add an RSS feed \(even create more pages\) – View Displays can be used rather than duplicating views.

![Image of Page Display and Block content views displays](../.gitbook/assets/13%20%281%29.png)

If you explore the existing GovCMS Block Article View – three Displays exist: Page, Feed and Block.

![Image of GovCMS Block Article View](../.gitbook/assets/14.png)

Views displays allows you to easily create a duplicate of any other display and add some customisations and overrides.

## Views caching

Views also allow you to speed up your site if you have two views that load similar fields. This is because with Views you can cache both the query and rendered output, which reduces the load on your database. You can learn more about Views caching in Unit 10.

## Views attachments

The Views module includes some pre-built templates, which can be activated and edited to suit your requirements.

![Image of Views pre-built templates](../.gitbook/assets/15.png)![Image of Views pre-built templates](../.gitbook/assets/16%20%281%29.png)

## The Views editing interface – Format pane

In this section we’re going to look at the Views editing interface.

![Image of Views editing interface](../.gitbook/assets/17.png)

- **A. Displays**: Create multiple displays from the same view. This might mean multiple pages with different filters or blocks, RSS feeds, etc.
- **B. Format**: Output content into lists, tables, or show the full content \(node\) display.
- **C. Fields**: Specify fields such as title, date, taxonomy, etc.
- **D. Filter criteria**: This is the most important aspect, since you limit the selection this way.
- **E. Sort criteria:** Specify ordering of the list - by created date, by title or any other property.
- **F. Header**: Add arbitrary HTML to the top and bottom of your views.
- **G. Pager**: Specify how many items to display or whether or not to show a "previous/next" pager.


## Related content with Views \(contextual filters\)

In the Unit 6 exercises, we used filters in Views to limit the data displayed \(e.g. to show certain content types or show content categorised with a specific taxonomy term. For our Jobs website, we want to show related content when we view a job listing for a specific state/territory, without having to build a new view for each new state. The solution is to use **context** to control the items displayed. We can set up GovCMS to check the taxonomy terms from the article, and dynamically include content that’s categorised with the same term.

We can configure a view so that it’s filtered dynamically, depending on the context. For example, we could use a contextual filter to add a block that contains related content or that presents a list of articles by the same author.
