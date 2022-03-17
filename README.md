# excelGeneration
#Credit for the core table export code concept goes to insin (met on Freenode in #javascript) and core code inspired from https://gist.github.com/insin/1031969



This plugin is a hack on a hack. The .xls extension is the only way [some versions] of excel will even open it, and you will get a warning about the contents which can be ignored. The plugin was developed against Chrome and other have contributed code that should allow it to work in Firefox and Safari, but inconsistently since it's a hack that's not well supported anywhere but Chrome. I would not use this in public production personally and it was developed for an Intranet application where users are on Chrome and had known versions of Excel installed and the users were educated about the warning. These users also save-as in Excel so that when the files are distributed, the end-users don't get the warning message.

Using the plugin
-------------------
Script:
-------

<script src="https://github.com/rnkNandhu/excelGeneration.js"></script>

------------------------------

using Method:
----------------

$("#yourHtmTable").excelGeneration({
    exclude: ".excludeThisClass",
    name: "Worksheet Name",
    filename: "SomeFile.xls", // do include extension
    preserveColors: false // set to true if you want background colors and font colors preserved
});
-------------------------------------------------------------------------------------
