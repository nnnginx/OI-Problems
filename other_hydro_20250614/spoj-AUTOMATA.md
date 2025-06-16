<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Bob is playing Hide and Seek with alphabets and he is amazed by the properties of '?' and '*' in the language. He is given a language 'L'. He has to check whether the given string 'S' is present in the language 'L'. He needs your help. Print "Yes" if S is present in L , else print "No".</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Definition for L :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">L consists of 28 characters , a-z and '?' and '*'</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">? denotes zero or 1 character(s).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">* denotes zero or any number of characters.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Example :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">String "adb" is present in language L = {a?b}</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">String "adb" is present in language L ={a*b}</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">String "ab" is present in language L = {a?*b*}</div>
<p>Bob is playing Hide and Seek with alphabets and he is amazed by the properties of '?' and '*' in the language. He is given a language 'L'. He has to check whether the given string 'S' is present in the language 'L'. He needs your help. Print "Yes" if S is present in L , else print "No".</p>
<p>Definition for L :</p>
<p>L consists of 28 characters , a-z and '?' and '*'</p>
<p>? denotes zero or 1 character(s).</p>
<p>* denotes 0 or any number of characters.</p>
<p>Example :</p>
<p>String "adb" is present in language L = {a?b}</p>
<p>String "adb" is present in language L ={a*b}</p>
<p>String "ab" is present in language L = {a?*b*}</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>First line of input consists of T (T&lt;=50). Every test case consists of two strings, first line consists of 'L' and second line consists of 'S'. L consists characters among the 28 characters 'a'-'z' , '?' , '*' only. S consists of only lower case alphabets.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Print "Yes" if String 'S' is present in language 'L', else print "No".</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5</pre>
<pre>a?b</pre>
<pre>acb</pre>
<pre>a?b</pre>
<pre>abbb</pre>
<pre>a*b</pre>
<pre>abbbb</pre>
<pre>a*b</pre>
<pre>asbdfuisdhfsbdfsdfb</pre>
<pre>abb
</pre>
<pre>bb</pre>
<pre><strong>Output:</strong>
Yes</pre>
<pre>No</pre>
<pre>Yes</pre>
<pre>Yes</pre>
<pre>No</pre>