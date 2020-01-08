# GriddieJS

### Goal: Create a library for creating grid system with P5Js. Make the process of creating grids or game boards much easier

##### Functions

###### createGrid(tx,ty,options)

Creates the grid object, set to a variable to store it. 
Parameters:
  tx: amount of tiles in the x
  ty: amount of tiles in the y
  options: additional optional parameters
    xoff: offset of the grid from the side of the canvas
    yoff: offset of the grid from the top of the canvas
    offmode: How the offsets are applied
      CORNER: offset will only apply to the left and top side. DEFAULT OPTION
      ALL: offset will apply to all sides (which will keep it centered)
     spacing: amount of spacing in between each tile.
     param: additional paramaters specified by the user. Given as an object with the key being the
            name and the value being the default value when the grid is created.
            
##### Methods

###### For Tiles:
.middle: will give the middle of the tile as [x,y]
.x or .y will give the x or y position of the corner of the tile. (Shorthand for .corner(0)]
.corner(c) will give the x and y as [x,y] of the specified corner, 0-3 going top left, top right, bottom left, bottom right. 
