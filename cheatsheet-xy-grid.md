# xy-grid cheatsheet

- The Foundation XY Grid System is a 12 column grid system based on Flexbox. 
- The flex grid has 12 spaces/cells per row.  Going over 12 measures means that items will wrap underneath
- &lt;DIV&gt; are used for demonstration only - use semantic tags where appropriate.
___NOTES:___ Foundation is mobile first, that means small-size is the default for all sizes, small-12 is always implied. This is not an instructional page for the grid system - use the documentation and youtube for that.

## SIZING COLUMNS/CELLS
| CLASS NAME | WHAT IT DOES | EXAMPLE|
|------------|--------------|--------|
|.grid&ndash;x | creates a wrapper for a horizontal grid |```<div class="grid-x"><div class="cell">...</div></div>```|
| `.grid-margin-x` | adds margins to the left and right sides of each cell|```<div class="grid-x grid-margin-x"><div class="cell">...</div></div>```|
| `.grid-padding-x` | adds padding to the left and right sides of each cell|```<div class="grid-x grid-margin-x"><div class="cell">...</div></div>```|
|`.grid-container`|By default the grid system expands to fit the __full browser window__.Grid container creates a max-width of 1200px and centers the containner on the page.|```<div class="grid-container"><div class="grid-x"><div class="cell">...</div></div></div>```|
| `.cell` | declares a cell, full width  by default | ```<div class="cell">...</div>```|
| `.small-1 ... .small-12` | specifies width for small screens | ```<div class="cell small-4">...</div>``` |
| `.medium-1 ... .medium-12` | specifies width for medium screens | ```<div class="cell medium-2">...</div>``` |
| `.large-1 ... .large-12` | specifies width for large screens | ```<div class="cell large-2">...</div>``` |




left
right




grid-y
grid-margin-y
grid-padding-y

