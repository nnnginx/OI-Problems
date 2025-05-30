<p>See <a href="../ZZPERM/">ZZPERM</a> problem description. This an improved version with more demanding test cases.</p>
<h3>Input</h3>
<p>The input consists of at most 15 test cases. Each case contains a word (W) not longer than 64 letters and one positive number (D &lt;= 1000000000). The letters of each word are in increasing order. Input is terminated by EOF.</p>
<h3>Output</h3>
<p>For each case output all of the zig-zag permutations of W whose rank is divisible by D, in increasing lexicographic order, one word per line. In the next line print the total number of zig-zag permutations of W. There is no case that produces more than 365 lines of output. Print an empty line after each case.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
j 1
abc 2
aaabc 1
aaabb 2
aaaaaaaaaaaaaaaaabbbbbbbbbbbbbbbcccdd 123456
aaaaaaaaabbbbbbbbbcccccccccddddddddd 1000000000


<strong>Output:</strong>
j
1

bac
cab
4

abaca
acaba
2

1

babacbcabacabadabababababababababadab
213216

abacbcacbdadcdbcadbdacbdacbdadbcbcad
abadadcdcdcdbdbdadbcabacacbdbcbcacab
acabacbcbdbcbdcdadadacbcadbcbcadadbd
acacbcbdacbdcdacbcadbdbcbcadadbdabad
acadbcadbdbcacadbdbcacbdbdacbdbcadac
acbcacbcadbdadadadbcbdcdabacacbdbdbc
acbcbdadbdcdbcbcbcacbdadadadadbcacab
acbdadcdcdadadbdababacbcbcbcacbdbdac
acbdcdbdbcacbcbcadabadbcabadbdcdacad
adacbcacbcbcbdcdcdbdadadabadbdbcacab
adadbcbcadbcabacadbdbcbdabadcdcdacbc
adbcadbcabacbdacacbcbcbdcdadbdadbdac
adbdacababacadadcdbcbcadbdacbcbdcdbc
adbdcdacbdbcbdbcadadadbcadacbcacbcab
adcdbdacadacbdbcbdadacbcbcadbdbcacab
babacbdcdbdcdbcadcdbcabacacadadbdacb
bacacadbdcdbcbdbdcdacbdacabacadbcadb
bacadcdbcbdabacbcacacadadadcdbdbdbcb
bacbdadacabacadacbdcdbcadbcbdbcbdadc
badacadbcadacbcbdadbdbcacbcbdcdabadc
badbcacbdabadcdbcadbdacabacbdacbdcdc
badbdcdbdadacbcbcacacbdbdacbdadbcaca
bcabacadbdbdacacbdadcdadbcbcbcadacbd
bcacadacbcbdcdbdbcbdbdadadabacbdacac
bcacbdbdcdcdababadacbcadacacbdbdbcad
bcadbcadbdbdcdcdadbcbcacbcababadacad
bcbcabadacadcdadacbdadbcbdcdbcacbdab
bcbcbcadbcadbcadbdadbcbcadabacadadcd
bcbdacbdacbdbcbdadacacbdcdbdadacabac
bcbdbdbdcdacacacbdbcadadbcababacadcd
bdabadcdbdadbcadcdbcbdcdbcabacabacac
bdacbcbcbcadadbcadcdabadbcacbdcdabad
bdadbcabacbcbcababadacadcdcdbdcdacbd
bdbcacacbdbcadbcbdabacbcadacadadbdcd
bdbcbdacacbdadbdcdababadadcdbcacbcac
bdbdbcadbcacadbcadacadbdbdcdbcacacab
bdcdacbdadadbcbcacacbcacabadbdbcadbd
bdcdcdadacadcdbdbcababadbcacbcadbcab
cabacbdcdbdadacacadbcbcacadbcbdbdadb
cacabadcdbdbdbcbcbdacabadbdacbdacadc
cacadcdbcbcbdcdacababacbcadbdbdbdada
cacbdadbdadacbdababacbcbdcdcdcdabacb
cadacadbdabacbcacbdbdcdadbcadadbcbcb
cadbcacbcbdcdbdbcadbcbdadabacbdacada
cadbdbcbdacadbdacadacbdbcbcadbcabadc
cbcabacbcbdadabacbcadbdadcdcdadacbdb
cbcadacadadbdbcacbcadbdbdacbcabadcdb
cbcbcadacbcadadadbcbdacadbcbdbdacadb
cbcbdbcadcdacbdadacbdbcacadacbdabadb
cbdacadacbcbdcdbdabadbcbcacabadcdadb
cbdadbdadabadcdabadcdacbcbcabacbcbdc
cbdbcbdcdbcbdacacbdadadcdababacabadc
cbdcdacbdbcbdadacacadbcabababadcdbdc
cdabadacabadcdbdcdbdbcabadbcbcacadbc
cdacbcbcadabadcdbdbcbcacbdadadabadbc
cdadbcacacbcadadbdbdbcabadbcbcbcadad
cdbcacadbcbdbcadbdadadbdbcacbcadabac
cdbcbdadadacbdbcabacbcbcabadacadcdbd
cdbdbcabadcdbdbdcdacacababadbdacacbc
cdcdacacbcadbcabadbdcdbcbcabadadbdab
dababacbcbcadbdacacbcacbdbdcdadcdadb
dabadbdcdacacadabadcdbdbcbcbcacbdbca
dacadacbdbdbcacbcadbdbcacbcadbdcdaba
dacbcbdadadcdbdacadcdababacbcacbdbcb
dadabadbcbcadcdbdacbcadacadbcbcbdbca
dadbcadadbdcdcdabacbcbdbcacbdbcabaca
dadcdbcacabadadbcabadbcadcdadbcbcbcb
dbcacbcadacadbcacbdadacbcbdacbdbdadb
dbcadcdbcbdbdadbdadbcacbcacacbcabada
dbcbdacbcadbdacbdadbdacbcadbcacadacb
dbdacacbdadbcbcbcbcadbdadbcadbcadaca
dbdbcacadacabacbcadacbdadcdbdbdbcbca
dbdcdabacadadbcbdcdbcacacbcbdbdacaba
dcdacadadbcbcabacbcacbdbcbdbcadadadb
dcdbcadadbcbcadbcbcadabadbdcdbcacaba
dcdcdacabadbdbdacacbcacbdababadbcbdc
76317369490

</pre>