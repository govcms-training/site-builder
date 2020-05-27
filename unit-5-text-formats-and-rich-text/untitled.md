# Text formats

Some notes on text formats:

* The filters in the text format setting are applied sequentially, with the output of each filter being passed onto the next filter.
* Text formats should be assigned by role. Anonymous users should only have access to plain text input format, whereas trusted users can have access to _Rich text_ privileges so they can add links, images, and so on.
* The HTML filter only allows the following tags by default:

&lt;a href hreflang&gt; &lt;em&gt; &lt;strong&gt; &lt;cite&gt; &lt;blockquote cite&gt; &lt;code&gt; &lt;ul type&gt; &lt;ol start type&gt; &lt;li&gt; &lt;dl&gt; &lt;dt&gt; &lt;dd&gt; &lt;h2 id&gt; &lt;h3 id&gt; &lt;h4 id&gt; &lt;h5 id&gt; &lt;h6 id&gt; &lt;img src alt data-entity-type data-entity-uuid&gt; &lt;u&gt; &lt;s&gt; &lt;sup&gt; &lt;sub&gt; &lt;table&gt; &lt;caption&gt; &lt;tbody&gt; &lt;thead&gt; &lt;tfoot&gt; &lt;th&gt; &lt;td&gt; &lt;tr&gt; &lt;p&gt; &lt;drupal-entity data-entity-type data-entity-uuid data-entity-embed-display data-entity-embed-display-settings data-align data-caption data-embed-button&gt;

* The site administrator can add or remove HTML tags from this list in the **Filter settings** section from **Configuration** → **Content authoring** → **Text formats and editors** → **Rich text**.

A more detailed explanation of Input Formats and Filters can be found here: [https://www.drupal.org/docs/user\_guide/en/structure-text-format-config.html](https://www.drupal.org/docs/user_guide/en/structure-text-format-config.html)

