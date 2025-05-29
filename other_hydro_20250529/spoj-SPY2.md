<p>Blue Mary extremely likes making PPTs. She has already made <strong>L</strong> PPTs. Now the only problem before finish is to set the background pictures for each PPT. She has <strong>N</strong> background pictures, and each PPT needs exactly one background picture. Different PPTs can use same background pictures. Obviously, there are <strong>N<sup>L</sup></strong> combinations.</p>
<p>For each combination, Blue Mary defines its weight as <strong>(k+1)<sup>-1</sup></strong>, where <strong>k</strong> is the number of pictures (from the <strong>N</strong> pictures in total) that do not appear in it. Now Blue Mary wants to calculate the sum of weights of all combinations. (Blue Mary is such a weird girl that she always does some meaningless calculations.) She asks you for help.</p>
<h3>Input</h3>
<p>Multiple test cases, the number of them is less than 500. Each test case consists of a single line with two space-separated integers <strong>N</strong> and <strong>L</strong>. All input numbers are positive and less than 10<sup>6</sup>. Input terminates by EOF.</p>
<p>Input data is almost log-uniform randomly generated.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, output the required value in a single line. It's guaranteed that this number is always an integer for all input data. Since it can be quite large, output it modulo 10<sup>9</sup> +2015. (Why not 10<sup>9</sup>+7? Remember Blue Mary is a weird girl!)</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 2

<strong>Output:</strong>
3
</pre>