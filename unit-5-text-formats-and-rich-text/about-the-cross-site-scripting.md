# About cross-site scripting

Cross-site scripting (or XSS) is a security vulnerability typically found in websites. In a site that is not well protected, malicious users can enter script into web pages that are viewed by other users (for example, in a comment or in the body of a page). A cross-site scripting vulnerability may be used by attackers to login as another user. It’s important to configure the text formats of your website to prevent such abuse.

The good news is that GovCMS8 comes with two preconfigured text formats:

1. Rich text (CKEditor-enabled)
2. Plain text

As a site builder, you can always add your own text formats and configure the roles allowed to use them.

Follow these and other best practices to keep your site safe:

1. The **Rich Text** format is intended for trusted users only (Content Authors or Administrators). Even though it has HTML tags filter applied (see the Allowed HTML Tags in Rich Text format configuration under Configuration  Content authoring  Text formats and editors  Rich text), some sites may request you that no restriction is in place and no HTML tag restriction can be in place. **This can represent a severe security risk.**
2. The **Plain text** format is intended for anonymous users, and does have CKEditor enabled.
3. When working with user-generated content, it's always best to keep input format settings as secure as possible. Select the least amount of functionality possible for each role; for example, don't allow anonymous users to have access to **Rich Text** format.

![](<../.gitbook/assets/0 (1).png>)

Source: [https://xkcd.com/327/](https://xkcd.com/327/)

Comic reproduced under a [Creative Commons Attribution-NonCommercial 2.5 License](http://creativecommons.org/licenses/by-nc/2.5/).

![](../.gitbook/assets/1.png)

**Note:** Certain inputs are restricted by default on GovCMS8 (such as the tags needed to display video properly) to protect the system from malicious code. Rich text format should only be accessible by trusted users.

#### **Exercise 5.1 (optional):** Set up the Rich Text editor

In this exercise you’ll learn how to set up the rich text editor.

1. Configure the Rich Text editor
   1. Make sure you’re logged in as an administrator.
   2. Go to Configuration → Content authoring → Text formats and editors ![](../.gitbook/assets/2.png)
   3. Click the **Configure** link in the Operations column
   4. Review the Roles section, which allows you to configure the roles allowed to access Rich text format
   5. The Toolbar configuration allows you to manage editor buttons/plugins. ![](<../.gitbook/assets/3 (1).png>) **As a rule,** give users as few buttons as possible, for as long as possible.
   6. The **CKEditor plugin settings** allow you to configure some additional options, such as **Linkit** plugin and **Image uploads**
   7. Check the **Enabled filters** section. Note that the “Limit allowed HTML tags and correct faulty HTML” option is selected. It’s important to keep this option enabled for increased security. If additional HTML tags are required to be supported, update the **Allowed HTML tags** field with the tags that you need. Avoid whitelisting the \<script> tag, since it may introduce a backdoor to malicious scripts.
   8. The **Filter processing order** section allows you to arrange the execution order of filters. Avoid modifying the default order unless necessary.
2. **Test the editor** Now you can test the editor out by creating a new _Standard page_, making sure the input format is set to _Rich text_. ![](<../.gitbook/assets/4 (2).png>)
   1. Toggle between the _Plain text_ input field and _Rich text_ by selecting Plain text in the Text format selector ![](<../.gitbook/assets/5 (1).png>)
   2. Add some text, and then make it bold. Also try adding a list, an image and a link.

**Tip:** You can get some sample images at Dynamic Dummy Image Generator: http://dummyimage.com/

*
  1. Click **Save.** See how your page looks. Is the page being displayed as you expected?

#### **Challenge exercise 5.2:** Create a new text format

In this exercise, we want to set up a new text format that allows trusted editors to input iFrames. This will let trusted users embed widgets and videos from popular sites.

Your new text format should have these properties:

* Only available to Content Authors and Site Administrators
* Allow a variety of regular HTML tags
* Allow a video from YouTube
