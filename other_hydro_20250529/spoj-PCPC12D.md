<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">Meeda will compete this year in the ACM-ICPC world finals, but he is a crazy guy, he created a new strategy to attack the problem set. His new strategy is to solve the problems according to their names. He’ll sort the problem set according to the following rules.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">•<span style="white-space: pre;"> </span>Remove all whitespace characters from the problem names.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">•<span style="white-space: pre;"> </span>Replace any capital letters with the corresponding small one. i.e ‘A’ will be ‘a’</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">•<span style="white-space: pre;"> </span>count the occurrence of each character</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">•<span style="white-space: pre;"> </span>Problem A comes before problem B, if A contains lexicographically smaller characters more than B i.e A = “cba” comes before B = “bc” because A contains 1 'a' and B contains 0 'a'.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">But as you may know that meeda is a very lazy guy and he needs to train for this strategy before the world finals, so he needs your help to write an efficient program to help him in the training.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">Input Specification</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">The first line of the input contains T, number of test cases, each test case starts with an integer n (0&lt;n&lt;1000) number of problems, follow n lines each containing string s. The ith line is the name of the ith problem. s will be a sequence of characters (a-z, A-Z or any white space character), length of s is less than 100 characters.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">Output Specification</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">First line of each test case should contains “case: ” without double quotes followed by the test case number starting from 1, then follow problem names sorted as described above.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">Sample Input</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">2</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">2</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">abc</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">ab</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">4</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">bcsaasd</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">dbasaaaa</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">azzz</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">bayy</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">Sample Output</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">case: 1</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">ab</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">abc</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">case: 2</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">dbasaaaa</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">bcsaasd</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">bayy</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">azzz</span></div>
<p>&nbsp;</p>
<p><span style="font-size: small;">Meeda will compete this year in the ACM-ICPC world finals, but he is a crazy guy, he created a new strategy to attack the problem set. His new strategy is to solve the problems according to their names. He’ll sort the problem set according to the following rules.</span></p>
<p><span style="font-size: small;">•<span style="white-space: pre;"> </span>Remove all whitespace characters from the problem names.</span></p>
<p><span style="font-size: small;">•<span style="white-space: pre;"> </span>Replace any capital letters with the corresponding small one. i.e ‘A’ will be ‘a’</span></p>
<p><span style="font-size: small;">•<span style="white-space: pre;"> </span>count the occurrence of each character</span></p>
<p><span style="font-size: small;">•<span style="white-space: pre;"> </span>Problem A comes before problem B, if A contains lexicographically smaller characters more than B i.e A = “cba” comes before B = “bc” because A contains 1 'a' and B contains 0 'a'.</span></p>
<p><span style="font-size: small;">But as you may know that meeda is a very lazy guy and he needs to train for this strategy before the world finals, so he needs your help to write an efficient program to help him in the training.</span></p>
<p><span style="font-size: small;"><strong>Input Specification</strong></span></p>
<p><span style="font-size: small;">The first line of the input contains T, number of test cases, each test case starts with an integer n (0&lt;n&lt;1000) number of problems, follow n lines each containing string s. The ith line is the name of the ith problem. s will be a sequence of characters (a-z, A-Z or any white space character), length of s is less than 200 characters.</span></p>
<p><span style="font-size: small;"><strong>Output Specification</strong></span></p>
<p><span style="font-size: small;">First line of each test case should contains “case: ” without double quotes followed by the test case number starting from 1, then follow problem names sorted as described above.</span></p>
<p><span style="font-size: small;"><strong>Sample Input</strong></span></p>
<p><span style="font-size: medium;">2</span></p>
<p><span style="font-size: medium;">2</span></p>
<p><span style="font-size: medium;">abc</span></p>
<p><span style="font-size: medium;">ab</span></p>
<p><span style="font-size: medium;">4</span></p>
<p><span style="font-size: medium;">bcsaasd</span></p>
<p><span style="font-size: medium;">dbasaaaa</span></p>
<p><span style="font-size: medium;">azzz</span></p>
<p><span style="font-size: medium;">bayy</span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"><strong>Sample Output</strong></span></p>
<p><span style="font-size: medium;">case: 1</span></p>
<p><span style="font-size: medium;">abc</span></p>
<p><span style="font-size: medium;">ab</span></p>
<p><span style="font-size: medium;">case: 2</span></p>
<p><span style="font-size: medium;">dbasaaaa</span></p>
<p><span style="font-size: medium;">bcsaasd</span></p>
<p><span style="font-size: medium;">bayy</span></p>
<p><span style="font-size: medium;">azzz</span></p>
<p>&nbsp;</p>
<p><strong><span style="font-size: medium;">note :&nbsp;</span></strong><span style="font-size: small;">sorry for the wrong description .</span></p>
<p><span style="font-size: small;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;max length is 200 .</span></p>