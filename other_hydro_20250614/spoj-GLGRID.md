<p>The 21st century introduces the multicores. As a result a research is going on in parallel Computing. With time the number of processor would grow very large. As of now, Professor Biloo  at IIIT asks a student to implement the following code on multiple G-line processors.<br><br>

</p><pre>        for(i=1;i&lt;=x;i++){
                for(j=1;j&lt;=x;j++){
                        for(k=1;k&lt;=a;k++){
                                z=z%y;
                        }
                }
                for(j=1;j&lt;=b;j++){
                        z=z/y;
                }
        }
        for(i=1;i&lt;=c;i++){
                z=z%y;
        }
</pre>

<br>

<p>The students experiments and finds that the only significant operations are the modulus(%) and division(/) operation which take almost equal time. The time taken by other operations may be ignored in the order analysis. He finds a algorithm to solve the problem in which these operations can be carried out in random order. For his testing he chooses M processors . Each processor will carry out exactly M operations (% or /) .The performance is optimal when such a scheme exactly covers all the operations.<br><br>

Puzzled, the student finds that this can only be done for some specific values of x for given a,b and c. He wants to trick the professor, so he needs few values of x for which his algorithm works. However, to make the professor feel that he manually did it these values of x need to be as small as possible.<br><br>

Given the values of a,b,c and k, output the first k values of x, for which the student's algorithm works.<br><br>

<b>Note:</b> The value of x should be greater than or equal to 0.<br>

</p><h3>Input</h3>
<p>The first line of input contains an integer t , the number of testcases. For each testcase , there is exactly one line which contains 4 space separated a,b,c and k.

</p><h3>Output</h3>
<p>For each test case, output the corresponding k values of x, each in successive different lines.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
1 2 1 4


<b>Output:</b>
0
1
2
3

</pre>

<h3>Constraints and Limits</h3>
<p>t ¡Ü 10. The values in the output vi ¡Ü 10^12. Each of the intermediate values will fit in a 64 bit variable. The values a,b,c would be such that 0 ¡Ü a,b,c ¡Ü 100            and b^2-4ac ¡Ý 0. k ¡Ü 1000.<br>
<br>
<b> Note  : </b> Test data to this problem was modified on Feb 7. <br>
<b> Note 2: </b> There were some mistakes in the test data discovered on March 11, 2008. New tricky cases provided by <a href="http://www.spoj.com/users/john_jones">Blue Mary</a> are also put up now and some "Accepted" solutions have received wrong answer. My apologies to one and all for the mistakes.<br>
</p>