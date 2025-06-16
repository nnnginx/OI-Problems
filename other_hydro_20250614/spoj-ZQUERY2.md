<p>Considering a set of segments. At the beginning, the set is totally empty.</p>
<p>There are <strong>N</strong> operations: insert or erase a <em>vertical</em> (or <em>horizontal</em>) segment and then you have to compute how many intersections are there.</p>
<p><em>There is no two same type of segments that share a common point in the set</em>.</p>
<h3>Input</h3>
<p>The first line contains <strong>N</strong> (<strong>1</strong> ¡Ü <strong>N</strong> ¡Ü <strong>10<sup>5</sup></strong>) - the number of operations.</p>
<p>The following <strong>N</strong> lines describe the operations:</p>
<ul>
<li><strong>1 X<sub>1</sub> Y<sub>1</sub> X<sub>2</sub> Y<sub>2</sub></strong>: insert a segment whose two endpoints are <strong>(X<sub>1</sub>, Y<sub>1</sub>)</strong> and <strong>(X<sub>2</sub>, Y<sub>2</sub>)</strong> to the set. (|<strong>X<sub>1</sub></strong>|, |<strong>Y<sub>1</sub></strong>|, |<strong>X<sub>2</sub></strong>|, |<strong>Y<sub>2</sub></strong>| ¡Ü <strong>10<sup>9</sup></strong>)</li>
<li><strong>2 K</strong>: erase the <strong>K-th</strong> oldest segment from the set. (<strong>1</strong> ¡Ü <strong>K</strong> ¡Ü current size of the set)</li>
</ul>
<h3>Output</h3>
<p>For each query, print the number of intersections of the line segments in the set after processing the operation in one line.</p>
<h3>Example</h3>
<pre>  <strong>Input:</strong>
  10
  1 -1 0 -2 0
  1 2 -2 0 -2
  1 1 1 1 -3
  2 1
  1 6 -2 5 -2
  2 3
  1 2 -2 2 -6
  1 -4 -3 -5 -3
  1 3 -4 -1 -4
  2 2
</pre>
<pre>  <strong>Output:</strong>
  0
  0
  1
  1
  1
  1
  2
  2
  3
  2
</pre>
<p><strong>UPD</strong> (1/30/2015): Increase time limit from 2s to 5s. My C++ solution (unoptimized) runs in about 7 seconds.</p>