# Manage Media

Media is a drop-in replacement for the Drupal core upload field with a unified User Interface where editors and administrators can upload, manage, and reuse files and multimedia assets. 

The core **Media** module provides a 'base' entity for media assets. This allows you to standardise the way your GovCMS site interacts with media resources. Local files or images, YouTube videos, Tweets, Instagram or Facebook posts, etc. can all be treated in a common way, regardless of where the media resource itself is ultimately stored. Being a standard content entity, you can reference and use this new entity in any place GovCMS knows how to work with them.

Just like with Content types, with this new entity type you can create **Media Types**, add fields to them, manage display modes \(for view and form operations\), and so on.

## Creating and configuring Media Types

If you’ve worked with **nodes** before, you will find some similarities in the basic concepts when dealing with **media entities**. For example, **Media Types** are the equivalent to **media entities** the way **Content Types** are to **nodes**. In other words, the media entity \(just like any other content entity in Drupal 8\) has **Media Types**.

These Media Types are available in GovCMS out-of-the-box for you:

1. File
2. Image
3. Audio file \(local\)
4. Video file \(local\)
5. Remote video

They are ready to use, and if you want to directly create a Media entity you can go to /media/add/{type\_name} and see how the media entity form looks.

One important difference of media entities when compared to nodes is that _not all media types are equal_. They are specialised so that they are able to know how to manage the media resource they’re dealing with in the best way. For example, media types that deal with _images_ will be able to validate file extensions, as well as know how to map width/height image information to Drupal fields. On the other hand, this knowledge won't be necessary or useful to _youtube_ media entities, which in turn will probably need to know how to retrieve a thumbnail or the video author information from the remote video server.

Throughout this training we’ll rely on the default media types. 

> (i) If you need to create new media types, follow instructions from this documentation page: [Creating and configuring Media Types](https://www.drupal.org/docs/8/core/modules/media/creating-and-configuring-media-types).

