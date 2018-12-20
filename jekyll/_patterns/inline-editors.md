---
layout: page
title: Inline Editors
order: 7
draft: true
---

Inline editors provide in-context text editing capabilities without directing users to a new interface or modal dialog.
Inline editors are largely used in code output where maintaining syntax structure is important.


## Usage

<div class="grid-2" markdown="1">
![inline editor usage](../images/patterns/inline-editors/inline-editor-usage.png)

<div markdown="1">
Inline editors should be provided to users where it is desirable to edit segments of text (typically code) without disrupting the larger document. 
</div>
</div>

## Style

<div class="grid-2" markdown="1">
![inline editor style in dark mode](../images/patterns/inline-editors/inline-editor-style.png)

<div markdown="1">
The inline editor is largely without prescribed style and adopts various properties for text size and height from its parent element. 
When focused it is highlighted by a dotted outline. 

When editing, the text color becomes black and the textarea background becomes white regardless of the syntax highlighting or whether the user is using light or dark mode.
</div>
</div>

## Behavior

<div class="grid-2" markdown="1">
![inline editor behaviour](../images/patterns/inline-editors/inline-editors.gif)

<div markdown="1">
For isolated segments of code or text, where an individual property or value is present (the Rule View pane), the inline editor should be invoked upon a single click on the qualifying text or code.

In areas where a large body of code is present (the Inspector), the inline editor should be invoked by double clicking a qualifying segment of text.  Additionally, the inline editor should be invoked when the user hits enter and a selected segment of editable text has focus.
</div>
</div>


