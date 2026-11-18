# Block visibility

As previously mentioned, **blocks** are self-contained chunks of your website’s page layout that are placed inside the **regions** of your theme.&#x20;

They have visibility settings that can determine when they display, and can range from static content (like the site logo) to dynamic content (like the main navigation or main page content).

To start, let's find an existing block and look at its configuration and visibility settings.

Go to **Structure** and then **Block Layout**, and select **Configure** on a row associated with a block.

<figure><img src="../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

Depending on which block you select, you will be given different options.

For example, if you select **Configure** on the row associated with **Header site branding - slogan**, you'll see the following configuration options allowing you to configure various aspects of this branding block:

<figure><img src="../.gitbook/assets/Screenshot 2026-07-01 at 4.38.09 pm.png" alt=""><figcaption></figcaption></figure>

Whereas the **Search** block in the **Header middle 3** region only has the following:

<figure><img src="../.gitbook/assets/Screenshot 2026-07-01 at 4.39.02 pm.png" alt=""><figcaption></figcaption></figure>

You can **configure** different blocks to see the different options they have.

### Visibility settings

Each block also has its own available settings that you can configure and change. However, there is also a set of **visibility** settings common to every single block.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-01 at 4.41.34 pm.png" alt=""><figcaption></figcaption></figure>

This section allows you fine-grained control over the configuration of the visibility conditions that must be met for this block to display.

#### Pages

The **most common visibility setting** is what URL (page) the block should appear on. You can configure either an allow list or a deny list based on the radio button.

You can also include a wildcard asterisk to set the block to appear in entire sections of the website.

This is often used for adding blocks to sections of your website. For example, if a business unit has content that lives under the path /about-us (such as /about-us/corporate and /about-us/foi) you could configure a block to appear at **/about-us\*** so that it appears in that region on every page that begins with **/about-us**.

<figure><img src="../.gitbook/assets/image (84).png" alt=""><figcaption></figcaption></figure>

#### Response status

This setting allows you to set your visibility based on the returned response code. For example, if the block should be visible if the page returns a 200, 403 or 404 error.

However, since you can customise your website to redirect to a certain page based on a 403 or 404 error anyway, this is rarely ever used.

<figure><img src="../.gitbook/assets/image (85).png" alt=""><figcaption></figcaption></figure>

#### Roles

This allows you to set the visibility of a block depending on the active user's role. This may be useful to display certain blocks to certain content authors, perhaps providing content authoring hints or business area contacts for certain sections.

For government websites, having public users authenticated with roles is quite rare, so this option is rarely used.

<figure><img src="../.gitbook/assets/image (86).png" alt=""><figcaption></figcaption></figure>

#### Webforms

The webforms visibitliy setting allows you to set the visibility based on if a webform is on the page. However, this is also rarely used as it's often easier and more reliable to embed a webform on a specific page, and then set the visibility of the block using the **pages option** instead.

<figure><img src="../.gitbook/assets/image (87).png" alt=""><figcaption></figcaption></figure>

#### Content type

The **second most useful block visibility setting**, this allows you to configure a block to only appear for certain content types. For example, if you have a block that links to a sign-up form, you can set it to display on all **events** content.

<figure><img src="../.gitbook/assets/image (88).png" alt=""><figcaption></figcaption></figure>

#### Vocabulary

Lets you set your display based on if the user is viewing a specific taxonomy vocabulary, not a specific term inside that vocabulary.

<figure><img src="../.gitbook/assets/image (89).png" alt=""><figcaption></figcaption></figure>

#### Webform

A second webform option with less configuration options.

<figure><img src="../.gitbook/assets/image (92).png" alt=""><figcaption></figcaption></figure>

Next we'll create a new block and add it to some of our pages.
