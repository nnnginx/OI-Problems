<p>Texas is the state having the largest number of cows in the US: according to the 2005 report of the NationalAgricultural Statistics Service, the bovine population of Texas is 13.8 million. This is higher than thepopulation of the two runner-up states combined: there are only 6.65 million cows in Kansas and 6.35millions cows in Nebraska. 

</p><p>There are several diseases that can threaten a herd of cows, the most feared being "Mad Cow Disease" or Bovine Spongiform Encephalopathy (BSE); therefore, it is very important to be able to diagnose certain illnesses. Fortunately, there are many tests available that can be used to detect these diseases. 

</p><p>A test is performed as follows. First a blood sample is taken from the cow, then the sample is mixed with a test material. Each test material detects a certain number of diseases. If the test material is mixed with a blood sample having any of these diseases, then a reaction takes place that is easy to observe. However, if a test material can detect several diseases, then we have no way to decide which of these diseases is present in the blood sample as all of them produce the same reaction. There are materials that detect many diseases (such tests can be used to rule out several diseases at once) and there are tests thatdetect only a few diseases (they can be used to make an accurate diagnosis of the problem). 

</p><p>The test materials can be mixed to create new tests. If we have a test material that detects diseases A and B; and there is another test material that detects diseases B and C, then they can be mixed toobtain a test that detects diseases A, B, and C. This means that if we have these two test materials, then there is no need for a test material that tests diseases A, B, and C-such a material can be obtained bymixing these two. 

</p><p>Producing, distributing, and storing many different types of test materials is very expensive, and inmost cases, unnecessary. Your task is to eliminate as many unnecessary test materials as possible. Ithas to be done in such a way that if a test material is eliminated, then it should be possible to mix an equivalent test from the remaining materials. ("Equivalent" means that the mix tests exactly the samediseases as the eliminated material, not more, not less). </p>

<h3>Input</h3>

<p>The input contains several blocks of test cases. Each case begins with a line containing two integers: the number 1 &lt;= n &lt;= 300 of diseases, and the number 1 &lt;= m &lt;= 200 of test materials. The next m lines correspond to the m test materials. Each line begins with an integer, the number 1 &lt;= k &lt;= 300 of diseases that the material can detect. This is followed by k integers describing the k diseases. These integers are between 1 and n . 

</p><p>The input is terminated by a block with n = m = 0 .</p>

<h3>Output</h3>

<p>For each test case, you have to output a line containing a single integer: the maximum number of test materials that can be eliminated. </p>

<h3>Example</h3>
<pre><b>Input:</b>
10 5
2 1 2
2 2 3
3 1 2 3
4 1 2 3 4
1 4
3 7
1 1
1 2 
1 3
2 1 2
2 1 3
2 3 2
3 1 2 3
0 0

<b>Output:</b>
2
4
</pre>
<b>Warning: large input/output data, be careful with certain languages</b>