# Taxonomy - Categorising content

Taxonomy is a core Drupal/GovCMS module that gives your website(s) use of the organisational keywords known in other systems as categories, tags, or metadata. It allows you to connect, relate and classify your website’s content. In GovCMS, these terms are gathered within “vocabularies”. The Taxonomy module allows you to create, manage and apply those vocabularies.

Taxonomy should be driven by the business requirements of your website, thinking about possible future functional expansion. Here are some questions to help you determine how you may want to use taxonomy:

* Are there subsections of your site that you’d like to look different from the main theme?
* Are there content areas of your site that should be edited only by a specific part of your organisation?
* Is there content that can be shared across your site (such as a press release, form or fact sheet)?
* Is there a business need to support local sites such as service centres or local events?
* Are there different ‘states’ you need to set (such as left navigation/breadcrumbs) for site sections?
* Do you need to provide default lists of content by taxonomy term or default RSS feeds by term?

Many contributed modules rely on Taxonomy-generating; for example, menus based on existing tags.

You may also like to refer to [https://www.drupal.org/docs/8/core/modules/taxonomy/taxonomy-module-overview](https://www.drupal.org/docs/8/core/modules/taxonomy/taxonomy-module-overview) for more information on taxonomy.

!\[A picture containing screenshot

Description automatically generated]\(../.gitbook/assets/75%20%282%29.png)

### List (text) field versus taxonomy

You can also add a "List (text)" field to a content type. What’s the difference between List (text) and a taxonomy field?

To manage values in the **List (text)** field, a privileged user role (like Site Administrator) is required to alter the site configuration. Taxonomy, on the other hand, could be managed similarly to content by Content Editors.

### Normalise content types with Taxonomy

Taxonomy can be used in a workflow, to customise defined sections of your website with different themes or to display specific content based on taxonomy terms. Although taxonomy can be used in various ways, probably the most important use of taxonomy in GovCMS is to relate content.

#### **Exercise 4.1:** Add new vocabulary

Job seekers want to see content (including available jobs) that relate to a specific state/territory, such as ACT or Victoria. To meet this requirement, all Job Posting content on the site should be categorised by State/Territory. To do this, we’ll create a new vocabulary called ‘State/Territory’ and add terms to it (all of Australia’s states and territories).

In this exercise you’ll create a vocabulary, add terms and reorder the terms.

1. **Create a vocabulary and add terms**
   1. Go to **Structure** →**Taxonomy** and click **Add vocabulary**. Enter in the following information:

* **Name**: State/territory
* **Description**: Australian states/territories
* Click **Save**.

![](<../.gitbook/assets/76 (2).png>)

*
  1. You can now see the new _State/Territory_ vocabulary on the main Taxonomy page (**Structure** → **Taxonomy**). Next you’ll need to add terms to the vocabulary. Click **Add term**.
* Let’s add our first term Navigate to **Structure** → **Taxonomy** → **State/Territory** → Click the **List terms** link in the “Operations” column.
* Click **Add term** button.
* **Name**: ACT
* **Description**: leave empty
* **Relations**: leave all defaults
  1. Click **Save.**

**Enter the rest of terms and re-order**

*
  1. Enter the remaining terms (in this case the remaining states and territories). Each time you save, the form will reload, ready for you to add more terms. Enter the following terms with a short description for each:
* New South Wales
* Victoria
* South Australia
* Western Australia
* Northern Territory
* Queensland
* Tasmania
  1.  Navigate to the **list** of all terms in the vocabulary. By default the list is ordered alphabetically, but you can change the order by dragging the terms up or down. As an exercise, drag “Queensland” to the top of the list. !\[A screenshot of a cell phone

      Description automatically generated]\(../.gitbook/assets/77%20%282%29.png)
  2. Click **Save**.

#### **Exercise 4.2:** Add taxonomy field to content types

As a Site Administrator, I want to ensure all (not only **Job posting**) content has a state/territory value selected. Use your experience from the previous exercises to add the State/Territory field to all content types.

![](<../.gitbook/assets/78 (1).png>)
