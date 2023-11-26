# Exercise 5.1 (Optional): Set up the Rich Text editor

In this exercise you’ll learn how to set up the rich text editor.

## Configure the Rich Text editor

1. Make sure you’re logged in as a user with the role that allows editing of text formats.
2.  Go to _Configuration_ → _Content authoring_ → **Text formats and editors**.

    <figure><img src="../.gitbook/assets/image (15).png" alt=""><figcaption><p>Text Format page</p></figcaption></figure>
3. Click the **Configure** link in the Operations column next to _Rich text_.
4. Review the Roles section, which allows you to configure the roles allowed to access Rich text format.
5.  The Toolbar configuration allows you to manage editor buttons/plugins.



    > **As a rule,** give users as few buttons as possible, for as long as possible.

    <figure><img src="../.gitbook/assets/Ex-5-1-Text-Formats-Editors-2.png" alt=""><figcaption></figcaption></figure>
6. The **CKEditor plugin settings** allow you to configure some additional options, such as **Embed Media**.
7.  Check the **Enabled filters** section.



    Note that the **Limit allowed HTML tags and correct faulty HTML** option is selected. It’s important to keep this options enabled for **increased security**.

    If additional HTML tags are required to be supported, update the **Allowed HTML tags** field with the tags that you need. Avoid whitelisting the \<script> tag, since it may introduce a backdoor to malicious scripts.\


    <figure><img src="../.gitbook/assets/image (16).png" alt=""><figcaption><p>Showing test filters</p></figcaption></figure>

    <figure><img src="../.gitbook/assets/image (17).png" alt=""><figcaption><p>Showing allowed html tags</p></figcaption></figure>
8. The **Filter processing order** section allows you to arrange the execution order of filters. Avoid modifying the default order unless necessary.

## Test the editor

Now you can test the editor out by creating a new _Page._\


<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption><p>Body field of Page content</p></figcaption></figure>

1.  Add some text, and then make it bold. Also try adding a list, an image and a link.

    > **Tip:** You can get some sample images at Dynamic Dummy Image Generator: [http://dummyimage.com/](http://dummyimage.com)
2. Click **Save.**
3. See how your page looks. Is the page being displayed as you expected?
