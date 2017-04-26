## Zotonic TinyMCE init for support of inline svg elements

### What it is

The _admin_tinymce_overrides_js.tpl initializes TinyMCE and adds svg
elements as valid to the editor.
Copy the file _admin_tinymce_overrides_js.tpl, or merge with existing,
to your Zotonic site templates directory.

To enable svg sanitization in Zotonic you also have to add
{html_elt_extra, [ <<"svg">> ]},
to you sites config file. (Without trailing "," if it is the last one.)

After this you should be able to paste and save svg elements into the
editor when in source mode.
