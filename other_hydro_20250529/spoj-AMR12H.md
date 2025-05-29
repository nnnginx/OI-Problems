<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Wormtongue looked from face to face. In his eyes was the hunted look of a beast seeking some gap in the ring of his enemies.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">'Nay, Eomer, you do not fully understand the mind of Master Wormtongue,' said Gandalf, turning his piercing glance upon him. 'He is bold and cunning. Even now he plays a game with peril and wins a throw.' - Gandalf, trying to figure out Wormtongue's mind.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In fact, Wormtongue's mind is a complicated system of evaluating various variables and parameters. In essence, each parameter is a uniform random floating point variable between 0 and 1 (inclusive). Further, his mind works on calculating best and worst-case values, which are equivalent to min/max of 2 expressions.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For example, right now Wormtongue is calculating :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">'Chances of escaping' = max('Theoden letting me go', 'Me killing everyone')</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">'Theoden letting me go' = max('Theoden is forgiving by nature', 'Gandalf advises him to let me go').</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">'Me killing everyone' = min('Me killing Gandalf', 'Me killing Theoden').</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">So, you are given an expression consisting of independent uniform [0, 1] random variables, on which you have an expression consisting of "min", and "max" alone. Help Gandalf figure out Wormtongue's mind by finding the expected value of this expression.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input (STDIN):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line contains T, the number of test cases.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Each test case consists of a single line describing the expression. The characters of the string are derived from the set {'M','m','x'}, where 'M' stands for max, 'm' stands for min, and 'x' is a random variable</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Formally, in the expression tree, each node which asks for max is labeled as 'M', each node which asks for min is labelled 'm', and all the leaves are labeled 'x'. The description of the expression is preorder traversal of this tree.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For example, Mxmxx describes the expression max(x1, min(x2, x3)).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output (STDOUT):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For each test case, output one line which contains the expected value of the expression. The results should be accurate within an error range of 10^-6.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= T &lt;= 1,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= input string length &lt;= 100</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">x</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">mxx</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Mxx</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">MmxxMxx&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0.500000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0.333333</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0.666667</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0.700000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Notes/Explanation of Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For the first test case, it asks for the mean of a random number between 0 and 1, which is 0.5.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Note:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">It is recommended to use long long and long double data types in calculation to avoid precision errors.</div>
<p>Wormtongue looked from face to face. In his eyes was the hunted look of a beast seeking some gap in the ring of his enemies.</p>
<p>'Nay, Eomer, you do not fully understand the mind of Master Wormtongue,' said Gandalf, turning his piercing glance upon him. 'He is bold and cunning. Even now he plays a game with peril and wins a throw.' - Gandalf, trying to figure out Wormtongue's mind.</p>
<p>&nbsp;</p>
<p>In fact, Wormtongue's mind is a complicated system of evaluating various variables and parameters. In essence, each parameter is a uniform random floating point variable between 0 and 1 (inclusive). Further, his mind works on calculating best and worst-case values, which are equivalent to min/max of 2 expressions.</p>
<p>&nbsp;</p>
<p>For example, right now Wormtongue is calculating :</p>
<p>'Chances of escaping' = max('Theoden letting me go', 'Me killing everyone')</p>
<p>'Theoden letting me go' = max('Theoden is forgiving by nature', 'Gandalf advises him to let me go').</p>
<p>'Me killing everyone' = min('Me killing Gandalf', 'Me killing Theoden').</p>
<p>&nbsp;</p>
<p>So, you are given an expression consisting of independent uniform [0, 1] random variables, on which you have an expression consisting of "min", and "max" alone. Help Gandalf figure out Wormtongue's mind by finding the expected value of this expression.</p>
<p>&nbsp;</p>
<p><strong>Input (STDIN):</strong></p>
<p>The first line contains T, the number of test cases.</p>
<p>Each test case consists of a single line describing the expression. The characters of the string are derived from the set {'M','m','x'}, where 'M' stands for max, 'm' stands for min, and 'x' is a random variable</p>
<p>Formally, in the expression tree, each node which asks for max is labeled as 'M', each node which asks for min is labelled 'm', and all the leaves are labeled 'x'. The description of the expression is preorder traversal of this tree.</p>
<p>For example, Mxmxx describes the expression max(x1, min(x2, x3)).</p>
<p>&nbsp;</p>
<p><strong>Output (STDOUT):</strong></p>
<p>For each test case, output one line which contains the expected value of the expression. The results should be accurate within an error range of 10^-6.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= T &lt;= 1,000</p>
<p>1 &lt;= input string length &lt;= 100</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>4</p>
<p>x</p>
<p>mxx</p>
<p>Mxx</p>
<p>MmxxMxx&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>0.500000</p>
<p>0.333333</p>
<p>0.666667</p>
<p>0.700000</p>
<p>&nbsp;</p>
<p><strong>Notes/Explanation of Sample Input:</strong></p>
<p>For the first test case, it asks for the mean of a random number between 0 and 1, which is 0.5.</p>
<p>&nbsp;</p>
<p><strong>Note:</strong></p>
<p>It is recommended to use <strong>long long</strong> and<strong> long double</strong> data types in calculation to avoid precision errors.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>