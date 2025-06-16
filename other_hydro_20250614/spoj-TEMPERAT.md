<p>The Byteotian Institute of Meteorology (BIM) measures the air temperature     daily.     The measurement is done automatically, and its result immediately printed.     Unfortunately, the ink in the printer has long dried out...     The employees of BIM however realised the fact only recently, when the     Byteotian Organisation for Meteorology (BOM) requested access to that data.</p>
<p>An eager intern by the name of Byteasar saved the day, as he systematically     noted down the temperatures reported by two domestic alcohol thermometers     placed on the north and south outside wall of the BIM building.     It was established decades ago by various BIM employees that the temperature     reported by the thermometer on the south wall of the building is never lower     than the actual temperature, while that reported by the thermometer on the     north wall of the building is never higher than the actual temperature.     Thus even though the exact temperatures for each day remain somewhat of     a mystery, the range they were in is known at least.</p>
<p>Fortunately for everyone involved (except Byteasar and you, perhaps),     BOM does not require exact temperatures. They only want to know the longest     period in which the temperature was not dropping (i.e. on each successive     day it was no smaller than on the day before).     In fact, the veteran head of BIM knows very well that BOM would like this     period as long as possible.     To whitewash the negligence he insists that Byteasar determines, based on     his valuable notes, the longest period in which the temperature     <strong>could have been</strong> not dropping.     Now this is a task that Byteasar did not quite expect on his BIM internship,     and he honestly has no idea how to tackle it.     He asks you for help in writing a program that determines the longest such     period.</p>
<h2>Input</h2>
<p>In the first line of the standard input there is one integer <span><img src="./24638/file/SAyiQOuT.png" alt=""></span> (<span><img src="./24638/file/yMKOadZr.png" alt=""></span>) that denotes the number of days for which       Byteasar took notes on the temperature.       The measurements from day <span><img src="./24638/file/Ft3xfuHP.png" alt=""></span> are given in the line no. <span><img src="./24638/file/ZIOvxKUA.png" alt=""></span>.       Each of those lines holds two integers, <span><img src="./24638/file/Ti91HtIV.png" alt=""></span> and <span><img src="./24638/file/fFUjqZUl.png" alt=""></span> (<span><img src="./24638/file/z5E1D0rT.png" alt=""></span>).       These denote, respectively, the minimum and maximum possible temperature       on that particular day, as reported by the two thermometers.</p>
<h2>Output</h2>
<p>In the first and only line of the standard output your program should       print a single integer, namely the maximum number of days for which the       temperature in Byteotia could have been not dropping.</p>
<h2>Example</h2>
<p>For the input data:</p>
<pre>6
6 10
1 5
4 8
2 5
6 8
3 5</pre>
<p>the correct result is:</p>
<pre>4</pre>
<p><img src="./24638/file/kunW00Us.png" alt=""></p>