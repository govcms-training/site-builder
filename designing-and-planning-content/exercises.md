---
icon: dumbbell
---

# Exercises

After the above lessons you should have learnt:

* What content types are, and how Drupal uses them to organise content
* How to create a new content type using new and reused fields
* How to customise the form display of a content type
* How to customise the public display of a content type
* What paragraphs are and how to create a new one
* How to cross reference content
* What the Minisite module is and how to use it

{% hint style="info" icon="dumbbell" %}
As we'll be using the **Speaker content type** in future examples, please make sure you complete the first two exercises below.

**Tip**: Use Lorem Ipsum to bulk out rich text areas - [https://www.lipsum.com/feed/html](https://www.lipsum.com/feed/html)&#x20;
{% endhint %}

### Exercise 1

Create a new content type with the following configuration:

* Content type called **Speaker**
* Title should be **Name**
* Available to add to the **Primary navigation** menu
* **Biography** field with a rich text editor
* **Photo** where a user can upload a single image
* Customise the Manage display using Field Groups with the following settings:
  * HTML Element field group, labelled **Container**
  * HTML Element field group, labelled **Left column**
  * HTML Element field group, labelled **Right column**

<figure><img src="../.gitbook/assets/Screenshot 2026-07-07 at 4.51.52 pm.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Tip 1**: The names of the field groups require exact spelling to inherit the correct templates created for the Training environment.
{% endhint %}

{% hint style="info" %}
**Tip 2**: The Components field listed above will only be available once you've created the Book paragraph in the next exercise.
{% endhint %}

### Exercise 2

Create a new **Paragraph** type and add it to the **Speaker** content type.

For example, a paragraph that lists the the speaker's accomplishments:

* Create a new paragraph called **Accomplishment**
* Add a **Title** and **Summary** field
* Add it to the **Speaker** content type as a new paragraph type in the existing components field.

### Exercise 3

We'll also need some sample content for future lessons, so create at least 3 speakers.

Consider the relationship between the content editing experience, and the options you selected when configuring the content and paragraph types, as well as the choices made when changing the Manage form display page.
