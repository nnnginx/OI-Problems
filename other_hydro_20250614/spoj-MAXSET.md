<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">Krish is teaching Ram Bubble sort .whenever kirsh swaps two elements in the array (while sorting),he ties a rope that connects both the element in the array.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">find the size of the maximal set in the array in which none of the elements are connected with any other element .</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">eg : { 1 , 3 ,2 }</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">1st iteration of bubble sort :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">2 and 3 swapped so tie 2 with 3&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">{1 ,2,3}</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">2nd iteration&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">{1,2,3}</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">3rd iteration&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">{1,2,3}</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">now ans is 2 .since size of &nbsp;the maximal set &nbsp;in which none of the elements is not connected with any other element.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">the possible maximal sets are {1,2} (since 1 and 2 are not tied with a rope) and {1,3} &nbsp;{ since 1 and 3 are not tied with the rope }</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">Input :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">First line of input contains T &nbsp;- No of test cases&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">first line of each test case contains n ( 1 &lt;= n &lt;= 100000 )- number of elements in the array&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">second line &nbsp;of each test case contains n elements of the array&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">output :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">print the size of the maximal set ( for each test case print a 1new line )&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">example:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">1 3 2&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">output :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow: hidden;">2</div>
<p>Ram and Sharav are good programmers &nbsp;.Ram is teaching Sharav Bubble sort .whenever Ram swaps two elements in the array (while sorting),he ties a rope between the element which are swapped.</p>
<p>find the size of the maximal set in the array in which none of the elements are connected with any other element after the bubble sort is done .</p>
<p>eg : { 1 , 3 ,2 }</p>
<p>&nbsp;</p>
<p>1st iteration of bubble sort :</p>
<p>2 and 3 swapped so tie 2 with 3&nbsp;</p>
<p>{1 ,2,3}</p>
<p>2nd iteration&nbsp;</p>
<p>{1,2,3}<br>no swaps in this iteration so dont tie any element with any other element&nbsp;</p>
<p>3rd iteration&nbsp;</p>
<p>{1,2,3}<br>no swaps in this iteration so dont tie any element with any other element&nbsp;&nbsp;</p>
<p>after the end of bubble sort only 2 and 3 are tied together&nbsp;</p>
<p>Answer for this example is 2 because the size of &nbsp;the maximal set &nbsp;in which none of the elements is not tied with any other element.</p>
<p>the possible maximal sets are {1,2} (since 1 and 2 are not tied with a rope) and {1,3} &nbsp;{ since 1 and 3 are not tied with the rope }</p>
<p>Possible subsets for this array are {1} , {2}, {3} ,{1,2} ,{1,3} ,{3,2} {1,3,2},{ }</p>
<p>out of these valid subsets are {1},{2},{3},{1,2},{1,3} In this valid subsets {1,2} and {1,3} are larger subsets .The size of both the subsets are 2 .so the answer is 2.</p>
<p>Input :</p>
<p>First line of input contains T &nbsp;- No of test cases&nbsp;</p>
<p>first line of each test case contains n ( 1 &lt;= n &lt;= 100000 )- number of elements in the array&nbsp;</p>
<p>second line &nbsp;of each test case contains n elements of the array&nbsp;</p>
<p>&nbsp;</p>
<p>output :</p>
<p>print the size of the maximal set ( for each test case print a 1new line )&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>example:</p>
<p>input : (from the example explained above )</p>
<p>1</p>
<p>3</p>
<p>1 3 2&nbsp;</p>
<p>&nbsp;</p>
<p>output :</p>
<p>2</p>
<p>Note : ropes are tied between two elements which are swapped while &nbsp;executing the sort routine. (bubble sort) .we need the size of the set containing the maximum number of elements which are not connected to any other element in the set .</p>