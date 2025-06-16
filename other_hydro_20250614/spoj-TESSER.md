<p>Dr. Bruce Banner had estimated a coarse location of Tesseract through  gamma radiation emission tracing experiment. It was estimated that  Tesseract was hidden somewhere within the Alps mountains. Captain  America was given the assignment to look for the Tesseract and bring it  back to S.H.I.E.L.D. While roaming through the mountains of Alps,  Captain America looked at the height of hills and clicked a panoramic  photograph of mountains. This gives an idea of the heights of mountains.  Meanwhile Banner was able to determine a continuous pattern of  mountains behind which the Tesseract lies and transmitted a message  containing the pattern.</p>
<p>The message is a string consisting of characters <strong>'G' , 'L'</strong> and <strong>'E'</strong> where <strong>G</strong> means greater,<strong> L</strong> means less and <strong>E</strong> means equal. But this estimation is likely to go wrong due to not  considering environmental disturbances that may have arisen in the  medium during the experiment.</p>
<p>Pattern estimate is correct only if one can find a set of consecutive heights out of the given <strong>N</strong> heights satisfying the message pattern (if <strong>G</strong> is first character of the message string then second height should be  greater than the first height of the selected set and so on) Captain  America seeks your help to find out whether the estimation is correct or  wrong so that Captain America could proceed his tasks.</p>
<h3>Input</h3>
<p>The first line of the input contains an integer <strong>T</strong> denoting the number of test cases. Each test case consists of 3 lines. The first line of each test case contains a single integer <strong>N</strong> denoting the number of hills. Second line of each test case consists of <strong>N</strong> integers <strong>(a_1,a_2....a_n)</strong>, the heights of hills. Third line contains the message pattern.</p>
<ul>
<li><strong>1</strong> ¡Ü <strong>T</strong> ¡Ü <strong>10<sup>5</sup></strong></li>
<li><strong>2</strong> ¡Ü <strong>N</strong> ¡Ü <strong>10<sup>5</sup></strong></li>
<li><strong>1</strong> ¡Ü <strong>a_i</strong> ¡Ü <strong>10<sup>9</sup></strong></li>
<li><strong>1</strong> ¡Ü <strong>Length of Message Pattern</strong> ¡Ü <strong>N-1</strong></li>
</ul>
<h3>Output</h3>
<p>For each test case print <strong>'YES'</strong> if the pattern estimation is correct. Else print <strong>'NO'.</strong></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
5
1 2 3 4 1
GGL

<strong>Output:</strong>
YES</pre>
<p>&nbsp;</p>
<h3>Explanation</h3>
<p>Answer is "YES", because 2 3 4 1 satisfies GGL pattern, i.e. 3 is greater than 2, 4 is greater than 3, 1 is less than 4.</p>