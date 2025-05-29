<p>
It was decided to make a parquet floor in a room of size NxM. The idea is to lay out some pattern on the floor. The parquet tiles with which the floor of the room looks best consist of squares 1x1, each of which can be either white or black. The required color of each square of the room is specified on the map of the room.</p><p>
There are four different forms of parquet tiles: <br><br>
<img src="/content/turbo:img0001.png" alt="Illustration of parquet tiles"><br><br>
Squares of one parquet tile can be painted differently. Some types of tiles can be of identical shape, but painted differently. Tiles of different types can have different cost. The number of available tiles of each type is not limited. Tiles are allowed to be turned around somehow (by an angle which is a multiple of 90 degrees), but it is not permitted to break a tile or to put it face sheet downwards. Initially, any part of the floor can be already laid out by tiles. You are requested to calculate the minimal cost of the tiles necessary to pave the remaining part of the room. </p>

<h3>Input</h3>
<p><i>t</i> ¨C the number of test cases, then <i>t</i> test cases follow. <br>
In the first line of each test case three numbers are written: <i>N, M</i> (the sizes of the room) and <i>K</i> (number of accessible types of tiles). <i>[1&lt;= N, M &lt;= 8], [1 &lt;= K &lt;= 10]</i>.
Next there is a description of the desired painting of the floor. The description is given in the form of <i>N</i> lines of <i>M</i> numbers each, where 0 denotes the color white, 1 - the color black, 2 - a square which has already been covered by a tile. In the last K lines the descriptions of available types of tiles are given in the following format: <br>
[Form] [cost] [painting] where:<br>
[Form] is a number from 1 to 4, describing the form of a tile (see figure above) <br>
[Cost] is an integer not larger than 10000, describing the cost of one tile of the type. <br>
[Painting] is a sequence of between one and three numbers 0 or 1. Its length is the same as the number of squares of which the tile consists, and the respective numbers describe colors of square tiles in the order in which the squares are numbered in the figure.
</p>

<h3>Output</h3>
<p>For each test case output one integer: the minimal cost of laying the remaining part of the parquet, or -1 if the task cannot be performed.</p>

<h3>Example</h3>
<p><b>Input:</b></p>
<pre>1
4 3 3
2 2 2
2 0 0
2 1 2
2 2 2
2 10 0 0
1 5 1
4 6 0 0 1
</pre>

<p><b>Output:</b></p>
<pre>15
</pre>