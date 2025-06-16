<p><span style="font-size: small;">Due to A.M.SCOtt in the 19th century, it's an incomplete columnar transposition cipher <br>with alternating single letters and digraphs. The first entry must be a digraph.<br>In both even and odd periods the first column and the first row always alternate:</span></p>
<table style="height: 200px; width: 200px;" border="0" align="left">
<tbody>
<tr>
<td><span style="text-decoration: underline;"><strong><span style="font-size: medium;">4</span></strong></span></td>
<td><span style="text-decoration: underline;"><strong><span style="font-size: medium;">1</span></strong></span></td>
<td><span style="text-decoration: underline;"><strong><span style="font-size: medium;">3</span></strong></span></td>
<td><span style="text-decoration: underline;"><strong><span style="font-size: medium;">2</span></strong></span></td>
<td><span style="text-decoration: underline;"><strong><span style="font-size: medium;">5</span></strong></span></td>
</tr>
<tr>
<td><strong><span style="font-size: small;">IN</span></strong></td>
<td><strong><span style="font-size: small;">C</span></strong></td>
<td><strong><span style="font-size: small;">OM</span></strong></td>
<td><strong><span style="font-size: small;">P</span></strong></td>
<td><strong><span style="font-size: small;">LE</span></strong></td>
</tr>
<tr>
<td><strong><span style="font-size: small;">T</span></strong></td>
<td><strong><span style="font-size: small;">EC</span></strong></td>
<td><strong><span style="font-size: small;">O</span></strong></td>
<td><strong><span style="font-size: small;">LU</span></strong></td>
<td><strong><span style="font-size: small;">M</span></strong></td>
</tr>
<tr>
<td><strong><span style="font-size: small;">NA</span></strong></td>
<td><strong><span style="font-size: small;">R</span></strong></td>
<td><strong><span style="font-size: small;">WI</span></strong></td>
<td><strong><span style="font-size: small;">T</span></strong></td>
<td><strong><span style="font-size: small;">HA</span></strong></td>
</tr>
<tr>
<td><strong><span style="font-size: small;">L</span></strong></td>
<td><strong><span style="font-size: small;">TE</span></strong></td>
<td><strong><span style="font-size: small;">R</span></strong></td>
<td><strong><span style="font-size: small;">NA</span></strong></td>
<td><strong><span style="font-size: small;">T</span></strong></td>
</tr>
<tr>
<td><strong><span style="font-size: small;">IN</span></strong></td>
<td><strong><span style="font-size: small;">G</span></strong></td>
<td><strong><span style="font-size: small;">SI</span></strong></td>
<td><strong><span style="font-size: small;">N</span></strong></td>
<td><strong><span style="font-size: small;">GL</span></strong></td>
</tr>
<tr>
<td><strong><span style="font-size: small;">E</span></strong></td>
<td><strong><span style="font-size: small;">LE</span></strong></td>
<td><strong><span style="font-size: small;">T</span></strong></td>
<td><strong><span style="font-size: small;">TE</span></strong></td>
<td><strong><span style="font-size: small;">R</span></strong></td>
</tr>
<tr>
<td><strong><span style="font-size: small;">SA</span></strong></td>
<td><strong><span style="font-size: small;">N</span></strong></td>
<td><strong><span style="font-size: small;">DD</span></strong></td>
<td><strong><span style="font-size: small;">I</span></strong></td>
<td><strong><span style="font-size: small;">GR</span></strong></td>
</tr>
<tr>
<td><strong><span style="font-size: small;">A</span></strong></td>
<td><strong><span style="font-size: small;">PH</span></strong></td>
<td><strong><span style="font-size: small;">S</span></strong></td>
<td><strong><span style="font-size: small;">&nbsp;</span></strong></td>
<td><strong><span style="font-size: small;">&nbsp;</span></strong></td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3 style="text-align: left;">Input</h3>
<p><span style="font-size: small;">N lines (N&lt;1000)<br>Each line of the input contains the numeric key (permutation order of the columns) <br>and a plaintext. Plaintext letters are in [A-Z] only with no punctuation. <br>The keylength max is 9 and the length of the plaintext is limited to 250. <br>The last line ends with EOF.</span></p>
<h3 style="text-align: left;">Output</h3>
<p><span style="font-size: small;">Output consist of exactly N lines of ciphertexts with letters in [A-Z] with no spaces.</span></p>
<h3 style="text-align: left;">Example</h3>
<pre><span style="font-size: small;"><strong>Input:</strong></span>
<br><span style="font-size: medium;"><strong>41325 INCOMPLETECOLUMNARWITHALTERNATINGSINGLELETTERSANDDIGRAPHS</strong></span>

<span style="font-size: small;"><strong>Output:</strong></span><br><br>&nbsp;<span style="font-size: medium;"><strong>CECRTEGLENPHPLUTNANTEIOMOWIRSITDDSINTNALINESAALEMHATGLRGR</strong></span></pre>