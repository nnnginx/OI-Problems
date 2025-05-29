<p>A huge aerolite had fallen in Antarctica!!!Many disasters happened and lots of people lost their lives, homes or even everything.Blue Mary, the well-known scientist, is to work out the secret of this aerolite for further study.</p>
<p>Blue Mary has found out that their are some numbers on this aerolite, 5 per line:</p><pre>1 1 1 1 6
0 0 6 3 57
8 0 11 3 2845
</pre>
<p>With her genius, Blue Mary knows that the 5th number is the key to solve the problem, but in some lines the 5th numbers were destoryed and we cannot know what they are instantly.</p>
<p>After some days, she finds out the way to calculate the 5th number finally, which is:</p>
<div align="justify">
    <ul>
        <li>
        A Regular Expression(RE) is a string which only contains characters '{','[','(',')',']','}' and satisfies the rules below.
        </li><li>
        An empty string is an RE.
        </li><li>
        If there's no character '[',']','{','}' in RE A, then (A) is an RE.
        </li><li>
        If there's no character '{','}' in RE A, then [A] is an RE.
        </li><li>
        If A is an RE, {A} is an RE.
        </li><li>
        If both A and B are REs, AB is an RE.
        </li>
    </ul>
</div>
<p>For example "()(())[]", "{()[()]}", "{{[[(())]]}}"(all without quotes) are REs and "()([])()","[()" are not REs.</p>
<p>The deep of an RE A, D(A), is defined as below:</p>
<div align="justify">
    <ul>
        <li>
        If A is an empty string,D(A)=0;
        </li><li>
        If A can be written as BC, D(A)=max(D(B),D(C));
        </li><li>
        If A can be written as (B) or [B] or {B}, D(A)=D(B)+1.
        </li>
    </ul>
</div>
<p>Such as D("(){()}[]")=2.</p>
<p>Suppose the first 4 numbers in current line are L1,L2,L3 and D, then the 5th number in current line is the number of REs modudo 11380.Each of the REs must have a depth of D and is made of L1 {}, L2 [] and L3 ().</p>
<p>Now Mary needs your help to work out the 5th number.</p>
<h3>Input</h3>
<p>Input contains exactly 10 test cases.Each test case contains one line, which contains 4 numbers L1,L2,L3,D(0&lt;=L1,L2,L3&lt;=10, 0&lt;=D&lt;=30), separated by single spaces.</p>
<h3>Output</h3>
<p>Ten lines, each contains a single integer denoted the 5th number.</p>
<h3>Example</h3>
<pre><b>Input:</b>
1 1 1 1
0 0 6 3
1 1 1 2
[and 7 test cases more]

<b>Output:</b>
6
57
8
[and 7 test cases more]
</pre>