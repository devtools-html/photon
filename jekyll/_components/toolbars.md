---
layout: page
title: Toolbars
order: 11
draft: true
---

Toolbars group buttons and controls together in a horizontal line spanning the width of a panel they have control over. Toolbars are typically located at the top of a panel, the controls they house change the state or perform actions on the content of their panel parent.

## Usage

<div class="grid-2" markdown="1">
![Toolbar example](../images/components/toolbars/toolbars-usage.png)

<div markdown="1">
A toolbar should be utilised when a series of grouped buttons or controls specific to a panel should appear high in the content hierarchy. A good example would be to house a series of filter controls which changes the global state or content of a panel, as seen in the Network Panel sub-toolbar.
</div>
</div>


## Types

### Main toolbar

<div class="grid-2" markdown="1">
![Main DevTools Toolbar](../images/components/toolbars/toolbars-main.png)

<div markdown="1">
The main “toolbox” toolbar which spans the width of Developer Tools Window.
</div>
</div>

### Sub-toolbar

<div class="grid-2" markdown="1">
![Subtoolbar example](../images/components/toolbars/toolbars-subtoolbar.png)

<div markdown="1">
Subheader toolbars are specific to individual panels, a good example is the Network Panel toolbar which houses filter tools and viewing options, tools specific to the Network Panel.
</div>
</div>


## Structure

Toolbars are used as containers for other elements, as such their structure can vary greatly. There are however some common patterns which should be acknowledged for improved consistency among existing implementations.

### Control grouping

<div class="grid-2" markdown="1">
![Button grouping example](../images/components/toolbars/toolbars-buttongroup.png)

<div markdown="1">
Buttons or controls which provide primary functions should be grouped and left aligned within the toolbar. 
Controls which provide secondary or ancillary functionality should be grouped and right aligned within the toolbar.

This pattern is observed in the Main toolbar, the Console and the Debugger Breakpoint toolbar.
</div>
</div>



### Search and filter input

<div class="grid-2" markdown="1">
![Toolbar with filter input field](../images/components/toolbars/toolbars-input.png)

<div markdown="1">
The placement of a search or filter input can vary within a toolbar depending on its perceived priority. As a rule of thumb, the more objective critical an input field is to a panel, the more it should appear toward the left of the toolbar. 

Input fields which provide more ancillary functionality should appear right aligned.
</div>
</div>

### Close button.

<div class="grid-2" markdown="1">
![Main toolbar close button](../images/components/toolbars/toolbars-closebutton.png)

<div markdown="1">
Remaining consistent with well established patterns, the button used to close a panel should be represented by a cross “X” [icon](https://design.firefox.com/icons/viewer/) and appear as the rightmost button in the toolbar.
</div>
</div>



### Clear and delete functions

<div class="grid-2" markdown="1">
![Toolbar with clear button](../images/components/toolbars/toolbars-clear.png)

<div markdown="1">
If the toolbar is to contain a control which clears the content of a panel (typically a list of entries), the control should be a button represented by the “classic steel bin” [icon](https://design.firefox.com/icons/viewer/) and should appear as the leftmost button in the toolbar.
</div>
</div>



## Styles

### Toolbar Button Color

<!-- == tabs start == -->
<div class="grid-2" markdown="1">
![Toolbar button styles](../images/components/toolbars/toolbars-style-buttons.png)

<div markdown="1">


<div data-tabs>
  <input type="radio" name="toolbar-style-color" id="toolbar-lightmode" checked="checked">
  <label for="toolbar-lightmode">Light</label>
  <div data-tab markdown="1">

Background: `transparent`, inherits toolbar background (Grey 10 `#f9f9fa`)

Icon: Grey 90 `#0c0c0d`

#### Hover

Background: Grey 20 `#ededf0`

Icon: Grey 90 `#0c0c0d`

#### Selected

Background: Grey 20 `#ededf0`

Icon: Blue 60 `#0060df`
  </div>

  <input type="radio" name="toolbar-style-color" id="toolbar-darkmode">
  <label for="toolbar-darkmode">Dark</label>
  <div data-tab markdown="1">

Background: `transparent`, inherits toolbar background (Grey 90 `#0c0c0d`)

Icon: Grey 40 `#b1b1b3`

#### Hover

Background: `#252526` *Photon color needed*

Icon: Grey 40 `#b1b1b3`

#### Selected

Background: `#252526` *Photon color needed*

Icon: `#75BFFF` *Photon color needed*
  </div>
</div>

</div>
</div>
<!-- == tabs end == -->

### Toolbar Tab Color


<!-- == tabs start == -->
<div class="grid-2" markdown="1">
![Toolbar tab styles](../images/components/toolbars/toolbars-style-tabs.png)

<div markdown="1">


<div data-tabs>
  <input type="radio" name="toolbar-tab-style-color" id="toolbar-tab-lightmode" checked="checked">
  <label for="toolbar-tab-lightmode">Light</label>
  <div data-tab markdown="1">

Background: `transparent`, inherits toolbar background (Grey 10 `#f9f9fa`)

Text: Grey 90 `#0c0c0d`

Icon: Grey 90 `#0c0c0d`

#### Hover

Background: Grey 20 `#ededf0`

Text: Grey 90 `#0c0c0d`

Icon: Grey 90 `#0c0c0d`

Tab top border (main toolbar only): `rgba(0,0,0,0.2)` *Photon color needed*

#### Selected

Background: `transparent`, inherits toolbar background (Grey 90 `#0c0c0d`)

Text: Blue 60 `#0060df`

Icon: Blue 50 `#0a84ff`

Tab top border (main toolbar only): Blue 50 `#0a84ff`

  </div>

  <input type="radio" name="toolbar-tab-style-color" id="toolbar-tab-darkmode">
  <label for="toolbar-tab-darkmode">Dark</label>
  <div data-tab markdown="1">

Background: `transparent`, inherits toolbar background (Grey 90 `#0c0c0d`)

Text: Grey 40 `#b1b1b3`

Icon: Grey 40 `#b1b1b3`

#### Hover

Background: `#252526` *Photon color needed*

Text: Grey 40 `#b1b1b3`

Icon: Grey 40 `#b1b1b3`

Tab top border (main toolbar only): `rgba(255,255,255,0.2)` *Photon color needed*

#### Selected

Background: `transparent`, inherits toolbar background (Grey 90 `#0c0c0d`)

Text: white `#ffffff`

Icon: white `#ffffff`

Tab top border (main toolbar only): Blue 50 `#0a84ff`

  </div>
</div>

</div>
</div>
<!-- == tabs end == -->


### Sizes

<div class="grid-2" markdown="1">
![Main toolbar measurements](../images/components/toolbars/toolbars-size-main.svg)

<div markdown="1">

#### Main toolbar

Height: `29px`

Text: `12px`, regular `400`

**Icons**

Width: `16px`

Height: `16px`

</div>
</div>




<div class="grid-2" markdown="1">
![sub-toolbar measurements](../images/components/toolbars/toolbars-size-subtoolbar.svg)

<div markdown="1">

#### Sub-toolbar

Height: `24px`

Text: `11px`, regular `400`

**Icons**

Width: `16px`

Height: `16px`
</div>
</div>




## Behaviours

Toolbars can contain a variety of different elements, these include but are not limited to:

* **Buttons** Often acting as tabs to alter the view of the window.
* **Separators** Typically a simple line which provides a method of separating groups of controls.
* **Icons** SVGs which typically appear within a button element to illustrate the button action.
* **Form controls** Checkboxes and input fields for filtering and customising the current view.




### Resizing 

<div class="grid-2" markdown="1">
![Toolbar Behaviour](../images/components/toolbars/toolbars-behaviour.png)

<div markdown="1">
When the parent panel of a toolbar is resized to a width that is smaller than the natural width of the toolbar’s combined child elements, an overflow button appears which provides menu ([doorhanger](doorhangers)) access to the elements which are no longer visible.

The double-chevron button is removed if the width of the parent panel is increased to allow for all of the toolbar menu items to appear in a  single row.
</div>
</div>

