<p>Have you ever wished to be given a direct problem statement in the contest? Do you hate the boring stories that problem setters write...starting from ¡°john was going on a trip¡±¡­passing with ¡°blablabla¡±¡­and ending with ¡°kindly help John J¡±. We all know that there is no John so why wasting contestants time. As we were contestants and know that feeling very well, we decided to break that boring way and save your time¡­</p>
<p>Given the following sequence details:&nbsp; <strong>F(0) = 0, F(1) = 1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>and<strong>&nbsp;</strong></p>
<p><strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; SUM F(i) [i from 0 to n] = F(n+2) - 1</strong></p>
<p>For a given integer M, we will generate another infinite sequence defined as:&nbsp; <strong>T(i) = F(i) % M</strong>. We noticed that this is a repeating sequence: it repeats itself after some <strong>C</strong> iterations, where C is the cycle length for sequence T. Let¡¯s define <strong>H(j),</strong> as the finite, <em>most left</em>, strictly increasing <strong>sub</strong>-sequence starting at position <strong>j</strong> in the sequence T, <em>preserving</em> the elements order of T. In other words:</p>
<p>1)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>H(0), </strong>the<strong> </strong>first element in H, is<strong> T(j)</strong></p>
<p>2)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>H(1)</strong>&nbsp; = T(k1), where T(k1) is the first element &gt; T(j) where j &lt; k1</p>
<p>3)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>H(2)</strong>&nbsp; = T(k2), where T(k2) is the first element &gt; T(k1) where k1 &lt; k2, and so on</p>
<p>For example, if M = 4, then T = [<strong>0 1 1 2 3 1</strong>&nbsp;&nbsp; 0 1 1 2 3 1&nbsp;&nbsp; 0 1 1 2 ¡­]. Furthermore: H(0) = [0 1 2 3], H(3) = [2 3], and H(5) = [1 2 3]. <strong>Length(&nbsp; H(j) )</strong> is the number of elements in that sequence, e.g. <strong>Length(H(5))</strong> = 3. The <strong>Cycle length(C)</strong> for sequence T is 6.</p>
<p>&nbsp;</p>
<p>For a given M, you will calculate its C, and <strong>evaluate</strong> the following <strong>summation</strong>:</p>
<p><strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; SUM Length( H(k) ) [k = 0 to C-1]</strong></p>
<p><strong>Input Specification:</strong></p>
<p>The first line of input contains an integer T that represents the number of test cases, then follow T lines each contains an integer 1 ¡Ü M ¡Ü 10<sup>5</sup>. NOTE: for any <strong><em>given</em></strong> test case, sequence T repeats after maximum C iterations where C ¡Ü 10<sup>5</sup>.</p>
<p><strong>Output Specification:</strong></p>
<p>For each test case, output a single line of output in the form <strong>¡°Case K: summation¡±</strong> where K is the number of the test case and summation is as defined in the problem statement.</p>
<p>&nbsp;</p>
<p><strong>Sample input:</strong></p>
<p>1</p>
<p>4</p>
<p><strong>Sample Output:</strong></p>
<p>Case 1: 16</p>