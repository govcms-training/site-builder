# Roles and Permissions

Rather than assigning individual permissions directly to each user, permissions are grouped into **roles**. You can define one or more roles on your site, and then grant permissions to each role.

Each (backend) user account on your site is automatically given the Authenticated user role, and may optionally be assigned one or more additional roles. When you assign a role to a user account, the user will have all the permissions of the role when logged in.

It’s a good practice to create several roles on your site.

GovCMS comes with a number of default roles:

1. Content Author
2. Content Approver
3. Site Builder
4. Site Administrator

## User roles analysis

In the case of our new Government Jobs Portal, our site needs three user roles:

* **Content Author:** These are the agency staff members who will be creating content for the website.
* **Content Approver:** These are the agency staff members who will be approving content for publishing.
* **Site Builder**: This role includes all of the access included in the above two roles but with some elevated permissions such as managing blocks, user accounts, content types, fields and media entities etc.

All of the above roles are available by default in GovCMS SaaS sites and in your training environment. However, the actual permissions can be configured differently on your agency website compared to the training environment.
