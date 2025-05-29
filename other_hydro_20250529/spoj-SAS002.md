<p>Apoorv is an expert in maths .There are very few questions in maths that Apoorv is unable to answer.Apoorv's teacher is not very fond of Apoorv.So he decided to give Apoorv a&nbsp; function value to calculate.Apoorv is unable to solve this problem and turns to you for help.Help him to find the answer to the function quickly.Apoorv's teacher will only check the final answer.So Apoorv is free to do calculate the value by any function he likes but the final answer should be same.Also as his teacher don't like him much he gave him a very strict time limit to solve the problem.Help Apoorv in finding the answer quickly.</p>
<p>The function given by Apoorv's teacher is as follows:</p>
<pre><code><span>function</span><span>(</span><span>number</span><span>)</span><span> </span><span>{</span><span>
              answer </span><span>=</span><span> </span><span>1</span><span>
              </span><span>for</span><span> </span><span>(</span><span> each i </span><span>from</span><span> </span><span>1</span><span> to number</span><span>)</span><span> </span><span>{</span><span>
                   </span><span>if</span><span>(</span><span> number modulo i </span><span>is</span><span> </span><span>0</span><span>  </span><span>)</span><span> </span><span>{</span><span>
                       answer=answer multiplied by i</span><span>&nbsp;</span><span>
                   </span><span>}</span><span>
              </span><span>}</span><span>
              </span><span>return</span><span> answer
          </span><span>}</span></code></pre>
<pre><code><span>Constraints:<br>At max 100 numbers will be given by Apoorv's teacher.<br>The value of number given by Apoorv's teacher will easily fit into 64 bit-integer and will always be positive.<br></span></code></pre>
<h3>Input</h3>
<p>First line will contain t denoting t numbers that are given by Apoorv's teacher.</p>
<p>Next t lines will contain a single integer denoting the number.</p>
<h3>Output</h3>
<p>For each t numbers output the value of answer in new line.Since the value of answer can be very large Apoorv's teacher is fine with you reporting the answer modulo <strong>10<sup>9</sup>+7.</strong></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>1<br>2<br><strong>Output:</strong>
1<br>2</pre>