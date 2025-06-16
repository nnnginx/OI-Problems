<p>Ada the Ladybug is attending Assertive Club of Mathematicians. On last session, Ada had a fight with her friend Horntail Hansel. Hansel claimed, that if somebody picks a set of binary-vectors of length <strong>K</strong>, he can generate an infinetly long binary vector, which will have none of the smaller vectors as substring. Ada claimed opossite and now she is prepairing a proof, she could pick a set (for any <strong>K</strong>), that every such infinite vector will contain at least one of her vectors as substring. Obviously, it is true, since if she picks all <strong>2<sup>K</sup></strong> vectors, Hansel's vector will always have at least one of such vectors as substring (and even as prefix).</p>
<p>She also wanted to construct such set, to add to importance, but then she realzed <strong>2<sup>K</sup></strong> is too much, so instead she wanted to construct minimal such set. Can you help her to find the size of such set? Even though it might be lesser, it is still pretty big, so output it modulo <strong>10<sup>9</sup>+7</strong></p>
<h3>Input</h3>
<p>The first line of input will contain <strong>1 ¡Ü T ¡Ü 10<sup>6</sup></strong>, the number of test-cases.</p>
<p>&nbsp;</p>
<p>The next <strong>T</strong> lines will contain <strong>1 ¡Ü K ¡Ü 10<sup>7</sup></strong>, the size of binary vectors Ada wants to generate.</p>
<h3>Output</h3>
<p>For each test-case, output the minimum number of binary vectors of length <strong>K</strong> Ada has to generate, so that Hansel can't make an infinite vector which wouldn't have at least one of Ada's vectors as substring. Output this modulo <strong>1000000007</strong>.</p>
<h3>Example Input</h3>
<pre>7
1
2
3
13
666
123456
3141592
</pre>
<h3>Example Output</h3>
<pre>2
3
4
632
595842408
994717838
244191463
</pre>
<h3>Examples of first 3 inputs:</h3>
<pre>0,1
00,01,11
000,001,101,111
</pre>