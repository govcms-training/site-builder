# Exercise 8.7: Set up profile fields

Previously, you added fields to content types. You can also add fields to user profiles. This means you can let users share information about themselves and then you can display it. You can also control permissions so only trusted users can see profiles. Below you can see the profiles will have a text field for description and also a list of interests and a profile picture.

![Image of User profile with image](../.gitbook/assets/213.png)

## Add a text field for a biography

1. Go to Configuration People → Account settings → Manage fields.
2. This interface is similar to the one for adding fields to content, now you can Add a new field with the following settings:
3. **Type:** Text -> Text (plain, long).
4. **Label:** About me.
5. Machine Name: field\_about\_me.
6. **Widget:** Select _Text area (multiple rows)_ (configurable later from the _Manage form display_ tab).
7. Review the User settings. We will keep all the default settings, however, review the options before you save.
8. Click Save settings.

## Add a taxonomy field for interests

We need to create a new “Interests” vocabulary we can use in this case.

1. Go to Structure → Taxonomy → Add vocabulary
2. Name: Interests
3. Save the vocabulary
4. At this stage we may not add any terms to the vocabulary and rely on users adding them via profile
5. If you moved away after the step 1, go to Configuration → People → Account settings → Manage fields
6. Add Field: Reference -> Taxonomy term:

* **Label**: Interests
* Allowed number of values: Unlimited
* Create referenced entities if they don't already exist: Yes
* **Vocabulary**: Interests
* **Widget:** Select _Autocomplete (Tags style)._ This could be configured after you add the field, from the _Manage form display_ tab.
* **Save** settings.

## Test by editing your account

Return to the front page.

1.  Click **Your username** in the top administration menu, then _View profile_, then the **Edit** tab.

    <img src="../.gitbook/assets/214.png" alt="Image of Edit profile buttton" data-size="original">
2. At the bottom of the form you can see the options available.
3. Fill in some text for **About me** and type in tags (comma-separated for multiple tags) for **Interests**, such as _Brazil, sailing, dancing._
4. Under **Picture**, upload an image if you haven't already.
5. Save.

Click the **View** tab and now you can view the admin profile. Try looking at it in another browser (if available) to see it without the administrative options.

You can also manage the display of the fields, for example hiding the label. As your Drupal skills improve, you can make changes to the site design through _Theming_ to alter the way this information looks; or change what displays through _Manage display_ configuration pages.
