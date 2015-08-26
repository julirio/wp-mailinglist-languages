# WordPress Newsletter plugin languages

The language files of the <a href="http://tribulant.com/plugins/view/1/wordpress-newsletter-plugin">WordPress Newsletter plugin</a> are separately distributed.
There are two reasons for this:

1. To reduce the size of the plugin which needs to be installed/uploaded
2. To allow you to host the languages in an external folder to prevent it from being overwritten.

## How to obtain the language files

You can obtain the language files from Github at: https://github.com/tribulant/wp-mailinglist-languages
This folder contains all the .PO and .MO files with the current, available languages.

Only the .MO files are actually used by WordPress. 
The .PO files are the source, which can be opened with an application such as poEdit: http://www.poedit.net

## How to use the language files

Follow these steps to use the language file(s) you want:

1. Pick the .MO files from Github for the languages that you want to use. For example "wp-mailinglist-de_DE.mo"
2. Go to "wp-content/plugins/" in your WordPress installation and create a "wp-mailinglist-languages" folder there.
3. Upload the "wp-mailinglist-de_DE.mo" file to "wp-content/plugins/languages/" folder you created.
4. If needed, rename the file to match your textdomain. If you are using the lite version, rename it to "newsletters-lite-de_DE.mo" for example.
5. Go to Newsletters > Configuration > System > WordPress Related in the plugin and tick/check "Yes, load external language file" for the "Load External Language" setting.
6. Ensure that you have the <code>WPLANG</code> constant set in your <code>wp-config.php</code> file accordingly eg. de_DE

Please note, if you don't tick/check that setting in #4 above, the plugin will look inside "wp-content/plugins/wp-mailinglist/languages/" for a language file.

That's it, the German - de_DE (in this example) language file will now be loaded if the locale is de_DE.
In the same manner, you can add more .MO files to that "wp-content/plugins/wp-mailinglist-languages/" folder accordingly.

## How to update the language files

Follow these steps to update language files:

1. Open the "wp-mailinglist-languages" folder distributed with the plugin.
2. Pick the .PO file for the language that you want to update for example "wp-mailinglist-es_ES.po" which is Spanish/Espanol.
3. Open the .PO file in an application like poEdit: http://www.poedit.net
4. Check the settings of the catalog in the application so it scans the correct paths, etc... and run a scan/update on the .PO file.
5. Translate/update strings as needed and then save the .PO file. It will automatically generate a new .MO file which can be used with the plugin and WordPress

For any questions or problems, please contact us: http://tribulant.com/support/

## Languages

Thank you for these wonderful people who contributed in translating the plugin:

* Afrikaans (af_ZA) by Tribulant Software
* German (de_DE) by Peter Schonmann and <a href="http://zerspanungstechnik.de">Daniel Minder</a>
* Greek (el_GR) by <a href="http://www.aio.gr">Harris Karanikolas | AiO Systems Information</a>
* Spanish (es_ES) by Juan Llamosas
* French (fr_FR) by Kim Gjerstad
* Hungarian (hu_HU) by <a href="http://www.idsign.hu">iD Sign | Gergely Almasi</a>
* Italian (it_IT) by Johnny
* Lithuanian (lt_LT) by Tomas
* Dutch (nl_NL) by <a href="http://www.webzenz.nl">Ronald de Caluwe | WebZenz</a>
* Brazilian Portuguese (pt_BR) by Vitor Argos
* Portuguese (pt_PT) by wordpress.mowster.net
* Romanian (ro_RO) by <a href="http://richardconsulting.ro">Richard Vencu</a>
* Swedish (sv_SE) by Tomas Lindhoff
* Turkish (tr_TR) by Sersah Namoglu
