<h3>Description</h3>
<p><i>According to Wikipedia, image processing is any form of signal processing for which the input is an image, such as photographs or frames of video; the output of image processing can be either an image or a set of characteristics or parameters related to the image. Most image-processing techniques involve treating the image as a two-dimensional signal and applying standard signal-processing techniques to it. </i></p>
<p>The task you are facing here is a relatively easy one (compared to our general conception of image processing!). Given a black-and-white image of size R * C with some digits (and possibly other shapes) on it, your program needs to figure out the digits written on the image. Specifically, the digits drawn on the graph will adhere to the following rules:
</p><p>1) Digits are drawn with a series of <i>strokes</i>. A <b>stroke</b> can be regarded as a <b>rectangle</b> of any size on the image, and its edges will always be parallel to either <b>x-axis</b> or <b>y-axis</b>. The number of strokes required to draw each digit will be exactly as follows:</p>
<pre>0 	1 	2 	3 	4 	5 	6 	7 	8 	9
4 	1 	5 	4 	3 	5 	5 	2 	5 	5
</pre>
<p>Refer to the <b>figure below</b> if you are unclear about how the digits are drawn.</p>
<p>2) Although the <b>width</b> of strokes used to draw a digit might be <b>different</b>, the <b>outer shapes of digits</b> will strictly follow those specified in the <b>figure below</b>. 
</p><p>3) In order for a digit to be recognizable, <b>all</b> parts (<b>strokes</b> and <b>joints</b>) presented in the graph below must also be clearly <b>distinguishable</b> in the image. 
</p><p><i>(Refer to the last sample test case if you are unsure about this requirement; in that test case, when the middle stroke of 2 is omitted, the number should not be considered as recognizable.)</i> 
</p><p>4) You may assume that the image is not rotated, and there is <b>no noise</b> in the input.</p>
<img src="/content/john_jones:imgrec2.jpg">
<p>Please output the sum of digits recognizable in the graph. In the case that no characters is recognizable, please output 0 instead.</p>
<h3>Input</h3>
<p>There are multiple test cases in the input file. 
</p><p>Each test case starts with two integers, R and C (1 &lt;= R,C &lt;= 500), specifying the number of rows / columns of the graph. Each of the following R lines contains consecutive C characters ("0" or "1"), describing the image to be processed. 
</p><p>Two successive test cases are separated by a blank line. A case with R = 0, C = 0 indicates the end of the input file, and should not be processed by your program. </p>
<h3>Output</h3>
<p>For each test case, please print a single integer, the sum of recognizable numbers. See the sample output for format details.</p>
<h3>Example</h3>
<pre><b>Input:</b>
5 12
001101011111
000101000011
000101001111
001101000011
000000000111

5 3
111
010
110
010
110

6 14
11111000011111
11001000000011
11111001000000
11111001001110
11001011001010
11111000001110

5 2
11
01
11
01
11

6 9
111100111
000100001
000100011
011100010
010000011
011110000

0 0

<b>Output:</b>
Case #1: 4
Case #2: 0
Case #3: 15
Case #4: 3
Case #5: 2
</pre>