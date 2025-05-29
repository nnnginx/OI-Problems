<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Question E - New Horizons</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">I’m king of a house! And, what’s more, beyond that,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">I’m king of a blueberry bush and a cat!</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">I’m Yertle the Turtle! Oh, marvelous me!</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For I am the ruler of all that I see!"</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Yertle has determined that the number of objects he can see, and hence rule, depends on the height of his throne. Your task, as Minister of Computing and Vertigo (a new combined Super Ministry), is to determine which objects Yertle would see should he build his throne to a particular height.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Standard input consists of:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"> A floating point number on a line by itself, specifying the diameter of Yertle’s planet in "flipper lengths".</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"> A line containing three floating point numbers: the height of Yertle’s throne (in flipper lengths), the latitude of Yertle’s throne (between -90 and +90 degrees), the longitude of Yertle’s throne (between 0 and 360 degrees).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"> Several lines, each containing three floating point numbers and a string of alphabetic and space characters. Each line indicates the height, latitude, longitude and name of an object on the surface of Yertle’s planet. The last line is indicated by the end of standard input.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">All distances are in flipper lengths, and all latitudes and longitudes are in degrees. Floating point values are formatted as a string of decimal digits with an optional decimal point and sign. The fields in the input are separated by exactly one space character. You may assume that no object hides another; only the horizon limits Yertle’s view.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Standard output consists of the list of objects whose tops are visible to Yertle, in alphabetical order.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Example Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">20000.0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">100.0 45.0 100.0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2.0 46.0 99.0 Cat</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">20.0 -45.0 260.0 House</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">5.0 45.1 100.2 Blueberry Bush</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Example Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Blueberry Bush</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Cat</div>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><em>I’m king of a house! And, what’s more, beyond that,</em></p>
<p><em>I’m king of a blueberry bush and a cat!</em></p>
<p><em>I’m Yertle the Turtle! Oh, marvelous me!</em></p>
<p><em>For I am the ruler of all that I see!"</em></p>
<p>Yertle has determined that the number of objects he can see, and hence rule, depends on the height of his throne. Your task, as Minister of Computing and Vertigo (a new combined Super Ministry), is to determine which objects Yertle would see should he build his throne to a particular height.</p>
<p><strong>Input:</strong></p>
<p>Standard input consists of:</p>
<p> A floating point number on a line by itself, specifying the diameter of Yertle’s planet in "flipper lengths".</p>
<p> A line containing three floating point numbers: the height of Yertle’s throne (in flipper lengths), the latitude of Yertle’s throne (between -90 and +90 degrees), the longitude of Yertle’s throne (between 0 and 360 degrees).</p>
<p> Several lines, each containing three floating point numbers and a string of alphabetic and space characters. Each line indicates the height, latitude, longitude and name of an object on the surface of Yertle’s planet. The last line is indicated by the end of standard input.</p>
<p>All distances are in flipper lengths, and all latitudes and longitudes are in degrees. Floating point values are formatted as a string of decimal digits with an optional decimal point and sign. The fields in the input are separated by exactly one space character. You may assume that no object hides another; only the horizon limits Yertle’s view.</p>
<p><strong>Output:</strong></p>
<p>Standard output consists of the list of objects whose tops are visible to Yertle, in alphabetical order.</p>
<p><strong>Example Input:</strong></p>
<p>20000.0</p>
<p>100.0 45.0 100.0</p>
<p>2.0 46.0 99.0 Cat</p>
<p>20.0 -45.0 260.0 House</p>
<p>5.0 45.1 100.2 Blueberry Bush</p>
<p><strong>Example Output:</strong></p>
<p>Blueberry Bush</p>
<p>Cat</p>
<p>&nbsp;</p>
<p>&nbsp;</p>