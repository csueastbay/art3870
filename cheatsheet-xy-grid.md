FOUNDATION XY-GRID Horizontal / Basic Grid Cheatsheet

- The Foundation XY Grid System is a 12 column grid system based on Flexbox. 
- The flex grid has 12 spaces/cells per row.  Going over 12 measures means that items will wrap underneath
- &lt;DIV&gt; are used for demonstration only - use semantic tags where appropriate.
___NOTES:___ Foundation is mobile first, that means small-size is the default for all sizes, small-12 is always implied. This is not an instructional page for the grid system - use the documentation and youtube for that.

## CELLS
| CLASS NAME | WHAT IT DOES | EXAMPLE|
|------------|--------------|--------|
| .cell | declares a cell, full width  by default | ```<div class="cell">...</div>```|
| .small-1 ... .small-12 | specifies width for small screens and larger | ```<div class="cell small-4">...</div>``` |
| .medium-1 ... .medium-12 | specifies width for medium screens and larger | ```<div class="cell medium-2">...</div>``` |
| .large-1 ... .large-12 | specifies width for large screens | ```<div class="cell large-2">...</div>``` |
| .auto |use to automaticially let foundation calculate the space that is left over for small or larger|``` <div class="cell small-4">...</div><div class="auto cell">...</div><div class="auto cell">...</div><div class="auto cell">...</div>```|
|.medium-auto|same as above for medium or larger||
|.large-auto|same as above for large||
|.shrink| Only take up the space the content needs.||

## ROWS/CONTAINERS
| CLASS NAME | WHAT IT DOES | EXAMPLE|
|------------|--------------|--------|
|.grid-x | creates a wrapper for a horizontal grid |```<div class="grid-x"><div class="cell">...</div></div>```|
| .grid-margin-x | adds margins to the left and right sides of each cell|```<div class="grid-x grid-margin-x"><div class="cell">...</div></div>```|
| .grid-padding-x | adds padding to the left and right sides of each cell|```<div class="grid-x grid-margin-x"><div class="cell">...</div></div>```|
|.medium-margin-collapse | collapses the margin for medium and larger screens |```<div class="grid-x grid-margin-x medium-margin-collapse"><div class="cell">...</div></div>```|
|.large-margin-collapse | collapses the margin for large screens |```<div class="grid-x grid-margin-x large-margin-collapse"><div class="cell">...</div></div>```|
|.medium-padding-collapse| does the same as margin collapse ||
|.medium-padding-collapse| does the same as margin collapse ||

## PAGE/CONTAINERS
| CLASS NAME | WHAT IT DOES | EXAMPLE|
|------------|--------------|--------|
|.grid-container|By default the grid system expands to fit the __full browser window__.Grid container creates a max-width of 1200px and centers the containner on the page.|```<div class="grid-container"><div class="grid-x"><div class="cell">...</div></div></div>```|
|grid-container-padded |adds padding to the grid container - not the cells |```<div class="grid-container grid-container-padded">``` |

## SOURCE ORDERING (start with correct order on mobile - normal document flow)
| CLASS NAME | WHAT IT DOES | EXAMPLE|
|------------|--------------|--------|
|.medium-order-1 ... medium-order-n | moves the container into the order specified within each enclosing container for medium or larger |.|
|.large-order-1 ... large-order-n | moves the container into the order specified within each enclosing container for large |.|

## UTILITIES ( https://foundation.zurb.com/sites/docs/flexbox-utilities.html )
| CLASS NAME | WHAT IT DOES | EXAMPLE|
|------------|--------------|--------|
| .small-offset-1 ... .small-offset-11| adds a left margin to the cell size based on column count for small and up ||
| .medium-offset-1 .... .medium-offset-11 |adds a left margin to the cell size based on column count for medium and up ||
| .large-offset-1 ... .large-offset-11 |adds a left margin to the cell size based on column count for large ||
| .align-right | Horizontal alignment classes are applied to flex parents. Left alignment is the default| ```<div class="grid-x grid-padding-x align-center"><div class="cell small-4">...</div><div class="cell small-4">...</div></div>```|
| .align-center | Aligned to the center | ```<div class="grid-x grid-padding-x align-center"><div class="cell small-4">...</div><div class="cell small-4">...</div></div>```|
| .align-justify| Aligned to the edges | ```<div class="grid-x grid-padding-x align-justify"><div class="cell small-4">...</div><div class="cell small-4">...</div></div>```|
| .align-spaced | Aligned to the space around | ```<div class="grid-x grid-padding-x align-spaced"><div class="cell small-4">...</div><div class="cell small-4">...</div></div>```|


## BLOCK GRID (creates a series of equally sized items in a block grid, great for gallerys of thumbnails)
| CLASS NAME | WHAT IT DOES | EXAMPLE|
|------------|--------------|--------|
|.small-up-1 ... .small-up-12| specifies a row of 2 items for small screens and up| ```<div class="grid-x grid-margin-x grid-margin-y small-up-2"><div class="cell"><img src="" alt=""></div></div>```|
|.medium-up-1 ... .medium-up-12| specifies a row of 2 items for medium screens and up| ```<div class="grid-x grid-margin-x grid-margin-y small-up-2 medium-up-3"><div class="cell"><img src="" alt=""></div></div>```|
|.large-up-1 ... .large-up-12| specifies a row of 2 items for large screens| ```<div class="grid-x grid-margin-x grid-margin-y small-up-2 medium-up-3 large-up-4"><div class="cell"><img src="" alt=""></div></div>```|

