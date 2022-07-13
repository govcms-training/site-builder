# Planning for Peformance

You should establish performance goals to ensure you spend effort wisely. These tips will help:

* Measure your site performance to establish a performance baseline
* Define goals and requirements for your site or application
* Review the data you have to find the most important areas to improve
* Define a list of potential improvements, categorise them by effort and impact, and prioritise the improvements that will bring you closer to your goals
* Cautiously build the site and ensure your architecture doesn't impact the performance
* Select the modules carefully to avoid performance issues

#### Establishing a performance baseline

Before attempting performance tuning, establish a performance baseline. Having the baseline will help you to assess how much of an improvement is achieved during and after the optimisation.

Once your website is running publicly, you need to use an external speed optimisation tool like [http://webpagetest.org/](http://webpagetest.org/). Make sure you select the closest test location - for example, consider running your test from a data centre in Sydney.

![](../.gitbook/assets/162.png)

An external performance analysis tool allows the following metrics to be captured:

* First Byte Time
* Document complete time
* Fully loaded time
* Number of requests
* Bytes in

These are the metrics that we can control on the application level.

![](<../.gitbook/assets/163 (1).png>)
