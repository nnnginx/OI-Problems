<p>It's the year 21546 AD, and due to increased population (you wouldn't believe me if I gave you the actual numbers), land has become very expensive. Because of the lack of space, Heaven and Hell were built in the same area. The area can be represented as a grid of <b>X</b> �� <b>Y</b> unit squares. Some of the squares were captured by the Devil (and thus belong to Hell) and the rest is the Almighty's property.  On each square, a room has been built with transparent glass walls.  However, some of the heavenly rooms are already occupied by Angels.  For security purposes, rooms occupied by Angels have concrete opaque walls.</p>

<p>Recently many fighters were killed in a tournament. Fighting is no longer considered cruel, so all the fighters will deserve spots in heaven. However, because of the space shortage, all of them may not be able to recieve a spot in heaven.  The fighters still hold a grudge against each other so a fighter cannot be placed in a room from which he can see any other fighter.  A fighter can only see in the four cardinal directions (North, South, East and West).  He cannot look diagonally or in any other direction.</p>

<p>Find the maximum number of fighters who can have a heavenly room.</p>

<h3>Input</h3>
<p>The first line of the input contains an integer <b>t</b>, the number of test cases.  <b>t</b> test cases follow.</p>

<p>The first line of each test case consists of two integers <b>X</b> &lt;= 300 and <b>Y</b> &lt;= 300, separated by a single space.  Next, <b>X</b> lines follow, each having <b>Y</b> letters separated by spaces.  The jth letter on the i-th line is one of the following (quotes are for clarity, and do not appear in the input):</p>
<ol>
<li>"H", if the room at location (i, j) is heavenly and vacant.</li>
<li>"A", if the room at location (i, j) is heavenly and is already occupied by an angel.  Note that these rooms are not transparent.</li>
<li>"D", if the room at location (i, j) belongs to the Devil.</li>
</ol>

<b>Output</b>
<p>A single line for each test case containing an integer denoting the maximum number of fighters that can fit in heaven.</p>

<h3>Example</h3>

<pre><b>Input:</b>
1
4 7
H H H H H H H
H H H H H H H
H H H H H H H
H H H H H H H

<b>Output:</b>
4
</pre>