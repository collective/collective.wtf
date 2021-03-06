Changelog
=========

1.0b10 (unreleased)
-------------------

* Moved to github: https://github.com/collective/collective.wtf.
  [maurits]

* Made compatible with Plone 4.1 by loading the permissions.zcml from
  Products.CMFCore (only when plone.app.upgrade is available, to keep
  compatibility with Plone 3).
  [maurits]

* Avoid a deprecation warning for InitializeClass in Zope 2.12.
  [hannosch]


1.0b9
-----

* Don't make assumptions about the csv dialect on import. Instead, sniff the
  first 1024 bytes.
  [mj]

1.0b8
-----

* Avoid creating a ghost workflow_csv folder in the current directory.
  [optilude]

1.0b7
-----

* Add CMF 2.2 / Plone 4 support. Note that the new workflow options (like
  "manager bypass" and "creation guard") are not (yet) supported.
  [optilude]

1.0b6
-----

* Add support for setting the state variable, with the 'State variable' option
  to the main workflow section.
  [optilude]

1.0b5
-----

* Now imports/exports meta_type, in order to support workflows defined with
  collective.reactiveworkflow.  This uses the option 'Type' in the main
  workflow section.
  [optildue]

1.0b5
-----

* Added utility methods to trigger automatic transitions on self and on
  the parent, borrowed from Products.ReactiveWorkflow, but made to be useable
  directly from a script rather than only in an event handler.
  [optilude]

* Improve documentation
  [optilude]

* Add inline script support
  [optilude]

1.0b4
-----

* Add script support
  [elro]

1.0b2
-----

* Add the ability to display roles in any context via a simple browser view
  [optilude]
