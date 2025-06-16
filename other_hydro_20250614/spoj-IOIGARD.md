<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Byteman owns the most beautiful garden in Bytetown. He planted n roses in his garden. Summer has come</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">and the flowers have grown big and beautiful. Byteman has realized that he is not able to take care of all the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">roses on his own. He has decided to employ two gardeners to help him. He wants to select two rectangular</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">areas, so that each of the gardeners will take care of the roses inside one area. The areas should be disjoint</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">and each should contain exactly k roses.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Byteman wants to make a fence surrounding the rectangular areas, but he is short of money, so he wants</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">to use as little fence as possible. Your task is to help Byteman select the two rectangular areas.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The garden forms a rectangle l meters long and w meters wide. It is divided into l · w squares of size</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 meter × 1 meter each. We fix a coordinate system with axes parallel to the sides of the garden. All squares</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">have integer coordinates (x,y) satisfying 1  x  l, 1  y w. Each square may contain any number of roses.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The rectangular areas, which must be selected, should have their sides parallel to the sides of the garden</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">and the squares in their corners should have integer coordinates. For 1  l1  l2  l and 1  w1  w2  w, a</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">rectangular area with corners (l1,w1), (l1,w2), (l2,w1) and (l2,w2):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">• contains all the squares with coordinates (x,y) satisfying l1  x  l2 and w1  y  w2, and</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">• has perimeter 2 · (l2−l1+1)+2 · (w2−w1+1).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The two rectangular areas must be disjoint, that is they cannot contain a common square. Even if they have a</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">common side, or part of it, they must be surrounded by separate fences.</div>
<p>&nbsp;</p>
<p>Byteman owns the most beautiful garden in Bytetown. He planted n roses in his garden. Summer has come&nbsp;and the flowers have grown big and beautiful. Byteman has realized that he is not able to take care of all the&nbsp;roses on his own. He has decided to employ two gardeners to help him. He wants to select two rectangular&nbsp;areas, so that each of the gardeners will take care of the roses inside one area. The areas should be disjoint&nbsp;and each should contain exactly k roses.&nbsp;Byteman wants to make a fence surrounding the rectangular areas, but he is short of money, so he wants&nbsp;to use as little fence as possible. Your task is to help Byteman select the two rectangular areas.</p>
<p>The garden forms a rectangle l meters long and w meters wide. It is divided into l · w squares of size&nbsp;1 meter × 1 meter each. We fix a coordinate system with axes parallel to the sides of the garden. All squares&nbsp;have integer coordinates (x,y) satisfying 1&lt;=x&lt;=l, 1&lt;=y&lt;=w. Each square may contain any number of roses.&nbsp;The rectangular areas, which must be selected, should have their sides parallel to the sides of the garden&nbsp;and the squares in their corners should have integer coordinates. For 1&lt;=l1&lt;=l2&lt;=l and 1&lt;=w1&lt;=w2&lt;=w, a&nbsp;rectangular area with corners (l1,w1), (l1,w2), (l2,w1) and (l2,w2):</p>
<p>• contains all the squares with coordinates (x,y) satisfying l1&lt;=x&lt;=l2 and w1&lt;=y&lt;=w2, and</p>
<p>• has perimeter 2 · (l2−l1+1)+2 · (w2−w1+1).</p>
<p>The two rectangular areas must be disjoint, that is they cannot contain a common square. Even if they have a&nbsp;common side, or part of it, they must be surrounded by separate fences.</p>
<p style="text-align: center;"><span style="font-size: x-small;"><strong><span style="font-size: small;">Task</span></strong></span></p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3 style="text-align: left;"><span style="font-size: small;"><span style="font-size: x-small;"><span style="font-weight: normal;"><span style="font-size: small;">Write a program, that:</span></span></span></span></h3>
<h3 style="text-align: left;"><span style="font-size: small;"><span style="font-size: x-small;"><span style="font-weight: normal;"><span style="font-size: small;">• reads from the standard input the dimensions of the garden, the number of roses in the garden, the&nbsp;</span></span></span></span><span style="font-weight: normal; font-size: small;">number of roses that should be in each of the rectangular areas, and the positions of the roses.</span></h3>
<h3 style="text-align: left;"><span style="font-size: small;"><span style="font-size: x-small;"><span style="font-weight: normal;"><span style="font-size: small;">• finds the corners of two such rectangular areas with minimum sum of perimeters that satisfy the given&nbsp;</span></span></span></span><span style="font-weight: normal; font-size: small;">conditions.</span></h3>
<h3 style="text-align: left;"><span style="font-size: small;"><span style="font-size: x-small;"><span style="font-weight: normal;"><span style="font-size: small;">• writes to the standard output the minimumsum of perimeters of two non-overlapping rectangular areas,&nbsp;</span></span></span></span><span style="font-weight: normal; font-size: small;">each containing exactly the given number of roses (or a single word NO, if no such pair of areas exists).</span></h3>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The first line of standard input contains two integers: l and w (1&lt;=l,w&lt;=250) separated by a single space&nbsp;— the length and the width of the garden. The second line contains two integers: n and k (2&lt;=n&lt;=5000,&nbsp;1&lt;=k&lt;=n/2) separated by a single space — the number of roses in the garden and the number of roses that&nbsp;should be in each of the rectangular areas. The following n lines contain the coordinates of the roses, one rose&nbsp;per line. The (i+2)-nd line contains two integers li, wi (1&lt;=li&lt;=l, 1&lt;=wi&lt;=w) separated by a single space&nbsp;— the coordinates of the square containing the i-th rose. Two or more roses can occur in the same square.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>The standard output should contain only one line with exactly one integer—the minimum sum of perimeters&nbsp;of two non-overlapping rectangular areas, each containing exactly k roses, or a single word NO, if no such pair&nbsp;of areas exists.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6 5
7 3
3 4
3 3
6 1
1 1
5 5
5 5
3 1

<strong>Output:</strong>
22</pre>