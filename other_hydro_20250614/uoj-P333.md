<p>���뿼���ھ��С���õ���һ�ݲر�ͼ���ر�ͼ�ϱ���� $n$ �������ڵ��µı����ݣ�Ҳ�������� $n$ ��������֮��ɹ������� $m$ ����·�����ǵĳ��ȡ�</p>
<p>С����������ǰ���ھ����б������еı��ء����ǣ�ÿ�������ݾ�����涼��Զ��Ҳ����˵���ӵ����ͨһ����ĳ�������ݵĵ�·�Ǻ����ѵģ�������������֮��ĵ�·��������׺ܶࡣ</p>
<p>С���ľ��ĸж��˿����ھ�������̣������̾��������������ͨһ���ӵ��浽ĳ�������ݵ�ͨ����ͨ���ĸ�����������С����������</p>
<p>�ڴ˻����ϣ�С������Ҫ������ο��䱦����֮��ĵ�·���Ѿ�������ĵ�·��������ͨ�в����Ĵ��ۡ�ÿ�����һ���µ�·��С���ͻ��뿼�Ŷ�һ���ھ���ɸ�����·���ܵ���ı����ݵı��ء����⣬С�����뿪�����õ�·���������Ѿ����ھ���ı�����֮��ĵ�·�����ٿ�����</p>
<p>�¿���һ����·�Ĵ����ǣ�</p>
<p>������·�ĳ��� �� �������̰����ͨ�ı����ݵ�������·���ı������������ı����ݵ����������������̰����ͨ�ı����ݺ�������·���ı����ݣ���</p>
<p>�����д����ΪС��ѡ���������̴�ͨ�ı����ݺ�֮����ĵ�·��ʹ�ù����ܴ�����С������������Сֵ��</p>
<h2>�����ʽ</h2>
<p>��һ�������ÿո����������� $n$ �� $m$���������ݵĸ����͵�·����</p>
<p>������ $m$ �У�ÿ�������ÿո��������������ֱ�����һ����·���ӵ����������ݵı�ţ����Ϊ $1$~$n$������������·�ĳ��� $v$��</p>
<h2>�����ʽ</h2>
<p>�����һ�У�һ������������ʾ��С���ܴ��ۡ�</p>


<pre><code class="language-input1">4 5
1 2 1
1 3 3
1 4 1
2 3 4
3 4 1
</code></pre>


<pre><code class="language-output1">4
</code></pre>


<p><img class="img-responsive center-block" src="//img.uoj.ac/problem/333/333.png" style="width:250px;" alt="����"></p>
<p>С��ѡ���������̴�ͨ�� $1$ �ű����ݡ�С�������˵�· $1\rightarrow 2$���ھ��� $2$ �ű��ء������˵�· $1\rightarrow 4$���ھ��� $4$ �ű��ء��������˵�· $4\rightarrow 3$���ھ��� $3$ �ű��ء������ܴ���Ϊ��
$$\begin{array}{c}1\times 1\\ \small{(1\rightarrow 2)}\end{array}\begin{array}{c}+\\ \ \end{array}\begin{array}{c}1\times 1\\ \small{(1\rightarrow 4)}\end{array}\begin{array}{c}+\\ \ \end{array}\begin{array}{c}1\times 2\\ \small{(4\rightarrow 3)}\end{array}\begin{array}{c}=4\\ \ \end{array}$$</p>


<pre><code class="language-input2">4 5
1 2 1
1 3 3
1 4 1
2 3 4
3 4 2
</code></pre>


<pre><code class="language-output2">5
</code></pre>


<p><img class="img-responsive center-block" src="//img.uoj.ac/problem/333/333-2.png" style="width:250px;" alt="����"></p>
<p>С��ѡ���������̴�ͨ�� $1$ �ű����ݡ�С�������˵�· $1\rightarrow 2$���ھ��� $2$ �ű��ء������˵�· $1\rightarrow 3$���ھ��� $3$ �ű��ء��������˵�· $1\rightarrow 4$���ھ��� $4$ �ű��ء������ܴ���Ϊ��
$$\begin{array}{c}1\times 1\\ \small{(1\rightarrow 2)}\end{array}\begin{array}{c}+\\ \ \end{array}\begin{array}{c}3\times 1\\ \small{(1\rightarrow 3)}\end{array}\begin{array}{c}+\\ \ \end{array}\begin{array}{c}1\times 1\\ \small{(1\rightarrow 4)}\end{array}\begin{array}{c}=5\\ \ \end{array}$$</p>
<h2>������</h2>
<p>�������������ء�</p>
<h2>������Լ��</h2>
<ul><li>����20%�����ݣ�<ul><li>��֤������һ������$1\le n\le 8$��$v\le 5000$ �����е� $v$ ����ȡ�</li>
</ul></li>
<li>����40%�����ݣ�<ul><li>$1\le n\le 8$��$0\le m\le 1000$��$v\le 5000$ �����е� $v$ ����ȡ�</li>
</ul></li>
<li>����70%�����ݣ�<ul><li>$1\le n\le 8$��$0\le m\le 1000$��$v\le 5000$</li>
</ul></li>
<li>����100%�����ݣ�<ul><li>$1\le n\le 12$��$0\le m\le 1000$��$v\le 500000$</li>
</ul></li>
</ul><p><strong>ʱ�����ƣ�</strong>$1\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$256\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20759/file/attachment.zip">������������</a></p>
