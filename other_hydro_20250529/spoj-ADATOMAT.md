<p>Ada the Ladybug grows tomatoes. She has a very long furrow full of them. At
the day of harvest, she picks all tomatoes, <b>sorts</b> them by size, index them
(from 1) and sell them for price of "<b>size ¡Á index</b>". How much money will she make, if she sells all of them?



</p><p>As the nature is very beautiful (and Ada is great mathematician), she found
the pattern for sizes of tomatoes. The patern works in (hopefully well known)
way: Let us have tomato of size <b>X<sub>i</sub></b>, then
<b>X<sub>i+1</sub></b> will be counted as  <b>X<sub>i+1</sub>=X<sub>i</sub>*a+b
    mod M</b>. <b>M</b> (modulo) is equal to
<b>10<sup>9</sup>+7</b> (1000000007).



</p><h3>Input</h3>

The first line contains <b>1 ¡Ü T ¡Ü 200</b>, the number of test-cases.

<p>Each test-case contains four numbers <b>N, a, b, X<sub>1</sub></b>:

</p><p> <b>1 ¡Ü N ¡Ü 2*10<sup>7</sup></b>, the number of tomatoes.

</p><p> <b>0 ¡Ü a, b, X<sub>1</sub> &lt; 10<sup>9</sup>+7 </b> - described above
(X<sub>1</sub> is the size of first tomato).

</p><p>Sum of <b>N</b> over all test-cases will not exceed <b>5*10<sup>7</sup></b>.

</p><h3>Output</h3>
For each test-case output the sum of all prices modulo <b>10<sup>9</sup>+7</b>.

<h3>Example Input</h3>
<pre>5 
2 2 3 1
3 1 1 1
5 1 2 1
4 1 0 1
20 5 6 7
</pre>
<h3>Example Output</h3>
<pre>11
14
95
10
150690584
</pre>
<h3>Sizes of tomatoes for each input</h3>
<pre>1 5
1 2 3
1 3 5 7 9
1 1 1 1
7 41 211 1061 5311 26561 132811 664061 3320311 16601561 75195297 83007811 375976491 399412248 415039061 632654193 879882454 926530843 985306173 997061239
</pre>