Jinja2 based templates for Roundup Issue Tracker
================================================

Roundup Issue Tracker is a great lightweight and customizable tool,
especially suitable for a help desk or personal tracker. Today, seamless
interaction with the tracker also requires support for mobile devices.

This is a generic issue tracker based on classic schema. It uses Jinja2 for
templating and Twitter Bootstrap for responsive markup. You will need `jinja`
and `gettext` for this to work.

These templates are based on the code distributed in the official Roundup
repository, but have a number of significant differences.

Dependency updates
------------------

* Twitter Bootstrap has been updated to version 5.3.2.
* No custom stylesheets are used, just pure Bootstrap.
* Removed jQuery and used vanilla JavaScript instead.
* [SimpleMDE](https://github.com/sparksuite/simplemde-markdown-editor/) markdown
  editor has been replaced with
  [EasyMDE](https://github.com/Ionaru/easy-markdown-editor).
* Added Bootstrap Icons 1.11.2 used for some form buttons.
* Added PopperJS 2.11.8 as a Bootstrap dependency.

UX/UI changes
-------------

* The layout has been significantly reworked and is now fully responsive.
* All table views except context history have been replaced with responsive
  grids.
* Duplicate links have been removed from navigation and menus.
* Navigation has been completely redesigned and placed on the sticky navbar.
* Keywords are now added to the issue index by default and can be used for quick
  filtering.
* The issue index now displays more detailed information, such as the number of
  messages and files.
* Added tooltips for real names, detailed times and some other things.
* When displaying a username, a profile link is now also added.
* Search and sort forms have been redesigned to make them more user-friendly.
* Added types for some search form fields to avoid entering invalid values.
* Forms are now disabled if the user does not have permission to change values.
* Attachments now allow multiple files to be uploaded.
* Global file list and issues now use different templates to display files.
* User list and file list can now also be downloaded in CSV format.
* Generated pages now use HTML5 semantic tags and heading hierarchy.
* Added support for Bootstrap dark theme and theme switching.

Restrictions
------------

Internationalization is only partially supported because translations of some
strings need to be added to the Roundup code. Most of the strings from the
original templates have been retained, but some have been changed or added.

Please note that there are no plans to port this to Zope TAL or another engine.

Installation
------------

Install an instance of Roundup and replace the tracker home directory with the
contents of this repository. If you have a production instance, you can only
replace the `html` and `static` directories.

Contributing
------------

If you would like to contribute to the project:

* Open pull request with improvements
* Discuss ideas in issues
* Spread the word
* Reach out with any feedback

License
-------

Distributed under the MIT License. See `LICENSE.txt` for more information.

Contact
-------

Anton Savchuk <mailto:a.savchuk@gmx.com>
