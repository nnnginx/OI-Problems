<p style="text-align: center;"><strong>Alphabetomials</strong></p>
<p>As we all know, there is a big difference between polynomials of degree 4 and those of degree 5. The question of the non-existence of a closed formula for the roots of general degree 5 polynomials produced the famous Galois theory, which, as far as the author sees, bears no relation to our problem here.</p>
<p>We consider only the multi-variable polynomials of degree up to 4, over 26 variables, represented by the set of 26 lowercase English letters. Here is one such polynomial:</p>
<pre>aber+aab+c<br></pre>
<p>Given a string <em>s</em>, we evaluate the polynomial on it. The evaluation gives <em>p</em>(<em>S</em>) as follows: Each variable is substituted with the number of appearances of that letter in <em>S</em>.<br> For example, take the polynomial above, and let <em>S</em> = "abracadabra edgar". There are six a's, two b's, one c, one e, and three r's. So</p>
<pre>p(S) = 6 * 2 * 1 * 3 + 6 * 6 * 2 + 1 = 109.<br></pre>
<p>Given a dictionary of distinct words that consist of only lower case letters, we call a string <em>S</em> a <em>d-phrase</em> if</p>
<pre>S = "S<sub>1</sub> S<sub>2</sub> S<sub>3</sub> ... S<sub>d</sub>",<br></pre>
<p>where S<sub>i</sub> is any word in the dictionary, for 1 ¡Ü i ¡Ü d. i.e., <em>S</em> is in the form of <em>d</em> dictionary words separated with spaces. Given a number <strong>K</strong> ¡Ü 10, your task is, for each 1¡Ü <em>d</em> ¡Ü <strong>K</strong>, to compute the sum of <em>p</em>(<em>S</em>) over all the <em>d</em>-phrases. Since the answers might be big, you are asked to compute the remainder when the answer is divided by 10009.</p>
<p>Input</p>
<p>The first line contains the number of cases <strong>T</strong>. <strong>T</strong> test cases follow. The format of each test case is:<br> A line containing an expression <em>p</em> for the multi-variable polynomial, as described below in this section, then a space, then follows an integer <strong>K</strong>.<br> A line with an integer <strong>n</strong>, the number of words in the dictionary.<br> Then <strong>n</strong> lines, each with a word, consists of only lower case letters. No word will be repeated in the same test case.</p>
<p>We always write a polynomial in the form of a sum of terms; each term is a product of variables. We write <em>a</em><sup>t</sup> simply as <em>t</em> <em>a</em>'s concatenated together. For example, <em>a</em><sup>2</sup><em>b</em> is written as <em>aab</em>. Variables in each term are always lexicographically non-decreasing.</p>
<p>Output</p>
<p>For each test case, output a single line in the form</p>
<pre>Case #X: sum<sub>1</sub> sum<sub>2</sub> ... sum<sub>K</sub><br></pre>
<p>where <em>X</em> is the case number starting from 1, and sum<sub>i</sub> is the sum of <em>p</em>(<em>S</em>), where <em>S</em> ranges over all i-phrases, modulo 10009.</p>
<p>Limits</p>
<p>1 ¡Ü <strong>T</strong> ¡Ü 100.<br> The string <em>p</em> consists of one or more terms joined by '+'. It will not start nor end with a '+'. There will be at most 5 terms for each <em>p</em>. Each term consists at least 1 and at most 4 lower case letters, sorted in non-decreasing order. No two terms in the same polynomial will be the same.<br> Each word is non-empty, consists only of lower case English letters, and will not be longer than 50 characters. No word will be repeated in the same dictionary.</p>
<p>Small dataset</p>
<p>1 ¡Ü <strong>n</strong> ¡Ü 20<br> 1 ¡Ü <strong>K</strong> ¡Ü 5</p>
<p>Large dataset</p>
<p>1 ¡Ü <strong>n</strong> ¡Ü 100<br> 1 ¡Ü <strong>K</strong> ¡Ü 10</p>
<p>Sample</p>
<table style="width: 357px; height: 238px;" border="0">
<tbody>
<tr>
<td><br> <span>Input</span> <br>&nbsp;</td>
<td><br> <span>Output</span> <br>&nbsp;</td>
</tr>
<tr>
<td><code> 2<br> ehw+hwww 5<br> 6<br> where<br> when<br> what<br> whether<br> who<br> whose<br> a+e+i+o+u 3<br> 4<br> apple<br> orange<br> watermelon<br> banana<br> <br> </code></td>
<td valign="top"><code> Case #1: 15 1032 7522 6864 253<br> Case #2: 12 96 576<br> </code></td>
</tr>
</tbody>
</table>