<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The Death Eaters are low on funds, and their leader Voldemort has asked them to get more money quickly, or face his wrath. &nbsp;They decide that the best way is to rob Gringotts Wizarding Bank. &nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">By threatening one of the goblins in charge of the bank, the 'M' Death Eaters have discovered that Gringotts has 'N' vaults, with vault number 'i' containing &nbsp;X[i] gold items. &nbsp;The weights of the gold items in the ith vault are g[i][1],g[i][2],...,g[i][X[i]]. But as soon as a vault is robbed, the magical wards go off and alarm bells ring. Thus they have enough time to rob just one vault each, and all robberies have to take place at the same time. The Death Eaters have decided that no two of them will rob the same vault as this increases the chances of them being caught.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Death Eater j has a bag which can hold weight v[j]. They are a greedy and cowardly lot, so a Death Eater will only agree to rob a vault if he can fill up his bag completely to its capacity by taking some subset of the objects present in that vault. Note that it is not possible for a Death Eater to break any gold item; either it should be taken fully, or not be taken.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Find the maximum weight of gold they can take away by planning their strategy correctly.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Input (STDIN):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line contains the number of test cases T. T test cases follow. Each test case contains integers M and N on the first line. The next line contains M integers, the jth of which is v[j], which is the maximum weight of gold the jth Death Eater's bag can hold. The following N lines describe the gold items in the vaults. The ith line contains X[i], the number of gold items present in the ith vault, followed by X[i] integers g[i][1]..g[i][X[i]], denoting the weights of the each of the items present in the ith vault. There is a blank line after each test case.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output (STDOUT):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output one line for each test case, containing the maximum total weight of gold that the Death Eaters can rob.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= T &lt;= 10</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= N,M &lt;= 50</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= X[i] &lt;= 25</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= v[i],g[i][j] &lt;= 10,000,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Time Limit: 10 s</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Memory Limit: 64 MB</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 9</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 4 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 3 9</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 10</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 7 8 10</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 1 2 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 3 7</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4 2 2 4 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">12</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">28</div>
<p>&nbsp;</p>
<p>The Death Eaters are low on funds, and their leader Voldemort has asked them to get more money quickly, or face his wrath. &nbsp;They decide that the best way is to rob Gringotts Wizarding Bank. &nbsp;</p>
<p>&nbsp;</p>
<p>By threatening one of the goblins in charge of the bank, the 'M' Death Eaters have discovered that Gringotts has 'N' vaults, with vault number 'i' containing &nbsp;X[i] gold items. &nbsp;The weights of the gold items in the ith vault are g[i][1],g[i][2],...,g[i][X[i]]. But as soon as a vault is robbed, the magical wards go off and alarm bells ring. Thus they have enough time to rob just one vault each, and all robberies have to take place at the same time. The Death Eaters have decided that no two of them will rob the same vault as this increases the chances of them being caught.</p>
<p>&nbsp;</p>
<p>Death Eater j has a bag which can hold weight v[j]. They are a greedy and cowardly lot, so a Death Eater will only agree to rob a vault if he can fill up his bag completely to its capacity by taking some subset of the objects present in that vault. Note that it is not possible for a Death Eater to break any gold item; either it should be taken fully, or not be taken.</p>
<p>&nbsp;</p>
<p>Find the maximum weight of gold they can take away by planning their strategy correctly.</p>
<p>&nbsp;</p>
<p><strong>Input (STDIN):</strong></p>
<p>The first line contains the number of test cases T. T test cases follow. Each test case contains integers M and N on the first line. The next line contains M integers, the jth of which is v[j], which is the maximum weight of gold the jth Death Eater's bag can hold. The following N lines describe the gold items in the vaults. The ith line contains X[i], the number of gold items present in the ith vault, followed by X[i] integers g[i][1]..g[i][X[i]], denoting the weights of the each of the items present in the ith vault. There is a blank line after each test case.</p>
<p>&nbsp;</p>
<p><strong>Output (STDOUT):</strong></p>
<p>Output one line for each test case, containing the maximum total weight of gold that the Death Eaters can rob.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= T &lt;= 10</p>
<p>1 &lt;= N,M &lt;= 50</p>
<p>1 &lt;= X[i] &lt;= 25</p>
<p>1 &lt;= v[i],g[i][j] &lt;= 10,000,000</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>2</p>
<p>2 3</p>
<p>3 9</p>
<p>2 4 5</p>
<p>2 3 9</p>
<p>1 10</p>
<p>&nbsp;</p>
<p>4 4</p>
<p>3 7 8 10</p>
<p>3 1 2 4</p>
<p>2 3 7</p>
<p>4 2 2 4 4</p>
<p>1 3</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>12</p>
<p>28</p>
<p>&nbsp;</p>
<p>&nbsp;</p>