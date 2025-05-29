<p>Digo has a cylindrical box which is vertically partitioned into <strong>N</strong> contiguous sectors which are open from the top. Each Sectorial Compartment initially contains a fixed number of coins. Now Digo wants to fill each Sectorial Compartment with equal number of coins. But the problem is that, at a time he is only allowed to increment any two adjacent sectors with one coin each. Given an initial arrangement, you need to tell whether such equalization is possible or not.</p>
<p>Every sector <strong>i</strong> (for all (0 &lt; <strong>i </strong>&lt;<strong> N</strong>)) is adjacent to sector (<strong>i + 1</strong>) and sector <strong>N</strong> is adjacent to sector <strong>1</strong>.</p>
<p><strong>Input</strong></p>
<p>In first line, the number of test cases <strong>T.</strong></p>
<p>Each test case consists of a number <strong>N, </strong>followed by a line containing <strong>N</strong> space seperated integers where <strong>i<sup>th</sup></strong> integer (<strong>Mi</strong>) denotes the number of coins in <strong>i<sup>th</sup></strong> sectorial compartment of the box (initially), in clockwise order.</p>
<p><strong>Output</strong></p>
<p>For every test case output ¡°<strong>YES</strong>¡± for possible and ¡°<strong>NO</strong>¡± for which equalization is not possible (Without quotes).</p>
<p><strong>Constraints</strong></p>
<p>1 &lt;= <strong>T</strong> &lt;= 1000</p>
<p>3 &lt;= <strong>N </strong>&lt;= 100 (Number of Sectorial Compartments)</p>
<p>1 &lt;= <strong>Mi </strong>&lt;= 10^9 (Number of coins in each Sectorial Compartment)</p>
<p><strong>Sample Input</strong></p>
<p>2</p>
<p>3</p>
<p>1 2 3</p>
<p>4</p>
<p>1 2 1 2</p>
<p><strong>Sample Output</strong></p>
<p>YES</p>
<p>NO</p>