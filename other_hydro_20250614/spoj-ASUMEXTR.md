<p>f(n) is defined as: f(n) = 1<sup>k</sup>+2<sup>k</sup>+3<sup>k</sup>+...+n<sup>k</sup>, so it is the sum of the k-th power of all natural numbers up to n.</p>
<p>In this problem you are about to compute,</p>
<p>f(1) + f(2) + f(3) + ... + f(n)</p>
<p><strong>Note</strong>: This is a harder version of the problem&nbsp;<a href="../ASUMHARD/" target="_blank">ASUMHARD</a>, with larger constraints. Please read the constraints section carefully.</p>
<h3>Input</h3>
<p>The first line is an integer <strong>T</strong>, denoting the number of test cases. Then, <strong>T</strong> test cases follow.</p>
<p>For each test case, there are two integers <strong>n</strong> and <strong>k</strong> written in one line, separated by space.</p>
<h3>Output</h3>
<p>For each test case, output the result of the summatory function described above.</p>
<p>Since this number could be very large, output the answer modulo <strong>1,234,567,891</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
2 3
10 3
3 3
100 0
100 1

<strong>Output:</strong>
10
7942
46
5050
171700</pre>
<h3>Explanation</h3>
<p>In case 1, <strong>n</strong> = 2, <strong>k</strong> = 3. f(1) = 1<sup>3</sup>, f(2) = 1<sup>3</sup>+2<sup>3</sup>. <strong>ans</strong> = f(1) + f(2) = 10.</p>
<h3>Constraints</h3>
<p>Overall constraints</p>
<ul>
<li>5 ¡Ü <strong>T</strong> ¡Ü 500000</li>
<li>1 ¡Ü <strong>n</strong> ¡Ü 10<sup>18</sup></li>
<li>0 ¡Ü <strong>k</strong> ¡Ü 10000000</li>
</ul>
<p>More precise information (there are 6 test files):</p>
<p>Test #0: <strong>T</strong>&nbsp;= 500000, 0 ¡Ü <strong>k</strong> ¡Ü 100</p>
<p>Test #1: <strong>T</strong>&nbsp;= 50000, 0 ¡Ü <strong>k</strong> ¡Ü 1000</p>
<p>Test #2: <strong>T</strong> = 5000, 0 ¡Ü <strong>k</strong> ¡Ü 10000</p>
<p>Test #3: <strong>T</strong> = 500, 0 ¡Ü <strong>k</strong> ¡Ü 100000</p>
<p>Test #4:&nbsp;<strong>T</strong> = 50, 0 ¡Ü <strong>k</strong> ¡Ü 1000000</p>
<p>Test #5: <strong>T</strong> = 5, 0 ¡Ü <strong>k</strong> ¡Ü 10000000</p>
<p>It should be clear from the constraints that an <strong>O(k<sup>2</sup>)</strong> solution <strong>will</strong> <strong>not pass</strong>. Inputs are generated uniformly randomly in the given ranges (with some manual worst case inputs). Time limit is set to 2x of my unoptimized C++ code.</p>