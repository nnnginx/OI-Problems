<p><span style="font-weight: bold;">[Due to SPOJ restrictions, this problem has been modified with respect to the original version used in the Argentinian Programming Tournament of 2015 in order to have multiple test cases per input file. The original version of this problem (in Spanish) can be found at </span><a style="font-weight: bold;" href="http://torneoprogramacion.com.ar/wp-content/uploads/2015/09/pruebaTAP2015.pdf">http://torneoprogramacion.com.ar/wp-content/uploads/2015/09/pruebaTAP2015.pdf</a><span style="font-weight: bold;"> ]</span></p>
<p>Hugo goes to primary school, but he is convinced that not enough homework is being given to him. Specifically, he was recently taught how to subtract two numbers, but each day he is given a single subtraction to perform at home. Hugo knows that in order to master such a complex technique he should practice much more, so he has decided to take matters into his own hands and create his own homework.</p>
<p>It's not easy for Hugo to invent exercises about a subject he does not fully comprehend, so he has devised the following method to perform multiple subtractions. He starts by asking his mother for a number <strong>N</strong>, and then forms the number <strong>M</strong> containing the same digits as <strong>N</strong> in increasing order from left to right, after which he finally performs the subtraction <strong>N-M</strong>. For example, if his mother chooses the number <strong>N = 321</strong> then <strong>M = 123</strong> and the subtraction Hugo must perform is <strong>N - M = 321-123 = 198</strong>.</p>
<p>Hugo wouldn't want to bother his mother too often, so he will repeat this procedure using the result of the subtraction <strong>N-M</strong> in one step as the number <strong>N</strong> he starts with in the next step. This will end only when at some point he reaches the value <strong>N = 0</strong>, as this case is useless to practice subtractions because he would have <strong>M = 0</strong>: Hugo already knows perfectly well that if he has no candies he cannot eat any candies, and will therefore continue to not have or eat candies forever.</p>
<p>Now Hugo's mother would like to know, given a number <strong>N</strong>, how many subtractions Hugo can perform if she gives him that number to start his homework. In the previous example, in the second step Hugo would have <strong>N = 198</strong> so that <strong>M = 189</strong> and <strong>N - M = 198 - 189 = 9</strong>. Then in the third step <strong>N = 9</strong>, <strong>M = 9</strong> and <strong>N - M = 0</strong>, so here the fun ends because in the fourth step he would have <strong>N = 0</strong>. Thus, starting with the number <strong>N = 321</strong> Hugo will perform <strong>3</strong> subtractions.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>There are multiple test cases in the input file. Each test case consists of one line containing an integer <strong>N</strong>, representing the number Hugo's mother will give him to start his homework (<strong>1 ¡Ü N ¡Ü 10<sup>9</sup></strong>).</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print one line containing one integer representing the number of subtractions Hugo will perform if he starts his homework with number <strong>N</strong>.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">321
20
960687301</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">3
2
91</span></pre>