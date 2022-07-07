# Add and configure fields

The Field module \(GovCMS core\) provides the configuration for fields and field attachments; the field types and input widgets themselves are provided by additional modules. Some of the modules are required, and the optional modules can be enabled from the Modules administration page \(Administer → Modules\).

GovCMS core includes the following field type modules: Text \(required\), Number, List, Taxonomy, Image, and File. Additional fields and widgets may be provided by contributed modules.

The Field module allows custom data fields to be attached to GovCMS entities \(content nodes, users, taxonomy vocabularies, etc.\) and takes care of storing, loading, editing, and rendering field data. Most users will not interact with the Field module directly, but will instead use the Field UI module user interface. Module developers can use the Field API to make new entities "fieldable" and allow fields to be attached to their entities.

![Image of Manage fields](../.gitbook/assets/35%20%282%29.png)
