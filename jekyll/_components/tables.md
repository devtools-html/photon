---
layout: page
title: Tables
order: 9
draft: true
---

Tabular data appears in a variety of places, the Network panel is the most obvious example. The console is also able to output a visual table using `console.table()` e.g. `console.table(["apples", "oranges", "bananas"]);`.

## Usage

<div class="grid-2" markdown="1">
![Network table](../images/components/tables/table-grid-light.png)

<div markdown="1">
Tables are used when data needs to be presented in a series of rows which may also possess any amount of columns. For large quantities of data it is recommended to include an interactive column header allowing users to sort the data by that specific column, as seen in the Network panel.
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
The Network panel table features column sorting and row highlighting on hover. The table can contain a rich variety of data including text, badges, images ([icons](../visuals/iconography): `16px` x `16px`) and timeline interface elements like graphs and vertical rules (pictured).
</div>
</div>

<div class="grid-2" markdown="1">
![Network table filter controls](../images/components/tables/table-filter-tools.svg)

<div markdown="1">
Filter controls are provided in the form of buttons for specific resource types and a filter input field for filtering URLs.
</div>
</div>

## Styles

Table rows alternate their background color, the subtle "zebra" effect assists in legibility:

### Dark mode
<div class="grid-2" markdown="1">
![Network table in dark mode](../images/components/tables/table-grid-dark.png)

<div markdown="1">
Odd Row Background Color: Grey 80 `#2a2a2e`

Even Row Background Color: `rgba(255,255,255,0.05)` (RGBA overlays the default Grey 80 `#2a2a2e`)

Column Header Background Color: Grey 85 `#1b1b1d`

Border/splitter Color: Grey 70 `#38383d`

Text Color: Grey 40 `#b1b1b3`

#### Selected row:

Background Color: Blue 70 `#003eaa`

Text Color: white `#ffffff`
</div>
</div>

### Light mode
<div class="grid-2" markdown="1">
![Network table in light mode](../images/components/tables/table-grid-light.png)

<div markdown="1">
Odd Rows Background Color white `#ffffff`

Even Rows Background Color: `rgba(0,0,0,0.05)` (RGBA overlays the default white `#ffffff`)

Column Header Background Color: Grey 10 `#f9f9fa`

Border/splitter Color: Grey 25 `#e0e0e2`

Text Color: Grey 70 `#38383d`

#### Selected row:

Background Color: Blue 55 `#0074e8`

Text Color: white `#ffffff`
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
![Table column headers](../images/components/tables/table-header-button.png)

<div markdown="1">
Tables should possess sortable column headers, clicking these buttons will toggle the sorting of the column they relate to. 

In the image, clicking the interactive "Size" header toggles the Size column from largest to smallest and from smallest to largest.

#### Selected Column Header (Light mode):

Background Color: Blue 55 `#0074e8`

#### Selected Column Header (Dark mode):

Background Color: Blue 70 `#003eaa`
</div>
</div>

<div class="grid-2" markdown="1">
![Table column tooltip](../images/components/tables/table-header-tooltip.png)

<div markdown="1">
If the table header is a clickable button to provide sorting controls, the tooltip should illustrate what the current sorting pattern is e.g. Sorted ascending, Sorted descending. 
</div>
</div>

### Rich tooltips and previews

<div class="grid-2" markdown="1">
![Example of an image preview as tooltip](../images/components/tables/table-rich-tooltips.png)

<div markdown="1">
Table cell tooltips have the opportunity to provide extra information/context to the data being hovered over. For example, a domain name when hovered can additionally provide the IP address of the domain.

When an image name is hovered over a [doorhanger](./doorhangers) should present a preview of the image with a caption containing the real pixel dimensions.

</div>
</div>

## Future Improvements

### Column resizing and sorting

All tables should provide column resizing and sorting functionality. Currently, not all tables provide these features.

The Network table requires individual column resizing capabilities so that lengthy strings like filenames and domains can be read easily without the need to alter the devtools or browser window width. 

Tables output to the console appear static, column headers provide no sorting behaviours. 

### Revision to zebra stripe and hover color scheme

The current table zebra effect is quite intense and should be revised for a subtler appearance that is easier on the eyes. Additionally, the row highlight color should perhaps be a modification of the underlying row color as opposed to being a solid hover color for both odd and even rows, this will retain the zebra effect while moving the cursor down the table. 

See: [Improve zebra table colors (Network, Storage)](https://github.com/devtools-html/ux/issues/10) 