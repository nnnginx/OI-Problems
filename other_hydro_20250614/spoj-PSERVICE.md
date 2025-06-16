<p>A website provides its users with a variety of services. There are a total of <strong>K</strong> services available on that website. At present there are <strong>M</strong> users/clients registered to the website.</p>
<p>Now each client of this service provider firm is to be allocated a project by the website which makes use of a string <strong>A1,A2,A3.............An</strong> of <strong>N</strong> services all of which the website is providing. The order in which the services are executed <strong>matters </strong>(compiling and then linking is different from linking and then compiling). Also, in a particular project, the same services cannot be executed twice in succession. For example, compiling ¡ú linking ¡ú compiling is allowed, but linking ¡ú linking ¡ú compiling is not allowed because 'linking' comes twice in succession.</p>
<p>All the M clients will start working at the same time and the time taken for the execution of all services is equal. At a time, one service can be accessed by only one client as there is only one server. For eg. If there are 3 clients with projects ¨C <strong>A1,A2...An</strong> ; <strong>B1,B2....Bn</strong> and <strong>C1,C2....Cn</strong> , then <strong>Ai</strong>, <strong>Bi</strong>, <strong>Ci </strong>are pairwise distinct<strong> </strong>for 1 &lt;= <strong>i</strong> &lt;= <strong>N</strong>. You need to find in how many ways in which the <strong>M</strong> clients can be allocated their projects.</p>
<p><strong>Input</strong></p>
<p>First line containing <strong>T</strong> (number of test cases).</p>
<p>For each test case one line containing 3 integers <strong>N</strong> ,<strong>M</strong> and <strong>K</strong>.</p>
<p><strong>Output</strong></p>
<p>For each test case output a separate line containing the answer modulo 1000000007.</p>
<p><strong>Constraints</strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>1 &lt;=<strong> T</strong> &lt;= 10</p>
<p>0 &lt;=<strong> N </strong>&lt;= 1000000000</p>
<p>1 &lt;=<strong> M </strong>&lt;= 100</p>
<p>0 &lt;= <strong>K </strong>&lt;= 1000</p>
<p><strong>Sample Input</strong></p>
<p>3</p>
<p>2 2 3</p>
<p>1 2 3</p>
<p>2 3 4</p>
<p><strong>Sample Output</strong></p>
<p>18</p>
<p>6</p>
<p>264</p>
<p>&nbsp;</p>