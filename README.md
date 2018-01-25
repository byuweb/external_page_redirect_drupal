# external_page_redirect
Drupal 7 theme to create pages that are content but redirect immediately to external links.


INTRODUCTION
----------------
This is especially useful for menu links that should be featured and displayed among
other internal content, but need to link to an external source.


INSTALLATION
-----------------
Git clone or download this module. Enable this module.

Under Structure > Content Types you will see a new content type 'External Link'.

This content type will allow you to define a title, summary or description,
and url path for a link. This results in actual content existing on your site,
so that it can be listed among internal content on your website, while still redirecting
automatically to the external url you provide.

This module relies on Field Redirection
https://www.drupal.org/project/field_redirection

TO USE
------------------

You will see the content type has been created.

1. Add a field of type link. You only need to worry about the url, not link title.


2. Follow Instructions for creating the link and display settings as the Field Redirection module states:
https://www.drupal.org/project/field_redirection

(Coming Soon: We will try to finish the module so you don't have to do these steps in the future.)

* Go to the "Manage Display" tab on the settings page for the entity of choice (user, content type, etc) settings page; for example, to work with the content type "redirect_user", go to the URL: http://example.com/admin/structure/types/manage/redirect_user/display (where "example.com" is your site's hostname).
* Expand the "Custom display settings" fieldset and ensure the "Full content" checkbox is checked.
* Click the "Save" button.
* Go to the "Full Content" tab.
* Ensure that all of the fields are hidden except for the field you wish to use.
* Click the selector in the Format column of the field in question.
* Select the HTTP status code to use for the redirect - see below, though 301 is usually the best option.
* Click the "Save" button.
* Ensure that other display modes do not use the redirect.
