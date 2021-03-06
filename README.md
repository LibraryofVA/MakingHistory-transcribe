Making History: Transcribe
=====================

Transcribe is built upon the open-source generosity of George Mason University's [Center for History and New Media](http://chnm.gmu.edu/) and was an original creation by the amazing staff at [The University of Iowa Libraries](http://www.lib.uiowa.edu/). Their project, DIYHistory|transcribe, can be found at [http://diyhistory.lib.uiowa.edu/](http://diyhistory.lib.uiowa.edu/) with their github repository located at [github.com/ui-libraries](https://github.com/ui-libraries). The Library of Virginia made changes to UI-Libraries solution all of which can be found within one of the two following github repositories: [plugin-Scripto](https://github.com/LibraryofVA/plugin-Scripto) and [Scribe](https://github.com/LibraryofVA/omeka-themes/tree/master/scribe). The Library of Virginia has also deployed a self built [Omeka Export plugin](https://github.com/LibraryofVA/plugin-Export) that retrieves the transcription text from Omeka in a format ready to be imported into our digital asset management system.

Overview
--------
[Making History - Trnscribe](http://www.virginiamemory.com/transcribe/) is a tool for engaging users in transcribing handwritten documents, making them more searchable and enhancing them for research. Transcribe is built on the [Omeka](http://omeka.org/) content management system and uses the [Scripto](http://scripto.org/) plugin to facilitate transcription. [Scripto](http://scripto.org/) uses [MediaWiki](http://www.mediawiki.org/wiki/MediaWiki), which allows users to continually improve upon work that has already been done. UI-Libraries made significant additions to the Scripto plugin, created a new Omeka theme, and customized other Omeka plugins to style and scale for a library production environment. A pervious version of the Library's project can be found at [Making History: Transcribe 2.0](https://github.com/LibraryofVA/MakingHistory-transcribe-2.0).

Requirements
------------
Transcribe requires the following:

+ [Omeka version 1.5](http://omeka.org/codex/Version_History)
+ [Omeka Dublin Core Extended plugin version 1.1](http://omeka.org/add-ons/plugins/dublin-core-extended/)
+ ui-libraries/plugin-CsvImport, a fork of Omeka's CsvImport that allows bulk upload of item and file-level metadata
+ We began with [ui-libraries/plugin-Scripto](https://github.com/ui-libraries/plugin-Scripto), a fork of CHNM's Scripto tool for crowd sourced transcription of documents. The Library of Virginia altered UI-Libraries plugin is available at [https://github.com/LibraryofVA/plugin-Scripto](https://github.com/LibraryofVA/plugin-Scripto).
  + Scripto requires a [MediaWiki](http://www.mediawiki.org/wiki/MediaWiki) installation.
+ [Scribe](https://github.com/ui-libraries/Scribe), a custom Omeka theme designed by UI-Libraries for use with ui-libraries/plugin-Scripto. The Library of Virginia's altered version is available at [https://github.com/LibraryofVA/omeka-themes/tree/master/scribe](https://github.com/LibraryofVA/omeka-themes/tree/master/scribe).

Features
--------
[UI-Libraries](http://www.lib.uiowa.edu/) introduced the following features to plugin-Scripto:

- Track completion status of document pages (i.e., 'Not Started', 'Needs Review', 'Completed')
- Track completion progress of documents based on page statuses.
- Sort documents within their collection by most completed, floating least completed to the top.
- Initialize document page text entry box with pre-existing text, if available (helpful if using Scripto to correct OCR for typescript pages).
- On every page action, automatically import transcriptions from MediaWiki as file metadata.


The [Scribe](https://github.com/ui-libraries/Scribe) theme directs its focus on guiding users to easy transcription tasks rather than collection management features, offering a clean, thumbnail-oriented transcription view for any number of Omeka image collections.

By default, any member of the public is allowed to edit and save transcription data, but only users with an account can track their progress. Approved account holders can also be granted administrator (or deputy) status, allowing them to finalize documents as "complete".

Installation
------------
Follow the documentation at each source code repository to install 

For best results, install the ui-libraries/plugin-Scripto plugin and create a collection before installing the Scribe theme.
