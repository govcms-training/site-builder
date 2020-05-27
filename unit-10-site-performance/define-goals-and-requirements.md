# Define Goals and Requirements

Now that you’ve got your baseline results, you can start setting your goals. Based on the problems outlined in your site’s speed test report, you may target different areas of your website, such as:

* Manage website caching - to reduce the **First byte** time and the **Fully loaded** time.
* Review and apply better optimised image styles - to reduce the **Bytes in** size of your pages and reduce the **fully loaded** time.
* Enable CSS and JS files aggregation - to reduce the number of requests.
* Enable browser caching - to reduce the **fully loaded time** and the **bytes in** for consecutive page visits.

To further improve **Document complete**, **Start Render** and **First Interactive** times, code changes may have to be applied to the application. It may require you to move some render-blocking CSS and JS files from the &lt;head&gt; region to the bottom of the page. Such changes are beyond the scope of this training.

Example goals may look like the below:

* Reduce the **fully loaded** time to stay under 4.7s per page
* Reduce the **Bytes in** below 2MB per page
* Minimise the number of requests
* Minimise the **First Byte** time

As you can see, some of the goals are not quantitative. This is because we can’t guarantee some of the metrics. Instead we target a noticeable improvement.

