<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">A positive integer&nbsp;<strong>X </strong>is a comet number if there exists 5 positive integers <strong>A B C D E </strong>such that:</p>
<ul style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">
<li style="margin: 2px; padding: 1px;"><strong>A + B + C + D = X</strong></li>
<li style="margin: 2px; padding: 1px;"><strong>A + E, B - E, C * E, </strong>and <strong>D / E</strong>&nbsp;are pairwise equal, meaning <strong>A + E = B - E = C * E = D / E</strong></li>
</ul>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">Kanata gave Suisei <strong>N&nbsp;</strong>positive integers <strong>A<sub>i</sub></strong>&nbsp;for <strong>1 </strong><span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;"><strong>¡Ü i </strong><span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;">¡Ü N</span><span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;">. </span></span></p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;"><span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;"><span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;">Suisei would like to know whether</span><span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;">&nbsp;A<sub>i</sub>&nbsp;</span><span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;">i</span><span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;">s a comet number or not.</span></span></p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Input Format</strong></p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">The first line contains an integer&nbsp;<strong>N</strong>.</p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">The next <strong>N</strong>&nbsp;lines contain an integer <span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;">A<sub>i</sub></span></p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Output Format</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">Print <strong>N</strong>&nbsp;lines.</p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">The <strong>i</strong>-th line contains the string "YES" (without quotes) if <span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;">A<sub>i</sub></span>&nbsp;is a comet number and "NO" <span style="font-family: Ubuntu, sans-serif; font-size: 14px;">(without quotes)&nbsp;</span>otherwise.</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Sample Input&nbsp;</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">4<br>8<br>1<br>69<br>128</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Sample Output</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">YES<br>NO<br>NO<br>YES</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Explanation</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">8 is a comet number as there exists a valid quintuple <strong>(A, B, C, D, E) = (1, 3, 2, 2, 1)</strong>.</p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; "><span style="font-family: Ubuntu, sans-serif; font-size: 14px;">128 is a comet number as there exists a valid quintuple&nbsp;</span><strong>(A, B, C, D, E) = (31, 33, 32, 32, 1)</strong><span style="font-family: Ubuntu, sans-serif; font-size: 14px;">.</span></p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Constraints</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; "><strong>1 ¡Ü&nbsp;N, A<sub>i</sub>&nbsp;¡Ü&nbsp;10<sup>5</sup></strong></p>