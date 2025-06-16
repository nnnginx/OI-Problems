<pre><span style="white-space: normal;"><h2>Description</h2>
<p>While Johnny was studying a biology course he found a chapter about genetics and he started reading about it. Genetics is the study of genes, and studies what genes are and how they work. Genes are how living organisms inherit features from their ancestors; for example, children usually look like their parents because they have inherited their parents' genes. Genetics tries to identify which features are inherited, and explain how these features are passed from generation to generation. Genes are made from a long molecule called DNA, which is copied and inherited across generations. DNA is made of simple units that line up in a particular order within this large molecule. The order of these units carries genetic information, similar to how the order of letters on a page carries information. A chromosome is an organized structure of DNA. It is a single piece of coiled DNA containing many genes, regulatory elements and other nucleotide sequences. Chromosomes also contain DNA-bound proteins, which serve to package the DNA and control its functions.</p>
<p>Johnny decided to run an experiment to simulate the behavior of inheritance of a chromosome <strong><em>C</em></strong> that can be modeled as an array of integers each element <strong><em>C[i]</em></strong> of the array represents a gene of that chromosome. The value of each gene will be between 0 and 1,000,000,006. Since Johnny does not like programming he requested your help to run a simulation for a very large number of generations to check the values of the chromosome after <strong><em>G</em></strong> generations. On each generation <strong><em>T</em></strong> the value of each gene is the summation of some genes from the generation <strong><em>T</em></strong>-1 mod 1,000,000,007. For example if the chromosome of length 3, has values of genes 4, 7, and 12 initially and the 1<sup>st</sup> gene in new generation calculated as sum of 1<sup>st</sup> gene and 2<sup>nd</sup> gene in previous generation and 2<sup>nd</sup> gene in new generation calculated as sum of 2<sup>nd</sup> gene and 3<sup>rd</sup> gene in previous generation and 3<sup>rd</sup> gene in new generation calculated as sum of 3<sup>rd</sup> gene and 1<sup>st</sup> gene in previous generation. So after 1<sup>st</sup> generation chromosome will be 11, 19, and 16 and after 2<sup>nd</sup> generation chromosome will be 30, 35, and 27 and so on till generation <strong><em>G</em></strong>.</p>
<h2>Input Format</h2>
<p>Input will start with <strong><em>T</em></strong> number of test cases. The first line of each test case will contain two integers <strong><em>G, N</em></strong> where 0 &lt;= <strong><em>G </em></strong>&lt; 10<sup>18</sup> representing number of generations and 1 &lt;= <strong><em>N </em></strong>&lt;= 100 representing length of the chromosome. Followed by a line containing <strong><em>N</em></strong> integers <strong><em>n[i]</em></strong> separated by space where 0 &lt;= <strong><em>i </em></strong>&lt; N and 0 &lt;= <strong><em>n[i] </em></strong>&lt; 1,000,000,007 representing the value of each gene in the given chromosome. Followed by <strong><em>N</em></strong> lines, each line <strong><em>i</em></strong> start with integer <strong><em>M[i]</em></strong> representing the number of genes from the previous generation that is going to be added together to get the value of the new gene <strong><em>i </em></strong>at the new generation, followed by <strong><em>M[i]</em></strong> numbers <strong><em>x[j]</em></strong> where 0 &lt;= <strong><em>j </em></strong>&lt; <strong><em>M[i]</em></strong> and 0 &lt;= <strong><em>x[j] </em></strong>&lt; <strong><em>N</em></strong> representing the indices of genes to be added. The value of the gene at the new generation is &nbsp;</p>
<h2>Output Format</h2>
<p>For each test case, output the result using the following format:</p>
<p><strong><em>k</em></strong>. <strong><em>n[0] n[1] ��. n[N-1]</em></strong></p>
<p>Where <strong><em>k</em></strong> is the test case number (starting at 1), a single period, a single space, and<strong><em> n[i]</em></strong> is the value of <strong><em>i</em></strong><sup>th</sup> gene after <strong><em>G</em></strong> generations.</p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="284" valign="top">
<h2>Sample Input</h2>
</td>
<td width="284" valign="top">
<h2>Sample Output</h2>
</td>
</tr>
<tr>
<td width="284" valign="top">
<p>1</p>
<p>2&nbsp; 3</p>
<p>4 7 12</p>
<p>2 0 1</p>
<p>2 1 2</p>
<p>2 2 0</p>
</td>
<td width="284" valign="top">
<p>1. 30 35 27</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p></span></pre>