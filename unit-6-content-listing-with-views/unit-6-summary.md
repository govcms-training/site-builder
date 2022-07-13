# Unit 6 Summary

This unit gave us an insight into how the Views module works and how you can use it to customise your website. Views is a great way to build complex queries into your database administration. Later in the course we will see other ways to make the most of Views.

#### Always use a caching strategy with Views

You can use caching with Views to save the results of a query for the next site visitor. All views can have a _Tag based_ or _Time based_ cache. If all views are set up with a cache of at least fifteen minutes or more it will reduce the load on the database. _Tag based_ cache is the default configuration and is suitable for most caching scenarios.

**Note:** Very short times in the _Time based_ caching may negatively impact your website performance.

![](<../.gitbook/assets/67 (1).png>)

You can change it to a _Time based_ cache in the right-hand column. Choose a setting based on how often your site is updated.\
![](<../.gitbook/assets/68 (2).png>)

#### Turn off the Views UI module

When you're not developing Views directly you should disable the UI. This will reduce the load on your server’s memory, but Views will still work.

##
