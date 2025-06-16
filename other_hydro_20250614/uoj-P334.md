<p>Sylvia��һ���Ȱ�ѧϰ��Ů���ӡ�</p>
<p>ǰ��ʱ�䣬Sylvia�μ���ѧУ�ľ�ѵ��������֪����ѵ��ʱ����Ҫվ���� Sylvia���ڵķ������� $n\times m$ ��ѧ�������������Ϊ $n$������Ϊ $m$��</p>
<p>Ϊ�˱��ڹ����̹���ѵ����ʼʱ�����մ�ǰ���󣬴����ҵ�˳��������е�ѧ���� $1$ �� $n\times m$ �����˺��루�μ��������������������ʼʱ���� $i$ �е� $j$ �е�ѧ���ı���� $(i-1)\times m+j$��</p>
<p>Ȼ������ϰ�����ʱ�򣬾�������ѧ����Ϊ���ָ�����������Ҫ��ӡ���һ���У�һ�������� $q$ ������������¼���ÿһ������¼����������� $(x,y)$��$1\le x\le n$��$1\le y\le m$����������ʾ�� $x$ �е� $y$ �е�ѧ����ӡ�</p>
<p>����ѧ����Ӻ󣬶����г�����һ����λ��Ϊ�˶�������룬�̹ٻ������´�����������ָ�</p>
<ol><li>�����롣��ʱ��һ�б��ֲ���������ѧ���������ȱ�����ѷ���������ָ��֮�󣬿�λ�ڵ� $x$ �е� $m$ �С�</li>
<li>��ǰ���롣��ʱ��һ�б��ֲ���������ѧ����ǰ���ȱ�����ѷ���������ָ��֮�󣬿�λ�ڵ� $n$ �е� $m$ �С�</li>
</ol><p>�̹ٹ涨���������������ѧ��ͬʱ��ӡ�����ǰһ����ӵ�ѧ�����֮����һ��ѧ��������ӡ������ÿһ����ӵ�ѧ��Ҫ���ʱ�����������ҽ��е� $n$ �е� $m$ ��һ����λ����ʱ���ѧ������Ȼ��������λ�á�</p>
<p>��Ϊվ������ĺ����ģ�����Sylvia��Ҫ����ÿһ������¼��У���ӵ�ͬѧ�ı���Ƕ��١�</p>
<p>ע�⣺ÿһ��ͬѧ�ı�Ų�����������¼��ķ������ı䣬�ڷ�������¼�������ͬѧ�ı�ſ���������ġ�</p>
<h2>�����ʽ</h2>
<p>���빲 $q+1$ �С�</p>
<p>�� $1$ �а��� $3$ ���ÿո�ָ��������� $n,m,q$����ʾ�����С�� $n$ �� $m$ �У�һ�������� $q$ ���¼���</p>
<p>������ $q$ �а����¼�����˳�������� $q$ ���¼���ÿһ������������ $x,y$����һ���ո�ָ�����ʾ�������¼�����ӵ�ѧ����ʱ���ڵ� $x$ �е� $y$ �С�</p>
<h2>�����ʽ</h2>
<p>�����¼������˳��ÿһ���¼����һ��һ����������ʾ�������¼������ѧ���ı�š�</p>


<pre><code class="language-input1">2 2 3
1 1
2 2
1 2
</code></pre>


<pre><code class="language-output1">1
1
4
</code></pre>


<p>$$\begin{bmatrix}1&amp;2\\3&amp;4\end{bmatrix}\Rightarrow\begin{bmatrix}&amp;2\\3&amp;4\end{bmatrix}\Rightarrow\begin{bmatrix}2&amp;\\3&amp;4\end{bmatrix}\Rightarrow\begin{bmatrix}2&amp;4\\3&amp;\end{bmatrix}\Rightarrow\begin{bmatrix}2&amp;4\\3&amp;1\end{bmatrix}$$</p>
<p>$$\begin{bmatrix}2&amp;4\\3&amp;1\end{bmatrix}\Rightarrow\begin{bmatrix}2&amp;4\\3&amp;\end{bmatrix}\Rightarrow\begin{bmatrix}2&amp;4\\3&amp;\end{bmatrix}\Rightarrow\begin{bmatrix}2&amp;4\\3&amp;\end{bmatrix}\Rightarrow\begin{bmatrix}2&amp;4\\3&amp;1\end{bmatrix}$$</p>
<p>$$\begin{bmatrix}2&amp;4\\3&amp;1\end{bmatrix}\Rightarrow\begin{bmatrix}2&amp;\\3&amp;1\end{bmatrix}\Rightarrow\begin{bmatrix}2&amp;\\3&amp;1\end{bmatrix}\Rightarrow\begin{bmatrix}2&amp;1\\3&amp;\end{bmatrix}\Rightarrow\begin{bmatrix}2&amp;1\\3&amp;4\end{bmatrix}$$</p>
<p>�жӵĹ�������ͼ��ʾ��ÿһ��������һ���¼��� </p>
<p>�ڵ�һ���¼��У����Ϊ $1$ ��ͬѧ��ӣ���ʱ��λ�ڵ�һ�е�һ�С���������ͬѧ������룬��ʱ���Ϊ $2$ ��ͬѧ�����ƶ�һ������λ�ƶ�����һ�еڶ��С�Ȼ������ͬѧ���ϱ��룬��ʱ���Ϊ $4$ ��ͬѧ����һ������ʱ��λ�ƶ����ڶ��еڶ��С������Ϊ $1$ ��ͬѧ���������λ�С�</p>
<h2>������</h2>
<p>�������������ء�</p>
<h2>������Լ��</h2>
<div class="table-responsive">
 <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th rowspan="1">���Ե���</th>
    <th rowspan="1">$n$</th>
    <th rowspan="1">$m$</th>
    <th rowspan="1">$q$</th>
    <th rowspan="1">����Լ��</th>
   </tr></thead><tbody><tr><td rowspan="1">1,2</td>
    <td rowspan="3">$\leq 1000$</td>
    <td rowspan="3">$\leq 1000$</td>
    <td rowspan="5">$\leq 500$</td>
    <td rowspan="5">��</td>
   </tr><tr><td rowspan="1">3,4</td>
   </tr><tr><td rowspan="1">5,6</td>
   </tr><tr><td rowspan="1">7,8</td>
    <td rowspan="2">$\leq 5\times 10^4$</td>
    <td rowspan="2">$\leq 5\times 10^4$</td>
   </tr><tr><td rowspan="1">9,10</td>
   </tr><tr><td rowspan="1">11,12</td>
    <td rowspan="2">$=1$</td>
    <td rowspan="1">$\le 10^5$</td>
    <td rowspan="1">$\le 10^5$</td>
    <td rowspan="3">�����¼� $x=1$</td>
   </tr><tr><td rowspan="1">13,14</td>
    <td rowspan="2">$\le 3\times 10^5$</td>
    <td rowspan="2">$\le 3\times 10^5$</td>
   </tr><tr><td rowspan="1">15,16</td>
    <td rowspan="1">$\le 3\times 10^5$</td>
   </tr><tr><td rowspan="1">17,18</td>
    <td rowspan="1">$\le 10^5$</td>
    <td rowspan="1">$\le 10^5$</td>
    <td rowspan="1">$\le 10^5$</td>
    <td rowspan="2">��</td>
   </tr><tr><td rowspan="1">19,20</td>
    <td rowspan="1">$\le 3\times 10^5$</td>
    <td rowspan="1">$\le 3\times 10^5$</td>
    <td rowspan="1">$\le 3\times 10^5$</td>
   </tr></tbody></table></div>

<p>���ݱ�֤ÿһ���¼����� $1\le x\le n,1\le y\le m$��</p>
<p><strong>ʱ�����ƣ�</strong>$2\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20760/file/attachment.zip">������������</a></p>
