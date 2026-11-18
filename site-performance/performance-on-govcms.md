# Performance on GovCMS

There are many factors that can affect how performant your website is, and its loading speed is a major factor in user retention.

There are many free and paid external tools that can give you an insight into your website's current performance and often provide suggestions on how to improve its performance.

Keep in mind that some factors are out of your control because they're platform-level settings applied to every GovCMS customer, and can’t be modified.

An external speed optimisation tool like **Webpagetest.org** will highlight any problems and provide some guidance to mitigate or minimise the impact.

![](<../.gitbook/assets/unknown (5).png>)

Another great free tool is **Lighthouse**, which is built into the Chrome browser. If your local IT department hasn’t restricted your permissions, you can **press F12** and select **Lighthouse**.

{% hint style="info" %}
[Page Speed Insights](https://pagespeed.web.dev/) provides the same results, but external scans such as this will be blocked by GovCMS' CDN.
{% endhint %}

![](<../.gitbook/assets/unknown (6).png>)

Choose your settings and select **Analyze page load**.

After the page finishes loading you’ll be presented with an in-depth report about the various performance aspects of your website.

![](<../.gitbook/assets/unknown (7).png>)

Let's look at how to interpret the results of your tests.

The three factors you have the most control over the speed your page loads are:

1. **Page weight**
2. **First contentful paint**
3. **Largest contentful paint**.

**Page weight** relates to the bandwidth required to transmit the contents of the page.

**First contentful paint** marks the time at which the first text or image is painted or displayed on the screen.

The **largest contentful paint** marks the time at which the largest block of text or largest image is painted.

This gives the user some indication that the page is loading and has not frozen.

The **first** and **largest** contentful paint metrics are a combination of server performance and page weight.

The video below explains some of these concepts.

{% embed url="https://www.youtube.com/watch?v=bESOzUyHAZM" %}

Since we have no control over **server performance**, the best improvements can be made by **managing your page weight**.

**Page weight** is very important, as the larger the page is to transmit, the longer it takes to load, which can frustrate your users.

This can also be very impactful for regional or mobile users who may not be using fast internet.

To help decrease you page weight, only **upload images sized for the web** and **avoid using embedded videos**, especially on homepages.

To help reduce your page weight, you can **use image styles** to ensure that despite what images are uploaded, that only correctly sized and optimised images are presented to the users.

However, some images may be baked into your theme. These are often banner or decorative images.

While content authors probably can't edit these, you should ask your developers to use correctly sized and optimised images in your theme.
