CSS FLEX BOX:

display: flex;

flex-direction: row(default)/row-reverse/column/column-reverse;

justify-content: center/flex-start/flex-end/space-between/space-around/space-evenly;

align-elements: flex-start/flex-end/center/stretch/base-line;

flex-wrap: nowrap/wrap/wrap-reverse;

flex-shrink: numbers; //less value will shrink more, high value will shrink more

flex-grow: numbers; //less value will grow less, high value will grow more

flex-basis: basic sizes in (em or px or %); //specifies the initial size of the item before CSS makes adjustments with flex-shrink or flex-grow

flex: flex-grow flex-shrink flex-basis
//will grow if size greater than flex-basis and will shrink if size less than flex-basis

order: value; //order property is used to tell CSS the order of how flex items appear in the flex container

align-self: flex-start/flex-end/center/stretch/base-line; //to adjust each item's alignment individually, instead of setting them all at once.



CSS GRID:

display: grid;

grid-template-columns: 100px 100px 100px; // to add three columns of size 100 px to grid

grid-template-rows: 100px 100px 100px; // to add three rows of size 100 px to grid

fr: sets the column or row to a fraction of the available space,

auto: sets the column or row to the width or height of its content automatically,

%: adjusts the column or row to the percent width of its container.

grid-column-gap: 10px; // to add gap between columns

grid-row-gap: 10px; // to add gap between rows

grid-gap: value; //it will create gap between all columns and rows

grid-gap: value1 value2; //value1 is used to set gap between rows and value2 is used to set gap between columns;

grid-column: 1 / 3; //This will make the item start at the first vertical line of the grid on the left and span to the 3rd line of the grid, consuming two columns.

grid-row: 1 / 3; //This will make the item start at the first horizontal line of the grid on the top and span to the 3rd line of the grid, consuming two rows.4

justify-self: start/ center/ end/ stretch; //this will justify horizontally 

align-self: start/ center/ end/ stretch; //this will justify vertically

justify-items: start/ center/ end/ stretch; //this will justify horizontally all items in grid;

align-items: start/ center/ end/ stretch; //this will justify vertically all items in grid;

grid-template-areas:
  "header header header"
  "advert content content"
  "footer footer footer";

grid-area: header/ footer; //you can place an item in your custom area by referencing the name you gave it






