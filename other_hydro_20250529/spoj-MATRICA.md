<p>A matrix is a rectangular table of letters. A square matrix is a matrix with an equal number of rows and columns. A square matrix M is called symmetric if its letters are symmetric with respect to the main diagonal (M<sub>i,j</sub> = M<sub>j,i</sub> for all pairs of i and j).</p>

<p>For example, the following two matrices are symmetric:</p>

<pre>AAB          AAA
ACC          ABA
BCC          AAA
</pre>

<p>However, the following two are not:</p>

<pre>ABCD          AAB
ABCD          ACA
ABCD          DAA
ABCD
</pre>

<p>Given a collection of available letters, you are to output a subset of columns in the lexicographically smallest symmetric matrix which can be composed using all the letters. If no such matrix exists, output "IMPOSSIBLE".</p>

<p>To determine if matrix A is lexicographically smaller than matrix B, consider their elements in row-major order (as if you concatenated all rows to form a long string). If the first element in which the matrices differ is smaller in A, then A is lexicographically smaller than B.</p>

<h3>Input</h3>
<p>The first line of input contains two integers N (1 ¡Ü N ¡Ü 30000) and K (1 ¡Ü K ¡Ü 26). N is the dimension of the matrix, while K is the number of distinct letters that will appear.</p>

<p>Each of the following K lines contains an uppercase letter and a positive integer, separated by a space.</p>

<p>The integer denotes how many corresponding letters are to be used. For example, if a line says "A 3", then the letter A must appear three times in the output matrix.</p>

<p>The total number of letters will be exactly N<sup>2</sup>. No letter will appear more than once in the input.</p>

<p>The next line contains an integer P (1 ¡Ü P ¡Ü 50), the number of columns that must be output.</p>

<p>The last line contains P integers, the indices of columns that must be output. The indices will be between 1 and N inclusive, given in increasing order and without duplicates.</p>

<h3>Output</h3>
<p>If it is possible to compose a symmetric matrix from the given collection of letters, output the required columns on N lines, each containing P character, without spaces. Otherwise, output "IMPOSSIBLE" (quotes for clarity).</p>

<h3>Example</h3>

<pre><b>Input:</b>
3 3
A 3
B 2
C 4
3
1 2 3

<b>Output:</b>
AAB
ACC
BCC

<b>Input:</b>
4 5
E 4
A 3
B 3
C 3
D 3
2
2 4

<b>Output:</b>
AC
BE
DE
ED

<b>Input:</b>
4 6
F 1
E 3
A 3
B 3
C 3
D 3
4
1 2 3 4

<b>Output:</b>
IMPOSSIBLE
</pre>

<b>Warning: large input/output data.</b>

<p>Note: The test data for this problem consist of the official test cases from the contest, as well some cases of my own.</p>