# Roles and permissions

The last core component of functionality for GovCMS is **roles** and **permissions**. This governs what your users can control.

Drupal uses an additive role and permission system that allows you to **stack** the granting of permissions to your users. Drupal only ever allows you to give positive access, you can't assign someone a deny permission, instead you simply assign them nothing.

This allows you to create granular roles and permissions.

For example, you could technically create a role that had all the permissions around editing basic page content, and a role around editing news, and another for events. Then, you could assign all those roles to a single user who can control all that content, and then just the event role to a user who only manages events.

Out-of-the-box, GovCMS has three roles: Content Author, Content Approver and Site Administrator.

{% hint style="info" %}
On your training environment we have created a Site Builder role for the Advanced Content Management training, which provides more than a content author but less than a full Site Administrator.
{% endhint %}

* **Content Authors** can create new content, edit content, and mark content for review by an Approver.
* **Content Approvers** can publish, archive and delete content created by Content Authors.
* **Site Administrators** can delete content, revert content revisions, place content blocks and perform other advanced content and website management tasks.

### Managing users

Managing users is covered in the [Introduction to Content Management training manual](https://app.gitbook.com/s/zAp101XNX82HnyCe3C9U/roles-and-permissions) and the associated training course.
