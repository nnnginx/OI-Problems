<p>Finding the shortest path that goes from a starting point to a destination point given a set of points and route lengths connecting them is an already well known problem, and it's even part of our daily lives, as shortest path programs are widely available nowadays.<br><br> Most people usually like very much these applications as they make their lives easier. Well, maybe not that much easier.<br><br> Now that almost everyone can have access to GPS navigation devices able to calculate shortest paths, most routes that form the shortest path are getting slower because of heavy traffic. As most people try to follow the same path, it's not worth it anymore to follow these directions.<br><br> With this in his mind, your boss asks you to develop a new application that only he will have access to, thus saving him time whenever he has a meeting or any urgent event. He asks you that the program must answer not the shortest path, but the almost shortest path. He defines the almost shortest path as the shortest path that goes from a starting point to a destination point such that no route between two consecutive points belongs to any shortest path from the starting point to the destination.<br><br> For example, suppose the figure below represents the map given, with circles representing location points, and lines representing direct, one-way routes with lengths indicated. The starting point is marked as S and the destination point is marked as D. The bold lines belong to a shortest path (in this case there are two shortest paths, each with total length 4). Thus, the almost shortest path would be the one indicated by dashed lines (total length 5), as no route between two consecutive points belongs to any shortest path. Notice that there could exist more than one possible answer, for instance if the route with length 3 had length 1. There could exist no possible answer as well.<br></p>
<p><img src="../../../content/disatoba:almost.gif" border="0" alt="subir imagenes"></p>
<h3>Input</h3>
<p>The input contains several test cases. The first line of a test case contains two integers <em>N</em> (2   �� <em>N</em> �� 500) and <em>M</em> (1   �� <em>M</em> �� 10<sup>4</sup>), separated by a single space, indicating respectively the number of points in the map and the number of existing one-way routes connecting two points directly. Each point is identified by an integer between 0 and <em>N</em> -1.  The second line contains two integers <em>S</em> and <em>D</em>, separated by a single space, indicating respectively the starting and the destination points (<em>S</em> �� <em>D</em>; 0   �� <em>S</em>, <em>D</em> &lt;  <em>N</em>). <br><br> Each one of the following <em>M</em> lines contains three integers <em>U</em>, <em>V</em> and <em>P</em> (<em>U</em> �� <em>V</em>; 0   �� <em>U</em>, <em>V</em> &lt;  <em>N</em>; 1   �� <em>P</em> �� 10<sup>3</sup>), separated by single spaces, indicating the existence of a one-way route from <em>U</em> to <em>V</em> with distance <em>P</em>.  There is at most one route from a given point <em>U</em> to a given point <em>V</em>, but notice that the existence of a route from <em>U</em> to <em>V</em> does not imply there is a route from <em>V</em> to <em>U</em>, and, if such road exists, it can have a different length. The end of input is indicated by a line containing only two zeros separated by a single space.</p>
<h3>Output</h3>
<p>For each test case in the input, your program must print a single line, containing  <tt>-1</tt> if it is not possible to match the requirements, or an integer representing the length of the almost shortest path found. <br></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
7 9
0 6
0 1 1
0 2 1
0 3 2
0 4 3
1 5 2
2 6 4
3 6 2
4 6 4
5 6 1
4 6
0 2
0 1 1
1 2 1
1 3 1
3 2 1
2 0 3
3 0 2
6 8
0 1
0 1 1
0 2 2
0 3 3
2 5 3
3 4 2
4 1 1
5 1 1
3 0 1
0 0


<strong>Output:</strong>
5
-1
6

</pre>