SearchBar
=========

This FreeCAD mod adds a search bar for tools, document objects and preferences.

⚠️ Several issues related to the C++ memory management interacting badly with Python's have caused lots of segfaults during development. ⚠️

⚠️️ Most of these should now be solved, but save your work often and proceed with caution while testing this extension. ⚠️

Extensibility
-------------

It can be extended by other mods, by adding a new result provider.

Usage
-----

The search bar appars next to the What's this? tool, in FreeCAD's default File toolbar.

![Screenshot of the search bar, with results in its drop-down menu and extra info about the result in a separate pane](screenshot.png)

Development
-----------

* `InitGui.py` adds an instance of `SearchBoxLight` to the GUI.
* `SearchBoxLight` is a hollowed-out implementation of a search box, it loads everything lazily.

License
-------

[![License: CC0 v1.0.](https://img.shields.io/badge/license-CC0-blue.svg)](https://creativecommons.org/publicdomain/zero/1.0/) This repository is in the public domain.
