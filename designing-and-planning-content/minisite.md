# Minisite

The [Drupal Minisite](https://www.drupal.org/project/minisite) module allows you to upload an archive with a 'minisite' and serve it from a Drupal page, while maintaining the minisite's look and feel.

Essentially, you create a page, upload a ZIP file, and Drupal then extracts that ZIP file and serves the contents from the node's URL alias.

{% hint style="warning" %}
Please note, this module does not actually import the minisite pages as Drupal nodes.
{% endhint %}

### The archive file structure

The file structure of the zip file archive that you upload is very strict; it requires a single folder, which contains at a minimum an index.html file at the root:

```
/minisite
  - index.html
```

In the example below, the minisite archive file also includes CSS, JS and a SVG logo in a subdirectory.

{% file src="../.gitbook/assets/minisite (1).zip" %}

If you try to upload a ZIP archive that is not in the correct format, you'l receive an error message.

When configuring the **Minisite field** you can define which files are allowed in the zip archive. By default it includes:

```
html, htm, js, css, png, jpg, gif, svg, pdf, docx, ppt, pptx, xls, xlsx, tif, xml, txt, woff, woff2, ttf, eot, ico
```

{% hint style="info" %}
While this list can be customised, you can't add any files that are disallowed at the platform level. An article on what file types are blocked can be found in the [GovCMS Knowledge Base](https://www.govcms.gov.au/news-events/news/knowledge-base).
{% endhint %}

### How to add a minisite

As the minisite basically takes over a node, it needs its **own** content type, and is not usually added as just another field to an existing content type.

So, [following the same steps as before](creating-a-content-type.md) we will:

1. Go to **Structure**, **Content types**
2. Select **Add content type**
3. Enter the name of **Minisite**
4. Set our content type settings to our preferences
5. Be redirected to the **Manage fields** page
6. Select the **Create a new field button** and select the **Minisite** field type

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 12.18.21 pm.png" alt="" width="352"><figcaption></figcaption></figure>

7. Add a label and select the **Minisite** field variant and select **Continue**

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 12.19.14 pm.png" alt=""><figcaption></figcaption></figure>

8. The upload destination will remain as **Public files**, as we want this visible to public users
9. Scroll down and you'll be presented with the unique field options for the minisite.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 12.20.22 pm.png" alt="" width="563"><figcaption></figcaption></figure>

The only non-self-explanatory field is the **Allowed file extensions list**, which as mentioned above is the list of file types that are allowed inside the archive file.

When your settings are complete, select **Save**.

Now we can test how the **Minisite module** works by creating a new minisite node. Go to **Content**, **Add content**, **Minisite**.

Add a **Title**, upload the above example archive into the **Minisite** field.

<figure><img src="../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

In the above example we've also checked the **Use URL alias** checkbox, and we're providing a manual URL alias in the node properties.

{% hint style="info" %}
This **Minisite content type** is just like any other content type, so you can define a URL alias pattern for it to use.
{% endhint %}

As the descriptive text suggests, checking the box will display the Minisite using the URL alias, in this case it would be:

```
/minisite/minisite/index.html
```

Leaving the checkbox unchecked will instead serve the minisite from the files directory where the archive is uploaded:

```
/sites/default/files/minisite/upload/minisite/index.html
```
