# Other performance considerations

Apart from activating system-wide caches, the following performance improvements should be achieved:

1. **Views caching:** The Views module provides internal caching tools, allowing for the reduction of rendering times and improving the performance of your site. When enabling Views caching, make sure that the right caching is activated. We recommend activating the **Tag-based** caching. This will ensure proper cache expiration on content updates. However, on traffic-heavy websites, it may be better to use the **Time-based** caching.

![](../.gitbook/assets/165.png)**Search API Views:** Search API views, like the **Jobs Search** one we built earlier, requires the **Search API (tag-based)** or **Search API (time-based)** caching. Applying non-Search API caching may not work as expected.

**Image Styles:** Images may contribute a significant portion to the total page size. Reducing page size helps speed up page loading times with less bandwidth. This is even more relevant for mobile devices.

As a Site builder, make sure that the right image styles are in place. Avoid using the **Original size** **image** when configuring displays - use the right image styles instead.
