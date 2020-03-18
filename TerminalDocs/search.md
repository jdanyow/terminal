---
title: Windows Terminal Search
description: Learn how to search in the Windows Terminal.
author: cinnamon-msft
ms.author: cinnamon
ms.date: 05/19/2020
ms.topic: how-to
ms.service: terminal
---

# How to search in Windows Terminal

The Windows Terminal comes with a search feature that allows you to look through the text buffer for a specific keyword. This is useful when looking for a command you had run before or for a specific file name.

## Using search

By default, you can open the search dialog by typing `Ctrl+Shift+F`. Once opened, you can type the keyword you're looking for into the text box and hit `Enter`.

![Windows Terminal search screenshot](./images/search.png)

### Directional search

The Terminal will default to searching from the bottom to the top of the text buffer. You can change the search direction by selecting one of the arrows in the search dialog.

![Windows Terminal directional search screenshot](./images/search-direction.gif)

### Case match search

If you'd like to narrow down your search results, you can add case matching as an option in your search. You can enable case matching by selecting the case match button, and the results that appear will only match the keyword entered with its specific letter casing.

![Windows Terminal case matching search screenshot](./images/search-case-match.gif)

## Searching within panes

The search dialog works with panes as well. When focused on a pane, you can open the search dialog and it will appear on the right side of that pane. Then, whatever keyword you search for, the results will only be found within that pane.

![Windows Terminal panes search screenshot](./images/search-panes.gif)

You can open the search dialog with any key binding you feel comfortable with. This can be done by adding a key binding in your profiles.json file that uses the `find` command. By default, this command is bound to `Ctrl+Shift+F`. The below key binding will bind `find` to `Ctrl+F`, so when typing `Ctrl+F`, the search dialog will open.

`{"command": "find", "keys": "Ctrl+F"}`