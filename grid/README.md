## Grid vs Flexbox

- Flexbox is great for navbars
- Grids for everything else

## How to use grid

- set `display: grid;` -- similar to display flex
- Grid goes from top to bottom. Need to specify rows (gtr) and columns (gtc).
- Can specify gap too - gap betwen all elements.
- GTC specifies how much screen width each column of your data takes. If there are 3 widths specified, your first 3 elements will take the specified width (can be expressed as a fraction of the available viewport too). Subsequent elements (4th, 5th) will go into the second row and follow the width fractions specified.
- GTR specifies the height of each row of your data. Elements that don't fit into the first column will go into the second row, etc.
- repeat(n, 1fr) creates n equally spaced rows or columns.
- grid-column and grid-row control how much of the grid each individual element occupies. grid-column 1/3 stretches an element from the 1st column to the start of the 3rd column (occupy first 2 columns). grid-row 1/3 does the same for rows - occupy first and second row.
