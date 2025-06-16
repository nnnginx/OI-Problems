<p>Byteazar has decided on going to Mars to tour the space stations  there being in existence. All marsian space stations lie on a  circumference of a circle. Byteazar lands in one of them and then moves  around by means of a special vehicle which is powered by an appropriate  fuel. A litre of this fuel allows him to travel one meter. However, the  provisions of the fuel are meagre, different quantities of it are  available in each space station. Byteazar may refuel in the space  station he is currently in, though he cannot get more fuel than it is  available in that very place (the capacity of his fuel tank is  unlimited). This quantity of fuel should allow him to reach the next  space station. Byteazar has to decide where to land, so that he can  visit all of the space stations. In the end he has to return to the  space station in which he has landed. During his journey Byteazar has to  travel on the circumference of the circle, constantly in one of the two  possible directions.</p>
<h2>Task</h2>
<p>Write a programme which:</p>
<ul>
<li>reads from the standard input the number of space stations,  distances between them and the amount of fuel available in each of them,</li>
<li>for each of the space stations checks, whether Byteazar can land  there i.e. whether by starting in that very station and travelling in a  freely chosen direction he is able to visit all of the space stations  and return to his spaceship,</li>
<li>writes the outcome to the standard output.</li>
</ul>
<h2>Input</h2>
<p>The first line of the standard input contains a single integer <span><img src="file://t56QbbRe.png" alt=""></span> (<span><img src="file://URxTXMxs.png" alt=""></span>). It denotes the number of space stations on Mars. The space stations are numbered from <span><img src="file://hId7rCG3.png" alt=""></span> to <span><img src="file://nqCvZkqA.png" alt=""></span>. In the next <span><img src="file://9O2Voc2p.png" alt=""></span> lines there is a description of all of the stations and the distances between them. The <span><img src="file://Gc0Icmke.png" alt=""></span>'st line contains two integers <span><img src="file://jAyRLO0q.png" alt=""></span> and <span><img src="file://IycxHAEP.png" alt=""></span> (<span><img src="file://2Yy8keLt.png" alt=""></span>, <span><img src="file://0cpe5g7V.png" alt=""></span>). The first one denotes the amount of fuel (in litres) available in the <span><img src="file://V2o8ddCb.png" alt=""></span>'th space station. The other denotes the distance (in metres) between the <span><img src="file://SQ8eWBN6.png" alt=""></span>'th and <span><img src="file://aC5ovfVy.png" alt=""></span>'st space station (obviously <span><img src="file://cvAVcPAY.png" alt=""></span> denotes the distance between the <span><img src="file://BV5yPESB.png" alt=""></span>'th and the <span><img src="file://a2pAGJGj.png" alt=""></span>st  space station). The total amount of available fuel, as well as the sum  of all distances between the space stations does not exceed <span><img src="file://H3q481Q3.png" alt=""></span>.</p>
<h2>Output</h2>
<p>The programme should write <span><img src="file://VAXZm2yJ.png" alt=""></span> lines to the standard output. The <span><img src="file://58sZA4lx.png" alt=""></span>'th line should contain the word <tt>TAK</tt> (i.e. <em>yes</em> is Polish), if Byteazar can land in the <span><img src="file://9AnGA18g.png" alt=""></span>'th space station or <tt>NIE</tt> (i.e. <em>no</em> in Polish) when it is not possible.</p>
<h2>Example</h2>
<p>For the input data:</p>
<pre>5
3 1
1 2
5 2
0 1
5 4</pre>
<p>the correct result is:</p>
<pre>TAK
NIE
TAK
NIE
TAK</pre>