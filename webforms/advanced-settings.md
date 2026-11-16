# Advanced settings

Most of the advanced settings for webforms are covered in the Introduction to Content Management training manual, such as:

* [List of all components](https://app.gitbook.com/s/zAp101XNX82HnyCe3C9U/webforms/basic-components)
* [Conditional fields](https://app.gitbook.com/s/zAp101XNX82HnyCe3C9U/webforms/advanced-features)
* [Form settings](https://app.gitbook.com/s/zAp101XNX82HnyCe3C9U/webforms/advanced-features)
* [Viewing and downloading submissions](https://app.gitbook.com/s/zAp101XNX82HnyCe3C9U/webforms/viewing-submissions)

In this section, we'll go over the **Advanced** and **Access** tabs for fields and set up a webform email handler.

Each field has a list of tabs containing configuration options.

<figure><img src="../.gitbook/assets/image (97).png" alt=""><figcaption></figcaption></figure>

**General** contains basic setting such as field name, default value and if the field is required.

**Conditions** allows you to set field conditionals to hide/show the field based on previous inputs.

### Advanced

The **Advanced** tab lets you control the various field wrapper and HTML elements used in the webform.

<figure><img src="../.gitbook/assets/govcms11-training.docker.amazee.io_admin_structure_webform_manage_civictheme_feedback (1) (1).png" alt="" width="375"><figcaption></figcaption></figure>

While you can set placeholder text in the **General** tab, you can **set a default value** to be provided on submission.

**Wrapper**, **Element** and **Label attributes** allow you to configure additional CSS classes and HTML attributes to your form elements. However, because the training website uses CivicTheme, which has extensive template overrides, these changes may not be rendered on the Training environment.

**Submission display** is only used to override how the value is displayed when viewing the submission as an Administrator via the UI. As most records are downloaded or viewed via email, this is rarely used.

**Administration** allows you to add additional context for this field that's only visible to administrative users.

### Access

<figure><img src="../.gitbook/assets/image (98).png" alt="" width="375"><figcaption></figcaption></figure>

The **Access** tab lets you configure access to the field based on user level or permission. However, since most GovCMS websites only allow for authenticated users for content management, this area is unlikely to be used.

### Sending a webform via email

Sending an email when a webform is submitted is a very common practice. It can be used to either send the contents of the form to a business area inside your agency, a confirmation to the submitter themselves, or both.

To configure a webform to send an email upon submission, first edit the webform, then go to **Settings,** **Emails / Handlers**, and select **Add email**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-28 at 2.13.41 pm.png" alt=""><figcaption></figcaption></figure>

**General settings** contain a title and notes field. This is only displayed on the emails/handlers page, however your title field should describe who the email is being sent to.

**Send to** allows you to select the email address that the submission should be sent to. By default, the email will be send to your website's primary email address, which is usually **\<project name>.noreply@govcms.gov.au**.

You can use the dropdown to change to **Custom To email address** if you want to send an email to a static email address, such as an internal business area. Alternatively, it could be a suitable value from the form itself for a confirmation message to the user.

{% hint style="info" %}
When selecting the To address of a value from the form, ensure it's of the field type Email, as that field will validate that the text entered is a valid email address. If you use a standard text field (like in the example below) there is no validation, and a user could enter an invalid email address, and then not recieve the confirmation email.
{% endhint %}

<figure><img src="../.gitbook/assets/Screenshot 2026-07-28 at 2.17.24 pm.png" alt="" width="375"><figcaption></figcaption></figure>

You can also configure any **CC** or **BCC** email addresses.

**Send from** allows you to configure what **from email** and **from name** should be used to send your submissions.

By default, this should send from your website's no-reply email address unless your developers and IT department have configured a different email server.

**Reply-to** can also be set if you want people to be able to reply to your public emails.

The **Message** area allows you to configure the body of the email that will be sent, including the subject line.

By default, the **Body** contains a standard template that includes replacement tokens for the date it was **submitted**, the **user** who created it (which will always be anonymous for public, non-logged-in users) and then a list of field labels and **values** from the user.

This can be customised by changing from **Default** to **Custom body**, or **Twig template**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-28 at 2.38.26 pm.png" alt="" width="375"><figcaption></figcaption></figure>

If you decide to use the \[webform\_submission:values] catch-all token, you can still customise it to not include some values by expanding the **Included email values/markup** accordion and then unchecking items.

In the example below, the markup element won't be included in the email.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-28 at 2.49.12 pm.png" alt="" width="563"><figcaption></figcaption></figure>

In the example below, we've selected **Custom body** and customised the value to only include the created **timestamp** and the value provided in the **first\_text\_field** field.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-28 at 2.45.32 pm.png" alt="" width="563"><figcaption></figcaption></figure>

After making changes, make sure you select **Save** at the bottom of the Add email handler **sidebar**.

### Conditional emails

By default, **all email handlers will fire** when a webform submission is saved. However, you can set the handlers to be **conditional,** based on user field selections.

For example, the user could have a checkbox they need to check for the system to send them a confirmation.

In that case, you could create conditional logic that only enables the handler if the **Send confirmation field** is checked.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-28 at 2.53.24 pm.png" alt="" width="563"><figcaption></figcaption></figure>

Or you might have a contact us form where the user can **select the business area** the email should be sent to. You can then create an email handler with a **custom To email** address, and conditional logic that only enables that handler if a **specific value is selected**.

<figure><img src="../.gitbook/assets/Screenshot 2026-07-28 at 2.56.01 pm.png" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot 2026-07-28 at 2.55.41 pm.png" alt="" width="563"><figcaption></figcaption></figure>
