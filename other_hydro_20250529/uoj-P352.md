<p>����İ����£�SingleDog�����ڽ����˼��������ڲ������Ǿ��ȵķ��֣��������ĵĺ��ġ���AlphaGo����̨�������ڵĵط�����Ȼ��һ����ά�ռ䣡</p>
<p>�򵥵�˵�������� $n \leq 5$ ά�ռ���һ���㼯��λ��һ�� $n$ ά������ķ����ڲ��������ڲ����������� $l_i\le x_i \le r_i$ �ĵ� $(x_1,x_2,\cdots,x_n)$ ���ɣ���������������λ�ڷ����ڲ������� $x_i - x_j \ge a_{i,j}$ �ĵ�$(x_1, x_2 \cdots,x_n)$ ���ɣ����� $l_i,r_i,a_{i,j}$ ��Ϊ������������</p>
<p>����SingleDog����֪���ľ���������ĵġ������ռ���������ı�����</p>
<p>Ϊ�˷���������⣬һ��<strong>�ȼ�</strong>����Ŀ�����ǣ�</p>
<p>�� $x_1,x_2,\cdots,x_n$ �� $n$ ��ʵ�����������е� $i$ ������ $x_i$ ������ $[l_i,r_i]$ �ھ���������ɣ����� $l_i$ �� $r_i$ ��Ϊ������������ $l_i\le r_i$��Լ�� $l_i=r_i$ ʱ��$[l_i,r_i]$ ��ʾ��Ԫ�ؼ��� $\{l_i\}$����</p>
<p>���� $n\times n$ ���������󣬾����ÿ��Ԫ�ش���һ��Լ�������е� $i$ �е� $j$ �е�Ԫ�� $a_{i,j}$ ����Լ��
$$x_i-x_j\ge a_{i,j}$$</p>
<p>���� $n\times n$ ��Լ��ͬʱ������ĸ��ʡ�</p>
<h2>�����ʽ</h2>
<p>��һ�а���һ�������� $n$����ʾʵ������������</p>
<p>������ $n$ �У��� $i$ ���������� $l_i,r_i$�������� $i$ �����䡣</p>
<p>������ $n$ �У�ÿ�� $n$ �������������������� $a_{i,j}$��</p>
<h2>�����ʽ</h2>
<p>���һ�У�����һ��ʵ������ʾ����ĸ��ʡ�</p>
<p>��Ĵ���ο��𰸵ľ��������� $10^{-7}$ ʱ����Ϊ����ȷ�ġ�</p>


<pre><code class="language-input1">1
0 10
-10
</code></pre>


<pre><code class="language-output1">1.000000000000
</code></pre>


<p>���۱��� $x_1$ ��ֵ�Ƕ��٣�Լ�� $x_1-x_1\ge-10$ �������������Լ���ĸ���Ϊ $1$��</p>


<pre><code class="language-input2">2
5 5
3 7
0 1
-3 0
</code></pre>


<pre><code class="language-output2">0.2500000000
</code></pre>


<p>$x_1=5$��$3\le x_2\le 7$������ $3\le x_2\le 4$ ʱ����ͬʱ��������Լ��������������Լ���ĸ���Ϊ ${1\over 4}=0.25$��</p>


<pre><code class="language-input3">2
4 5
3 6
-10 2
-10 -10
</code></pre>


<pre><code class="language-output3">0.0000000000
</code></pre>


<p>���� $4\le x_1\le 5$��$3\le x_2\le 6$ �� $x_1,x_2$ ������������ֻ��һ��ֵ $x_1=5,x_2=3$ ������Լ���ģ�������Լ���ĸ���Ϊ $0$��</p>


<pre><code class="language-input4">2
3 10
0 8
-1 1
-7 0
</code></pre>


<pre><code class="language-output4">0.5982142857
</code></pre>


<p>����Լ���ĸ���Ϊ ${67\over 112}$��������Ĵ�Ӧ���� $[{67\over 112}-10^{-7},{67\over 112}+10^{-7}]$ ��Χ�ڡ�</p>


<pre><code class="language-input5">3
0 10
2 10
2 9
0 -9 -10
4 0 -3
1 -4 0
</code></pre>


<pre><code class="language-output5">0.1491071429
</code></pre>



<pre><code class="language-input6">4
0 5
0 9
4 10
0 5
0 -8 -9 -5
1 0 -4 3
1 -6 0 3
-4 -10 -10 0
</code></pre>


<pre><code class="language-output6">0.2622839506
</code></pre>



<pre><code class="language-input7">5
0 10
0 10
4 4
0 9
0 7
-10 -9 -10 -10 -10
-10 -10 2 -10 -10
-10 -10 -10 1 -10
-10 -10 -10 -10 -5
-10 -10 -10 -10 -10
</code></pre>


<pre><code class="language-output7">0.1191269841
</code></pre>



<pre><code class="language-input8">5
0 2
1 8
7 10
2 7
6 10
0 -10 -10 -9 -10
-10 0 -7 -4 -8
3 3 0 1 -6
3 -6 -5 0 -5
-2 3 -9 1 0
</code></pre>


<pre><code class="language-output8">0.1713095238
</code></pre>

<h2>������Լ��</h2>
<p>����һЩԭ�򣬱���ʹ��������ԡ�ÿ�������������ɸ����Ե㣬��Ϊ 8 ����������ֻ��ͨ��һ������������в��Ե���ܵõ����������ķ�����</p>
<div class="table-responsive">
 <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>������</th>
    <th>��ֵ</th>
    <th>$n$</th>
    <th>��������</th>
   </tr></thead><tbody><tr><td>1</td>
    <td>5</td>
    <td>$=1$</td>
    <td>��</td>
   </tr><tr><td>2</td>
    <td>10</td>
    <td rowspan="3">$=2$</td>
    <td>$l_1=r_1$</td>
   </tr><tr><td>3</td>
    <td>20</td>
    <td>�� $j\ne i+1$���� $a_{i,j}=-10$</td>
   </tr><tr><td>4</td>
    <td>15</td>
    <td rowspan="3">��</td>
   </tr><tr><td>5</td>
    <td>10</td>
    <td>$=3$</td>
   </tr><tr><td>6</td>
    <td>10</td>
    <td>$=4$</td>
   </tr><tr><td>7</td>
    <td>20</td>
    <td rowspan="2">$=5$</td>
    <td>�� $j\ne i+1$���� $a_{i,j}=-10$</td>
   </tr><tr><td>8</td>
    <td>10</td>
    <td>��</td>
   </tr></tbody></table></div>

<p>�����������ݣ�$1\le n\le 5$��$0\le l_i\le r_i\le 10$��$-10\le a_{i,j}\le 10$��</p>
<p><strong>ʱ�����ƣ�</strong>$1\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$256\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20778/file/attachment.zip">������������</a></p>
