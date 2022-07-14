# About cross-site scripting

Cross-site scripting \(or XSS\) is a security vulnerability sometimes found in websites. In a site that is not well protected, malicious users can enter script into web pages that are viewed by other users \(for example, in a comment or in the body of a page\). A cross-site scripting vulnerability may be used by attackers to login as another user. It’s important to configure the text formats of your website to prevent such abuse.

The good news is that GovCMS comes with two preconfigured text formats:

1. Rich text \(CKEditor-enabled\)
2. Plain text

![Image of GovCMS text formats](../.gitbook/assets/Unit-5-Xss-1.png)

As a site builder, you can always add your own text formats and configure the roles allowed to use them.

Follow these and other best practices to keep your site safe:

1. The **Rich Text** format is intended for trusted users only \(Content Authors or Administrators\). Even though it has HTML tags filter applied \(see the Allowed HTML Tags in Rich Text format configuration under _Configuration_ → _Content authoring_ → _Text formats and editors_ → **Rich text**\), some sites may request that no restriction is in place and no HTML tag restriction can be in place. 

    {% hint style="danger" %}
    **This can represent a severe security risk.**
    {% endhint %}
    
2. The **Plain text** format is intended for anonymous users, and does have CKEditor enabled.
3. When working with user-generated content, it's always best to keep input format settings as secure as possible. Select the least amount of functionality possible for each role; for example, don't allow anonymous users to have access to **Rich Text** format.

> **Note:** Certain inputs are restricted by default on GovCMS \(such as the tags needed to display video properly\) to protect the system from malicious code. Rich text format should only be accessible by trusted users.

![Image of Comic](../.gitbook/assets/0%20%281%29.png)

Source: [https://xkcd.com/327/](https://xkcd.com/327/)

Comic reproduced under a [Creative Commons Attribution-NonCommercial 2.5 License](http://creativecommons.org/licenses/by-nc/2.5/).

