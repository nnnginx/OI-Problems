<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">Okayu and Korone are playing Phasmophobia.</p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">There are <strong>N</strong> rooms, numbered <strong>1</strong> to <strong>N</strong>. Each player has to enter the <strong>N</strong> rooms in an order.</p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">Let <strong>P</strong> be the permutation of size <strong>N</strong> representing the order of rooms Okayu enters, and <strong>Q</strong> for Korone.</p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">Korone doesn't want to be too far from Okayu, so they set up a plan as the following:</p>
<ul style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">
<li style="margin: 2px; padding: 1px;">Okayu will enter the rooms in numerical order. Formally, <strong>P = {1, 2, 3, ..., N}</strong>.</li>
<li style="margin: 2px; padding: 1px;">Korone will enter the rooms in a way such that <strong>|P<sub>i</sub></strong><strong>&nbsp;- Q<sub>i</sub></strong><strong>| </strong><span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;">¡Ü K </span><span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;">for every <strong>1 </strong><span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;"><strong>¡Ü i </strong><span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;">¡Ü N</span><span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;">.</span></span></span></li>
</ul>
<p><span style="font-family: Ubuntu, sans-serif;"><span style="font-size: 14px;">How many configurations can Korone enter the rooms? Since the answer can be large, print the answer modulo <strong>10<sup>9&nbsp;</sup>+ 7</strong>.</span></span></p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Input Format</strong></p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">The first and only line contains two integers&nbsp;<strong>N </strong><strong>and <strong>K</strong></strong>.</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Output Format</strong></p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><span style="font-family: Ubuntu, sans-serif; font-size: 14px;">Print an integer denoting the number of permutations <strong>Q</strong>&nbsp;satisfying the conditions above in modulo <strong>10<sup>9</sup>&nbsp;+ 7</strong>.</span></p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Sample Input 1</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">3 1</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Sample Output 1</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">3</p>
<p style="font-size: 18px; font-family: Ubuntu, sans-serif;"><strong>Sample Input 2</strong></p>
<p style="font-size: 14px; font-family: Ubuntu, sans-serif;">3 2</p>
<p style="font-size: 18px; font-family: Ubuntu, sans-serif;"><strong>Sample Output 2</strong></p>
<p style="font-size: 14px; font-family: Ubuntu, sans-serif;">6</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Explanation</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">In sample 1, the possible configurations are <strong>{1, 2, 3}</strong>,<strong> {2, 1, 3}</strong>,<strong> </strong>and<strong> {1, 3, 2}</strong>.</p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">In sample 2, all permutations are valid.</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Constraints</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; "><strong>1 ¡Ü&nbsp;N&nbsp;¡Ü&nbsp;1000</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; "><strong><span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;">1 ¡Ü K</span><span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;">&nbsp;¡Ü 5</span></strong></p>