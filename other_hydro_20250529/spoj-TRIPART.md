<p>
A triangle can be divided into two equal triangles by drawing a median on its largest edge (in the figure below such a division is shown with the red line). Then the smaller two triangles can be divided in similar fashion into equal triangles (shown in the picture below with blue lines). This process can continue forever.
</p>
<img src="/content/thanhvy:tripart.jpg">
<p>
Some mathematicians have found that when we split a triangle into smaller ones using the method specified above we have only some "styles" of triangles that only differ in size. So now given the lengths of the sides of the triangle your job is to find out how many different styles of small triangles we have. (Two triangles are of same style if they are similar.)
</p>

<h3>Input</h3>
<p>
First line of the input file contains an integer <i>N (0 &lt; N &lt; 35)</i> that indicates how many lines of input there are.
</p>
<p>
Each line contains three integers <i>a, b, c (0 &lt; a,b,c &lt; 100)</i> which indicate the sides of a valid triangle. (A valid triangle means a real triangle with positive area.)
</p>

<h3>Output</h3>
<p>
For each line of input you should produce an integer <i>T</i>, which indicates the number of different styles of small triangles, formed for the triangle at input. Look at the example for details. You can safely assume that for any triangle <i>T</i> will be less than <i>100</i>.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
3 4 5
12 84 90

<b>Output:</b>
3
41
</pre>