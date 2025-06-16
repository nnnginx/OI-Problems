<p><span style="font-size: small;">Here you have to decipher the AMSCO cipher :</span></p>
<p><span style="font-size: small;">Due to A.M.SCOtt in the 19th century, <strong>it's an incomplete columnar transposition cipher <br>with alternating single letters and digraphs</strong>. The first entry must be a digraph.<br>In both even and odd periods the first column and the first row always alternate:</span></p>
<table style="width: 219px; height: 159px;" border="0">
<tbody>
<tr>
<td><span style="font-size: medium;"><span style="text-decoration: underline;"><strong>7</strong></span></span></td>
<td><span style="text-decoration: underline;"><strong><span style="font-size: medium;">4</span></strong></span></td>
<td><span style="text-decoration: underline;"><strong><span style="font-size: medium;">5</span></strong></span></td>
<td><span style="text-decoration: underline;"><strong><span style="font-size: medium;">6</span></strong></span></td>
<td><span style="text-decoration: underline;"><strong><span style="font-size: medium;">3</span></strong></span></td>
<td><span style="font-size: medium;"><span style="text-decoration: underline;"><strong>2</strong></span></span></td>
<td><span style="font-size: medium;"><span style="text-decoration: underline;"><strong>1</strong></span></span></td>
</tr>
<tr>
<td><span style="font-size: small;"><strong>RI</strong></span></td>
<td><span style="font-size: small;"><strong>D</strong></span></td>
<td><span style="font-size: small;"><strong>ER</strong></span></td>
<td><span style="font-size: small;"><strong>S</strong></span></td>
<td><span style="font-size: small;"><strong>ON</strong></span></td>
<td><span style="font-size: small;"><strong>T</strong></span></td>
<td><span style="font-size: small;"><strong>HE</strong></span></td>
</tr>
<tr>
<td><span style="font-size: small;"><strong>S</strong></span></td>
<td><span style="font-size: small;"><strong>TO</strong></span></td>
<td><span style="font-size: small;"><strong>R</strong></span></td>
<td><span style="font-size: small;"><strong>MI</strong></span></td>
<td><span style="font-size: small;"><strong>N</strong></span></td>
<td><span style="font-size: small;"><strong>TO</strong></span></td>
<td><span style="font-size: small;"><strong>T</strong></span></td>
</tr>
<tr>
<td><span style="font-size: small;"><strong>HI</strong></span></td>
<td><span style="font-size: small;"><strong>S</strong></span></td>
<td><span style="font-size: small;"><strong>HO</strong></span></td>
<td><span style="font-size: small;"><strong>U</strong></span></td>
<td><span style="font-size: small;"><strong>SE</strong></span></td>
<td><span style="font-size: small;"><strong>W</strong></span></td>
<td><span style="font-size: small;"><strong>EA</strong></span></td>
</tr>
<tr>
<td><span style="font-size: small;"><strong>R</strong></span></td>
<td><span style="font-size: small;"><strong>EB</strong></span></td>
<td><span style="font-size: small;"><strong>O</strong></span></td>
<td><span style="font-size: small;"><strong>RN</strong></span></td>
<td><span style="font-size: small;"><strong>J</strong></span></td>
<td><span style="font-size: small;"><strong>IM</strong></span></td>
<td><span style="font-size: small;"><strong>M</strong></span></td>
</tr>
<tr>
<td><span style="font-size: small;"><strong>OR</strong></span></td>
<td><span style="font-size: small;"><strong>R</strong></span></td>
<td><span style="font-size: small;"><strong>IS</strong></span></td>
<td><span style="font-size: small;"><strong>O</strong></span></td>
<td><span style="font-size: small;"><strong>N</strong></span></td>
<td><span style="font-size: small;"><strong></strong></span></td>
<td><span style="font-size: small;"><strong></strong></span></td>
</tr>
</tbody>
</table>
<h3 style="text-align: left;">Input</h3>
<p><span style="font-size: small;">N lines (N&lt;1000)<br>Each line of the input contains the numeric key (permutation order of the columns) <br>and a ciphertext. Ciphertext letters are in [A-Z] only with no punctuation. <br>The keylength max is 9 and the length of the ciphertext is limited to 250. <br>The last line ends with EOF.</span></p>
<h3 style="text-align: left;">Output</h3>
<p><span style="font-size: small;">Output consist of exactly N lines of plaintexts with letters in [A-Z] with no spaces.</span></p>
<h3 style="text-align: left;">Example 1:</h3>
<pre><span style="font-size: small;"><strong>Input:</strong></span><br><span style="font-size: medium;"><strong> 7456321 </strong></span><span style="font-size: medium;"><strong>HETEAMTTOWIMONNSEJNDTOSEBRERRHOOISSMIURNORISHIROR</strong></span>
<span style="font-size: small;"><strong>Output:</strong></span><span style="font-size: medium;"><strong><br> </strong></span><span style="font-size: medium;"><strong>RIDERSONTHESTORMINTOTHISHOUSEWEAREBORNJIMMORRISON</strong></span><br><h3 style="text-align: left;">Example 2:
</h3><pre><span style="font-size: small;"><strong>Input:</strong></span><br><span style="font-size: medium;"><strong> 41325 </strong></span><span style="font-size: medium;"><strong>CECRTEGLENPHPLUTNANTEIOMOWIRSITDDSINTNALINESAALEMHATGLRGR</strong></span><span style="font-size: medium;"><strong></strong></span>
<span style="font-size: small;"><strong>Output:</strong></span><span style="font-size: medium;"><strong><br> INCOMPLETECOLUMNARWITHALTERNATINGSINGLELETTERSANDDIGRAPHS<br></strong></span></pre>
<span style="font-size: medium;"><strong></strong></span></pre>