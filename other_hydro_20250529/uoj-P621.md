<p>Bitaro ��һλ����������ƾ�����רҵ���ߡ�������ٰ�һ�ι��ʳ�����ƾ�����Bitaro ׼��дһƪ���±������¡�</p>
<p>��ξ������� $N$ ��ѡ�ֲμӣ����Ǵ� $1$ �� $N$ ��š�ÿ��ѡ�ֶ���һ�� <strong>rating</strong> ���������ڳ�����ƾ����е�������rating ��һ���� $1$ �� $10^9$ ֮����������������ˣ���</p>
<p>Bitaro �Ѿ��ɷ���ѡ���ǡ��������������Ϣ��</p>
<ul>
<li>ѡ�� $i\ (1\le i\le N)$ �� rating ���ڵ���ѡ�� $A_i$��������ܻ���� $A_i=i$ �������</li>
</ul>
<p>�ڲɷú�Bitaro �ӹ��� rating ϵͳ�Ĺ�˾�������ѡ�ֵ� rating �б��б���д��������Ϣ��</p>
<ul>
<li>ѡ�� $i\ (1\le i\le N)$ �� rating ���� $H_i$��</li>
</ul>
<p>Bitaro ��ͼ����������Ϣдһƪ������Ȼ����rating �б���ѡ�ֵ� rating ���ݿ������д���ġ�</p>
<p>��Ϊ�ظ������Ͼ�Ҫ���ˣ�Bitaro �Ѿ�û��ʱ��ȥ��ȡ��ȷ�� rating �б��ˡ���ˣ�Bitaro ���������б���ĳЩѡ�ֵ� rating ���ݣ�ʹ���б���� rating ������ɷ��еõ�����Ϣì�ܡ������б���ѡ�� $i\ (1\le i\le N)$ �� rating �Ļ���Ϊ $C_i$��Ҳ����˵��Bitaro �����ڻ��� $C_i$ �Ĵ����£����б���ѡ�� $i$ �� rating ����Ϊ $1$ �� $10^9$ ֮��������������������ˣ���Ϊ�˸��Ͻظ��գ�Bitaro ��Ҫ��С������ rating ���ܻ��ѡ�</p>
<p>����ѡ�������ɷ��л�õ���Ϣ��rating �б�͸���ÿ��ѡ�� rating �Ļ��ѡ�дһ���������ʹ�� rating �б���ɷû����Ϣì�ܵ�����£����� rating ����С�ܻ��ѡ�</p>
<h2>�����ʽ</h2>
<p>��һ��һ������ $N$��</p>
<p>������ $N$ �У�ÿ���������� $A_i,H_i,C_i$��</p>
<h2>�����ʽ</h2>
<p>���һ��һ����������ʾ��С�ܻ��ѡ�</p>


<pre><code class="language-input1">6
1 6 5
1 3 6
1 8 4
3 4 9
2 2 5
2 5 6
</code></pre>


<pre><code class="language-output1">14
</code></pre>


<p>��� Bitaro �����·�������ѡ�ֵ� rating����ô�õ����б�Ͳ�����ɷ��еõ�����Ϣì���ˡ�</p>
<ul>
<li>��ѡ�� $1$ �� rating �� $6$ ��Ϊ $1$������Ϊ $5$��</li>
<li>��ѡ�� $3$ �� rating �� $8$ ��Ϊ $4$������Ϊ $4$��</li>
<li>��ѡ�� $5$ �� rating �� $2$ ��Ϊ $10^9$������Ϊ $5$��</li>
</ul>
<p>�ܻ���Ϊ $5+4+5=14$����Ϊ������С���ܻ��ѣ�������� $14$��</p>
<p>������������������ $1,2,3$ �����ơ�</p>


<pre><code class="language-input2">5
1 1 1
2 2 1
4 3 1
3 3 1
4 3 1
</code></pre>


<pre><code class="language-output2">0
</code></pre>


<p>�����������У��б���ѡ�ֵ� rating ��ɷ��л�õ���Ϣ��ì�ܣ������С�ܻ���Ϊ $0$����� $0$��</p>
<h2>������</h2>
<p>������������������ $1,2,3$ �����ơ�</p>

<pre><code class="language-input2">20
1 7 381792936
1 89 964898447
1 27 797240712
3 4 299745243
2 18 113181438
2 20 952129455
4 34 124298446
4 89 33466733
7 40 109601410
5 81 902931267
2 4 669879699
8 23 785166502
8 1 601717183
8 26 747624379
1 17 504589209
9 24 909134233
16 56 236448090
8 94 605526613
5 90 481898834
9 34 183442771
</code></pre>


<pre><code class="language-output2">2711043927
</code></pre>



<pre><code class="language-input4">20
15 62 418848971
13 5 277275513
14 60 80376452
12 14 256845164
12 42 481331310
6 86 290168639
3 98 947342135
3 19 896070909
16 39 48034188
8 29 925729089
18 97 420006994
13 51 454182928
19 61 822405612
13 37 148425187
15 77 474094143
14 27 272926693
18 43 566552069
9 93 790433300
10 73 61654171
14 28 334498030
</code></pre>


<pre><code class="language-output4">4012295156
</code></pre>

<h2>������Լ��</h2>
<p>����ȫ�����ݣ����㣺</p>
<ul>
<li>$2\le N\le 2\times 10^5$</li>
<li>$1\le A_i\le N\ (1\le i\le N)$</li>
<li>$1\le H_i,C_i\le 10^9\ (1\le i\le N)$</li>
</ul>
<p>��ϸ�����񸽼����Ƽ���ֵ���±���ʾ��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">��������</th>
<th style="text-align:center;">��ֵ</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$N\le 5\ 000,\ A_1=1,\ A_i\le i-1\ (2\le i\le N)$</td>
<td style="text-align:center;">$14$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$A_1=1,\ A_i\le i-1\ (2\le i\le N)$</td>
<td style="text-align:center;">$65$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">�޸�������</td>
<td style="text-align:center;">$21$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>ʱ�����ƣ�$\texttt{2s}$</strong></p>
<p><strong>�ռ����ƣ�$\texttt{512MB}$</strong></p>
<h2>����</h2>
<p><a href="./21022/file/attachment.zip">������������</a></p>
