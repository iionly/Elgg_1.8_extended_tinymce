Elgg Extended Tinymce plugin for Elgg 1.8
Latest Version: 4.1.10
Released: 2015-05-15
Contact: iionly@gmx.de
License: GNU General Public License version 2
Copyright: (c) iionly 2012-2015, (C) Curverider 2008-2015

The TinyMCE editor is licensed under
GNU Lesser General Public License version 2.1
(c) 2003-2014 Moxiecode Systems AB.
Website: http://www.tinymce.com/



An extended tinymce plugin based on version 4.1.10 of the TinyMCE editor for Elgg 1.8.

For backward compatibility with version 3 of the editor the folder mod/extended_tinymce/vendor/tinymce/jscripts/tiny_mce/plugins/emotions/img contains the emoticons images at the location where they were available before.



Instructions:

1. If you have a previous version of the Extended Tinymce plugin installed, disable it and then remove the extended_tinymce from your mod directory before copying the new version on the server,

2. Copy/extract the extended_tinymce archive into the mod folder,

3. Disable the Elgg core tinymce plugin,

4. Enable the Extended Tinymce plugin.



Creating your own custom skin:

IMPORTANT: Tinymce uses a z-index of 100 for its fullscreen mode. This conflicts with the z-index values used by Elgg (e.g. Topbar). To get it fully working you need to adjust the z-index of ".mce-fullscreen" to 9001 within the files skin.min.css and skin.ie7.min.css of your customized skin.

1. Configure your custom skin at http://skin.tinymce.com/ and download it,

2. Copy your skin folder into the mod/extended_tinymce/vendor/tinymce/js/tinymce/skins directory,

3. Change the skin name of the skin option in mod/extended_tinymce/views/default/js/extended_tinymce.php to the name of your skin.



Adding a language for the tinymce editor (not to be mixed up with adding an Elgg language file for the plugin):

1. Download the language pack from http://www.tinymce.com/i18n/index.ph,

2. Extract the language files from the zip file,

3. Copy the language files into the mod/extended_tinymce/vendor/tinymce/js/tinymce/langs/ directory,

4. Flush the Elgg caches via the admin dashboard on your site.
