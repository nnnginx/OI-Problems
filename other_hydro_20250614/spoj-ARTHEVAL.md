<p align="left">
Evaluate a parenthesized expression of single-digit positive integers and the binary operators +, -, *.
</p><p>
The order of operations differs from the canonical one in that operations have no precedence; they are simply evaluated from left-to-right, with only parentheses affecting the order of evaluation.
</p><p>
Every intermediate step is guaranteed to have absolute value no greater than 1,000,000,000.
</p><p>
<b>Input:</b>
</p><p>Input is an arithmetic expression of single-digit positive integers, the binary operators +,-, * and parentheses (). The arithmetic expression will be well-formed and will have no spaces.
</p><p>
<b>Output:</b>
</p><p>The evaluated value of the arithmetic expression.
</p><p>
</p><table width="100%">
<tbody><tr>
<td valign="top"><b>Example Input 1:</b></td>
<td valign="top"><b>Example Input 2:</b></td>
<td valign="top"><b>Example Input 3:</b></td>
</tr>
<tr>
<td valign="top"><pre>1*2+1
</pre></td>
<td valign="top"><pre>1+1*2
</pre></td>
<td valign="top"><pre>(5*6)-(40+(1))
</pre></td>
</tr>
<tr>
<td valign="top"><b>Example Output 1:</b></td>
<td valign="top"><b>Example Output 2:</b></td>
<td valign="top"><b>Example Output 3:</b></td>
</tr>
<tr>
<td valign="top"><pre>3
</pre></td>
<td valign="top"><pre>4
</pre></td>
<td valign="top"><pre>-11
</pre></td>
</tr>
</tbody></table>