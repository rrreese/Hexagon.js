Hexagon.js
==========

A JavaScript library for drawing and interacting with hex grids. [Demo and usage](https://robert-reese.squarespace.com/blog/hexagonjs)

Currently Hexagon.js only supports flat topped hexagons (pull requests welcome).


Simply use the following html:

    <!DOCTYPE html>
    <head>
        <title>Hex</title>
        <script src="hexagon.js"></script>
    </head>
    <body>
        <canvas id="HexCanvas" width="1000" height="700"></canvas>
        <script>
            var hexagonGrid = new HexagonGrid("HexCanvas", 50);
            hexagonGrid.drawHexGrid(7, 10, 50, 50, true);
        </script>    
    </body>


Call the HexagonGrid constructor with the id of your canvas and the radius of your hexagons. drawHexGrid takes the number of columns and rows followed by  an offset. Optionally the coordinate system can be displayed.

A hexagon can be drawn at an abitrary point with drawHex(). Additionally there is the helper function drawHexAtColRow() which draws a hexagon at a grid column/row coordinate.
