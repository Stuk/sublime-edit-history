Edit History
============

Edit history stores a history of edits in every file. These edit points can then be navigated between.

"Rules"
-------

* A new edit location is only created if it is greater than 5 lines away from the previous saved edit location.
* Like in a browser, when you go back to a point and then create a new edit location all the "future" locations are cleared.

Commands
--------

Edit history provides two commands: `previous_edit` and `next_edit`

Keybindings
-----------

No default keybindings are provided as I couldn't find defaults that I liked that didn't override existing ones. I suggest `super+[` on Mac and `ctrl+[` on Linux and Windows. This overrides unindent and indent, but I use Tab and Shift+Tab for this functionality. You can add the following to your User Keybindings:

Mac

```
  { "keys": ["super+["], "command": "previous_edit" },
  { "keys": ["super+]"], "command": "next_edit" }
```

Linux/Windows

```
  { "keys": ["ctrl+["], "command": "previous_edit" },
  { "keys": ["ctrl+]"], "command": "next_edit" }
```

Context Menu
------------

Edit History adds "Back" and "Forward" entries to the context/right-click menu.