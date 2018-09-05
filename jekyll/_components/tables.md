---
layout: page
title: Tables
order: 9
---

Tabular data appears in a variety of places, the Network panel is the most obvious example. The console is also able to output a visual table using `console.table()` e.g. `console.table(["apples", "oranges", "bananas"]);`

## Usage

<div class="grid-2" markdown="1">
![Usage Example of a Checkbox as used in Firefox Options](../images/components/tables/table-grid-light.png)

<div markdown="1">
Tables are used when data needs to be presented in a series of rows which may also posses any amount of columns. For large quantities of data it is recommended to include a button column header allowing users to sort the data by that specific column, as seen in the Network panel
</div>
</div>


## Types

### Console tables

<div class="grid-2" markdown="1">
![Console table example](../images/components/tables/console-table-small.png)

<div markdown="1">
The console can display a tablular representation of an Array or Object. e.g. `console.table(["apples", "oranges", "bananas"]);`

Console table columns are not sortable or resizable.
</div>
</div>

### Network and Application panel
    
<div class="grid-2" markdown="1">
![Network table timeline example](../images/components/tables/table-timeline.png)

<div markdown="1">
The Network panel table features column sorting and row highlighting on hover. the table can contain a rich variety of data including text, images (icons: `16px` x `16px`) and timeline interface elements like graphs and vertical rules (pictured).

Filter controls are provided in the form of buttons for specific resource types and a filter input field for filtering URLs.
</div>
</div>

## Styles

Table rows alternate their background color, the subtle "zebra" effect assists in legibility:

### Dark mode
<div class="grid-2" markdown="1">
![Usage Example of a Checkbox as used in Firefox Options](../images/components/tables/table-grid-dark.png)

<div markdown="1">
Odd rows: Grey 80 `#2a2a2e`

Even rows: `rgba(255,255,255,0.05)`

Column header: Grey 85 `#1b1b1d`

Borders/splitters: `#3c3c3d`

Text: Grey 40 `#b1b1b3`

Selected row: `#204E8A`
</div>
</div>

### Light mode
<div class="grid-2" markdown="1">
![Usage Example of a Checkbox as used in Firefox Options](../images/components/tables/table-grid-light.png)

<div markdown="1">
Odd rows: white `#ffffff`

Even rows: `rgba(0,0,0,0.05)`

Column header: Grey 10 `#f9f9fa`

Borders/splitters: Grey 25 `#e0e0e2`

Text: Grey 70 `#38383d`

Selected row: Blue 55 `#0074e8`
</div>
</div>


<div class="grid-2" markdown="1">
![Table size and font properties](../images/components/tables/table-size-properties.svg)
<div markdown="1">
Font size: `11px`

Row height: `24px`

Line height: `24px`
</div>
</div>

## Behaviours

### Sorting
<div class="grid-2" markdown="1">
![Table Column headers](../images/components/tables/table-header-button.png)

<div markdown="1">
Tables can posses sortable column headers, clicking these buttons will toggle the sorting of the column they relate to. In the image, clicking the "Size" button header toggles the Size column from largest to smallest and from smallest to largest.

Selected column header (Light mode): Blue 55 `#0074e8`

Selected column header (Dark mode): `#204E8A`
</div>
</div>

<div class="grid-2" markdown="1">
![Table Column headers](../images/components/tables/table-header-tooltip.png)

<div markdown="1">
If the table header is a clickable button to provide sorting controls, the tooltip should illustrate what the current sorting pattern is e.g. Sorted ascending, Sorted descending. 
</div>
</div>

### Rich tooltips and previews

<div class="grid-2" markdown="1">
![Example of an image preview as tooltip](../images/components/tables/table-rich-tooltips.png)

<div markdown="1">
Table cells tooltips have the opportunity to provide extra information/context to the data being hovered over. For example, a domain name when hovered can additionally provide the IP address of the domain.

When an image name is hovered over a [doorhanger](./doorhangers) should present a preview of the image with a caption containing the real pixel dimensions.

</div>
</div>

## Future Improvements

### Column resizing
The Network table in particular requires individual column resizing capabilities so that lengthy strings like filenames and domains can be read easily without the need to alter the devtools or browser window width. 
Perhaps not a requirement for console tables.

###Sortable console table columns
Tables output to the console appear static, column headers provide no sorting behaviours. 