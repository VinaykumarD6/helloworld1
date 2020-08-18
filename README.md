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

