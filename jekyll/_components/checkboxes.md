---
layout: page
title: Checkboxes
order: 1
---

A checkbox is used to choose between two opposite states, often to select/deselect items or enable/disable actions.

Toggles provide an alternative UI for the same use cases and are often used on mobile.

## Usage

<div class="grid-2" markdown="1">
![Usage Example of a Checkbox as used in Firefox Options](../images/components/checkboxes/checkbox-usage.png)

Use checkboxes to provide a binary choice. For example to offer a choice about performing an action or not. It is considered “on” when it is checked, and “off” when it’s not.
</div>

## Combination

A checkbox can be used as a single element, or it can be combined into a list, or nested list of elements to pick multiple from.

### Single

<div class="grid-2" markdown="1">
![Example of a Single Checkbox](../images/components/checkboxes/checkbox-combination-single.svg)

Use one checkbox to offer one binary choice.
</div>

### Group

<div class="grid-2" markdown="1">
![Example of a Group of 3 Checkboxes](../images/components/checkboxes/checkbox-combination-group.svg)

Group checkboxes to convey a set of choices are related.
</div>

### Nested Group

<div class="grid-2" markdown="1">
![Example of 2 Checkboxes Nested Under Another Checkbox](../images/components/checkboxes/checkbox-combination-nested.svg)

<div markdown="1">
Nest checkboxes to convey that some options are only available if the parent option is selected.

> See [Nesting](../patterns/nesting.html) for more info on how to nest elements.
</div>
</div>

## Style

A checkbox consists of a part to indicate its state and a label to describe the binary choice it represents.

### Indicator & Label

<div class="grid-2" markdown="1">
![Example of a checked and an unchecked Checkbox.](../images/components/checkboxes/checkbox-states.svg)

<div markdown="1">
Use the indicator to show whether the checkbox is checked (“on”) or not (“off”).

Use the label to make the action clear and convey that it is a binary choice.
</div>
</div>

### Dimensions

<div class="grid-2" markdown="1">
![Illustration of the Size of a Checkbox.](../images/components/checkboxes/checkbox-size.svg)

<div markdown="1">
Corner Radius: `2px`

Height: `16px`

Width: `16px`

Horizontal Padding: `4px`
</div>
</div>

### Text and Color

<div class="grid-2" markdown="1">
![Illustration of a checked Checkbox.](../images/components/checkboxes/checkbox-checked.svg)

<div markdown="1">
Text: [Body 10](../visuals/typography.html#scale)

Text Color: Grey 90 `#0c0c0d`
</div>
</div>

### Toggle 

<div data-tabs>
  <input type="radio" name="tstyle" id="style-generic" checked="checked">
  <label for="style-generic">Light</label>
  <div data-tab markdown="1">

<div class="grid-2" markdown="1">
![Toggle in light mode](../images/components/checkboxes/checkbox-toggle-light.png)

<div markdown="1">

Cursor: `pointer`

#### Disabled

Background: Grey 30 `#d7d7db`

Switch(thumb): White `#ffffff`

#### Enabled

Background: Blue 55 `0074e8`

Switch(thumb): White `#ffffff`

</div>
</div>
  </div>


  <input type="radio" name="tstyle" id="style-success">
  <label for="style-success">Dark</label>
  <div data-tab markdown="1">

<div class="grid-2" markdown="1">
![Toggle in dark mode](../images/components/checkboxes/checkbox-toggle-dark.png)

<div markdown="1">
Cursor: `pointer`

#### Disabled

Background: Grey 60 `#4a4a4f`

Switch(thumb): Grey 40 `#b1b1b3`

#### Enabled

Background: Blue 55 `0074e8`

Switch(thumb): White `#ffffff`
</div>
</div>
  </div>
</div>

## Behaviors

### On / Off

<div class="grid-2" markdown="1">
![Example of a checked and an unchecked Checkbox.](../images/components/checkboxes/checkbox-states.svg)

<div markdown="1">
#### Checked (On):

Icon: [Checkbox-Check](../images/components/checkboxes/checkbox-check-16.svg)

Background Color: Blue 60 `#0060df`

#### Unchecked (Off):

Background Color: Grey 90 a10 `rgba(12, 12, 13, 0.1)`

Border: 1px Grey 90 a30 `rgba(12, 12, 13, 0.3)`
</div>
</div>

### Clicktarget

<div class="grid-2" markdown="1">
![Illustration of the extent of the clicktarget of a Checkbox.](../images/components/checkboxes/checkbox-clicktarget.svg)

<div markdown="1">
A checkbox can be toggled by clicking on the area of its checkbox as well as its label. Usually the clicktarget extends to the same width for each element in a collection of checkboxes. This results in a click target that extends beyond the label, for all elements shorter than the longest.

Clicking a checkbox triggers the action on release of the click. If, during the click, the mouse is moved off of the checkbox, no action is triggered.
</div>
</div>

### Disabled

<div class="grid-2" markdown="1">
![Illustration of a checked and an unchecked disabled Checkbox.](../images/components/checkboxes/checkbox-disabled.svg)

<div markdown="1">
40% Opacity

Can not be interacted with nor focused.
</div>
</div>

### Interaction

#### Checked

<div class="grid-2" markdown="1">
![Illustration of all appearances a checked Checkbox can show when interacted with.](../images/components/checkboxes/checkbox-interaction-checked.png)

<div markdown="1">
Background Color:

Default: Blue 60 `#0060df`

Hover: Blue 70 `#003eaa`

Pressed: Blue 80 `#002275`

##### Focused:

Border: none

Box Shadow: `0 0 0 1px #0a84ff inset, 0 0 0 1px #0a84ff, 0 0 0 4px rgba(10, 132, 255, 0.3)`
</div>
</div>

#### Unchecked

<div class="grid-2" markdown="1">
![Illustration of all appearances an unchecked Checkbox can show when interacted with.](../images/components/checkboxes/checkbox-interaction-unchecked.png)

<div markdown="1">
Background Color:

Default: Grey 90 a10 `rgba(12, 12, 13, 0.1)`

Hover: Grey 90 a20 `rgba(12, 12, 13, 0.2)`

Pressed: Grey 90 a30 `rgba(12, 12, 13, 0.3)`

##### Focused:

Border: none

Box Shadow: `0 0 0 1px #0a84ff inset, 0 0 0 1px #0a84ff, 0 0 0 4px rgba(10, 132, 255, 0.3)`
</div>
</div>


#### Toggle Animation

<div class="grid-2" markdown="1">
![Toggle slide animation](../images/components/checkboxes/checkbox-toggle-animation.gif)
{:.animated}

<div markdown="1">
On click, the toggle control animates between disabled and enabled states.

The animation includes the transitioning background colors and the switch movement from left to right (enabling) and right to left (disabling).


</div>
</div>


## Copy Rules

* Use the imperative voice for checkbox labels.

* Do not use terminal punctuation for checkbox labels.

* Maintain parallel construction for lists of related checkbox labels.

## Future Improvements

<div class="grid-2" markdown="1">
![Toggle slide animation](../images/components/checkboxes/checkbox-toggle-future.svg)
{:.animated}

<div markdown="1">
A revision to the toggle control is soon to appear in the ‘about’ pages of Firefox. The redesign features a tick symbol to reinforce clarity of the enabled state.


</div>
</div>
