Basic HTML:

<h1></h1>
<h2></h2>
<h3></h3>
<h4></h4>
<h5></h5>
<h6></h6>
<p></p>
Comments in HTML start with <!-- and end with a -->

HTML5 introduces more descriptive HTML tags. These include main, header, footer, nav, video, article, section and others.

<img src="https://www.your-image-source.com/your-image.jpg" alt="Author standing on a beach with two thumbs up.">

Note that img elements are self-closing.

All img elements must have an alt attribute. The text inside an alt attribute is used for screen readers to improve accessibility and is displayed if the image fails to load.


Note: If the image is purely decorative, using an empty alt attribute is a best practice.



You can use a (anchor) elements to link to content outside of your web page.

a elements need a destination web address called an href attribute. They also need anchor text. Here's an example:

<a href="https://freecodecamp.org">this links to freecodecamp.org</a>


Replace the href attribute value with a #, also known as a hash symbol, to create a dead link.

For example: href="#"



Turn an Image into a LinkPassed
<a href="#"><img src="https://bit.ly/fcc-running-cats" alt="Three kittens running towards the camera."></a>




HTML has a special element for creating unordered lists, or bullet point style lists.

Unordered lists start with an opening <ul> element, followed by any number of <li> elements. Finally, unordered lists close with a </ul>

For example:

<ul>
  <li>milk</li>
  <li>cheese</li>
</ul>


HTML has another special element for creating ordered lists, or numbered lists.

<ol>
  <li>Garfield</li>
  <li>Sylvester</li>
</ol>


You can create a text input like this:

<input type="text">

Note that input elements are self-closing.



Placeholder text is what is displayed in your input element before your user has inputted anything.

You can create placeholder text like so:

<input type="text" placeholder="this is placeholder text">

<form action="/url-where-you-want-to-submit-form-data"></form>

<button type="submit">this button submits the form</button>

For example, if you wanted to make a text input field required, you can just add the attribute required within your input element, like this: <input type="text" required>

<label for="indoor"> 
  <input id="indoor" type="radio" name="indoor-outdoor">Indoor 
</label>


<label for="loving"><input id="loving" type="checkbox" name="personality"> Loving</label>












Responsive Wen Design rules:

1.  @media media-type (max-width: 100px) { /* CSS Rules */ }
media-type can be all/screens/speech

@media (min-height: 350px) { /* CSS Rules */ }

2.  Make an Image Responsive:
img {
  max-width: 100%;
  height: auto;
}

3.  Use a Retina Image for Higher Resolution Displays:
The simplest way to make your images properly appear on High-Resolution Displays, such as the MacBook Pros "retina display" is to define their width and height values as only half of what the original file is. Here is an example of an image that is only using half of the original height and width:

<style>
  img { height: 250px; width: 250px; }
</style>
<img src="coolPic500x500" alt="A most excellent picture">

4.  To Make Typography Responsive: can use viewport units for responsive typography.

Viewport units are relative to the viewport dimensions (width or height) of a device, and percentages are relative to the size of the parent container element.

The four different viewport units are:

vw (viewport width): 10vw would be 10% of the viewport's width.
vh (viewport height): 3vh would be 3% of the viewport's height.
vmin (viewport minimum): 70vmin would be 70% of the viewport's smaller dimension (height or width).
vmax (viewport maximum): 100vmax would be 100% of the viewport's bigger dimension (height or width).




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

grid-area: horizontal line to start at / vertical line to start at / horizontal line to end at / vertical line to end at;

grid-template-rows: repeat(100, 50px); //create the 100 row grid, each row at 50px tall.

grid-template-columns: 100px minmax(50px, 200px);// minmax is used to limit the size of items when the grid container changes size.

grid-template-columns: repeat(auto-fill, minmax(60px, 1fr)); //auto-fill allows you to automatically insert as many rows or columns of your desired size as possible depending on the size of the container.

grid-template-columns: repeat(auto-fit, minmax(60px, 1fr)); //auto-fill keeps inserting empty rows or columns and pushes your items to the side, while auto-fit collapses those empty rows or columns and stretches your items to fit the size of the container.

Grid with grids






