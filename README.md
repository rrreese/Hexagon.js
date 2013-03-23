Hexagon.js
==========

A JavaScript library for drawing and interacting with hex grids.

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
            hexagonGrid.drawHexGrid(200, 100, 10, 30, true);
        </script>    
    </body>



Call the HexagonGrid constructor with the id of your canvas and the radius of your hexagons. drawHexGrid takes and offset followed by the number of columns and rows. Optionally the coordinate system is displayed.

