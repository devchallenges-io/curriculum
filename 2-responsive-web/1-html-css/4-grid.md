# Mastering CSS Grid: A Step-by-Step lesson

CSS Grid Layout revolutionized web design by allowing developers to precisely create complex layouts. Unlike older methods, CSS Grid provides a flexible and robust approach to element arrangement on a web page. It offers enhanced control over horizontal and vertical alignment of elements, facilitating responsive designs that adapt to various screen sizes. This advancement enables the creation of complex, adaptable layouts without necessitating complicated frameworks or hacks.

## 1. Understanding the Basics of CSS Grid

### Grid Container

When creating a CSS Grid layout, the main element you need is the _Grid Container_. This is simply an HTML element that acts as a container and has the `display: grid;` property applied to it. Once you do this, it becomes a powerful grid system where you can organize and arrange its child elements in any way you want.

<!-- TODO: add visualization here -->

### Grid Lines

A key concept in CSS Grid is _Grid Lines_. These are the lines that divide the grid into columns and rows. They act as reference points for positioning and aligning items within the grid. There are two types of grid lines:

1.  Vertical lines (column lines)
2.  Horizontal lines (row lines)

Every time you create a new column or row, two new grid lines are created — one at the start and one at the end.

### Grid Tracks

_Grid Tracks_ refer to the spaces between adjacent Grid Lines. In simpler terms, they are the columns and rows themselves. You can define these tracks using properties like `grid-template-columns` for columns and `grid-template-rows` for rows.

Here's how it works:

1.  When you define your tracks, you specify their sizes or behaviors.
2.  Each track can adjust its size based on its content or be given an explicit size using units like pixels, percentages, or fractions of free space (`fr`).

## 2. Exploring Grid Items, Grid Cells, and Grid Areas

When you use CSS Grid on a container element, the direct children become **Grid Items**. These items automatically join in the grid layout, positioning themselves according to the structure defined by **Grid Lines**.

- **Grid Item**: Any element that is a direct child of a Grid Container. It can be positioned and sized based on the grid’s defined tracks and areas.

The **Grid Cell** is the most basic unit within a CSS Grid, similar to a single cell in a table layout. It's formed by intersecting grid lines and serves as the fundamental building block of your layout.

- **Grid Cell**: The space between two adjacent row and two adjacent column grid lines. It's where content can be placed within the grid.

For organizing content that spans across multiple cells, CSS Grid provides **Grid Areas**. These are larger virtual spaces on your grid that can encompass one or more grid cells, allowing for more complex layouts.

- **Grid Area**: A space surrounded by four grid lines. A grid area can consist of any number of grid cells and is defined using properties like `grid-template-areas`.

Understanding these concepts helps you see how individual elements interact with CSS Grid structures. This knowledge will come in handy as you move on to creating layouts and manipulating items within your grid.

## 3. Creating a Basic CSS Grid Layout

To create a CSS Grid layout, follow these steps:

1.  Select an HTML container element that will serve as the Grid Container.
2.  Assign the **display** property to this element with the value of **grid**.

This single line of CSS is enough to convert the container into a grid layout where direct child elements become grid items.

```css
.container {
  display: grid;
}
```

Each direct child of the `.container` automatically takes its place in the grid. By default, they will position themselves as column tracks, filling up one row after another. This transforms a standard block-level flow into a powerful grid structure without additional markup or complex styles.

## 4. Defining Columns and Rows in CSS Grid

In CSS Grid, the `grid-template-columns` and `grid-template-rows` properties are crucial for creating the structure of your grid. They determine the column tracks and row tracks, which serve as the foundation of the entire grid layout.

### **Setting Up Column Tracks with **`grid-template-columns`**:**

You can use `grid-template-columns` to specify the number and sizes of columns in your grid container. By assigning values to this property, you can create column tracks that are fixed, flexible, or a combination of both.

```css
.container {
  display: grid;
  grid-template-columns: 100px 200px auto;
}
```

In this example:

1.  The first column is set to be exactly `100px` wide.
2.  The second column is defined as `200px`.
3.  The third column takes up the remaining space with `auto`.

### **Defining Row Tracks with **`grid-template-rows`**:**

Similarly, you can define the rows in your grid using `grid-template-rows`. This property determines the height of each row track.

```css
.container {
  display: grid;
  grid-template-rows: 150px auto 100px;
}
```

Here:

1.  The first row has a height of `150px`.
2.  The second row adjusts its height automatically based on its content.
3.  The third row is fixed at `100px`.

## 5. Placing Items in Specific Grid Cells

The `grid-column` and `grid-row` properties are essential for positioning items within a CSS Grid layout. These properties allow you to assign grid items to specific locations on the grid, giving you control over the placement of content.

### `grid-column`

This property determines a grid item's start and end positions along the column axis. Here are different ways to use it:

1.  **Single line number:** `grid-column: 2;` places the item starting at the second vertical grid line.
2.  **Span keyword:** `grid-column: span 3;` extends the item across three column tracks.
3.  **Line number range:** `grid-column: 1 / 3;` starts the item at the first line and ends it before the third line.

### `grid-row`

Similar to `grid-column`, this property defines where the grid item will sit along the row axis:

1.  **Single line number:** `grid-row: 1;` positions the item at the first horizontal grid line.
2.  **Span keyword:** `grid-row: span 2;` makes the item cover two row tracks.
3.  **Line number range:** `grid-row: 2 / 4;` sets the start and end of an item between specified row lines.

Combine these properties to target specific cells or areas:

```css
.item1 {
  grid-column: 1 / 3;
  grid-row: 1;
}
.item2 {
  grid-column: 3;
  grid-row: span 2;
}
```

In this example, `.item1` spans from column lines 1 to 3, occupying two columns and is placed in the first row. Conversely, `.item2` is positioned starting at column line 3 and spans two rows down. The flexibility offered by these properties enables designers to create complex layouts with elements spanning various cells, both horizontally and vertically.

## 6. Creating Grid Gaps for Spacing

The `gap` property, an essential tool in the CSS Grid arsenal, introduces a clear visual separation between grid items. It allows designers to define consistent space around items within a grid container, effectively controlling the padding between cells and rows.

### How to use `grid` or `grid-gap`

To apply spacing between grid items, set the `gap` property on the grid container element. This property can accept either one or two values:

- When one value is specified, it applies uniformly to both rows and columns.
- Two values allow individual specification for rows and columns respectively (first for rows, second for columns).

```css
.grid-container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px; /* Sets a 20px gap for both rows and columns */
}
```

Alternatively, `grid-row-gap` and `grid-column-gap` can be used to set row and column gaps independently.

```css
.grid-container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-row-gap: 20px; /* Sets a 20px gap between the rows _/ grid-column-gap: 10px; /_ Sets a 10px gap between the columns */
}
```

## 7. Aligning and Justifying Items in the Grid

CSS Grid provides powerful control over the alignment of items within your grid, which can be managed using `justify-items`, `align-items`, `justify-content`, and `align-content`. These properties influence how content fits within both the grid container and individual grid items.

### `justify-items`

This property aligns grid items along the inline (row) axis. By default, it is set to 'stretch', which causes items to fill the entire cell width. However, it can be set to 'start', 'end', 'center', or 'stretch' to achieve different effects.

```css
.container {
  display: grid;
  justify-items: start; /* Aligns items to the start of each cell */
}
```

### `align-items`

Similar to `justify-items`, but for the block (column) axis. It determines vertical placement within grid cells. Set its value to 'start', 'end', 'center', or 'stretch'.

```css
.container {
  display: grid;
  align-items: end; /* Aligns items to the end of each cell vertically */
}
```

### `justify-content`

This adjusts the position of the grid itself within the container along the inline axis when there is extra space outside of explicit tracks. Options include 'start', 'end', 'center', 'stretch', 'space-around', 'space-between', and 'space-evenly'.

```css
.container {
  display: grid;
  width: 100%;
  justify-content: space-between; /* Distributes extra space between columns */
}
```

### `align-content`

Operates like `justify-content`, but on the block axis. This property comes into play when there's more space in the grid container than required by the tracks.

```css
.container {
  display: grid;
  height: 400px;
  align-content: center; /* Centers the rows vertically within the container */
}
```

Leveraging these alignment properties ensures that designers have granular control over how elements are presented in their layouts, leading to more polished and precise designs. With careful application, it is possible to create a layout that looks great on all screen sizes and maintains consistency across different browsers.

## 8. Changing the Order of Grid Items

In CSS Grid, you can change the visual order of grid items using the `order` **property**. This feature was first introduced in CSS Flexbox and now also available in CSS Grid. The `order` property allows you to rearrange items independently of their source order within the HTML document.

Here's an example of how you can use the `order` property in CSS:

```css
.grid-item {
  order: 1; /* Assigns an order value to the grid item */
}
```

## 9. Creating Responsive Grid Layouts

Responsive design is essential for ensuring that web applications provide an optimal experience across various devices. The `minmax()` function in CSS Grid allows developers to define flexible grid tracks that can adapt seamlessly to different screen sizes.

### **Using the **`minmax()`** function:**

- The `minmax()` function takes two parameters: a minimum value and a maximum value.
- It enables grid tracks to have a range of acceptable sizes rather than a fixed size.
- Syntax example: `grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));`

This approach ensures that grid items are displayed effectively on both smaller screens, such as mobile phones, and larger ones, like desktop monitors. By setting a minimum size, content maintains readability and usability without shrinking too small. Conversely, the maximum value prevents grid items from stretching excessively on larger screens.

In practice:

```css
.container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
}
```

Here, the grid container `.container` sets up columns with a minimum width of `250px`. The columns expand to fill available space without exceeding the fraction of the container they are allocated (`1fr`). On narrower screens, fewer columns will fit before hitting the minimum size constraint, while wider screens will accommodate more columns within the maximum size constraint.

By integrating the `minmax()` function into responsive layouts, designers gain control over how content scales and adapts to different devices, ensuring consistent user experiences.

## 10. Building Complex Grid Structures

Nested grids and Grid Line Names are powerful tools for creating complex and sophisticated web layouts.

### Nested Grids

Implementing nested grids involves setting a grid item as a grid container itself. This allows the creation of a sub-grid within the main grid, offering increased layout flexibility and control. Here's an example:

```css
.container {
  display: grid;
  grid-template-columns: 1fr 2fr;
}

.item {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}
```

In this scenario, `.item` becomes a grid container with its own set of columns, independent of the parent `.container`. This technique is particularly useful when designing components that require their own unique layout structure, such as cards or sidebar menus.

### Grid Line Names

Grid Line Names simplify the process of placing items by assigning meaningful names to grid lines. Instead of relying on numerical positioning which can become unclear in complex layouts, named lines enhance readability and maintainability. Define line names when setting up `grid-template-columns` or `grid-template-rows` like so:

```css
.container {
  display: grid;
  grid-template-columns: [start]100px[main-start]1fr[main-end]100px[end];
}
```

To position items using these names:

```css
.item {
  grid-column: main-start / main-end;
}
```

This method clearly communicates where an item should be placed within the grid, reducing errors and making code adjustments easier for developers who may be collaborating on a project.

## Conclusion

Mastering CSS Grid empowers web developers with a robust toolset for crafting sophisticated, two-dimensional layouts that seamlessly adapt to the dynamic needs of modern web design. This comprehensive guide has journeyed through the foundational concepts, advancing to complex grid structures, underscoring the versatility and power of CSS Grid.
