---
icon: dumbbell
---

# Exercises

After the above lessons you should have learnt:

* About the Views module and how it can be used
* How to create, configure and customise a view
* How to create a list of related content using views
* How to create a list of relational content using views
* How to customise the Administration interface using the pre-existing views
* How Views Data Export works
* How Better Exposed Filters works

### Exercise 1

Create a view with a block output that list all events.

### Exercise 2&#x20;

{% hint style="info" %}
For this exercise you'll need a few speakers and event content pages. Edit each events content and add a speaker.
{% endhint %}

Using the view block you created in Exercise 1, place the view block on speaker pages only and filter the result set so that when viewing a speaker only events related to that speaker are shown.

* Place this view block in a region and force it to be shown on speaker pages only. Go to a speaker's page and verify that you see the block. The block should list all events (even events not related to the current speaker).
* Configure this view by setting up a relationship and contextual filter to only show events related to the current speaker.
* View a speaker and verify that only events with that speaker are shown from your view block.
