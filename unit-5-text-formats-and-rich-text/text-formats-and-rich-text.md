# Text formats and rich text

Site editors need a CMS that’s easy to use so they can input content without HTML knowledge.

Out-of-the-box, GovCMS provides a Rich Text editor \(**CKEditor**\) for writing content.

Rich text editors ensure that content can be added quickly and easily by people who don’t have any HTML experience. Rich text editors give users the ability to add images, create links, make text formatting changes such as bold text, etc.

## About text formats and filters

Text formats change how HTML tags and other text is processed and displayed on your site. Text formats are composed of a series of filters, each of which transforms text. When users create content, a text format is associated with the content, and the full, original text is stored in the database. The content is then passed through the filters in the text format before it’s displayed on the site.

The core **Filter module** provides text format functionality, and the GovCMS installation profile sets up **Rich text** and **Plain text** text formats. Each text format has an associated permission, so that you can allow only trusted users to use permissive text formats. This restricts untrusted users to text formats like **Plain text**, which filters out dangerous HTML tags.

## About the editors associated with text formats

Each text format can be associated with an editor, such as a visual WYSIWYG \(What You See Is What You Get\) HTML editor. The core Text Editor module provides the ability to associate editors with text formats, and to configure the editors \(such as adding and removing buttons from their toolbars\). The core **CKEditor** module provides the industry-standard editor known as CKEditor, so that it can be used to edit HTML content on your site.

