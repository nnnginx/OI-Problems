<p>���ǽ�����һ���ɱ��Ϊ $0, \dots , n-1$ �� $n$ ������ɵ��罻���硣�����е���Щ�Ի��Ϊ���ѡ���� $x$ ���˳�Ϊ $y$ ���˵����ѣ��� $y$ ����ͬʱҲ���Ϊ $x$ ���˵����ѡ�</p>
<p>��Щ�˽�ͨ�� $n$ ���׶μ���������磬�׶�Ҳ���Ϊ $0$ �� $n - 1$���� $i$ �����ڵ� $i$ ���׶μ��롣�ڽ׶� $0$��$0$ ���˼������粢��ΪΨһ���ˡ��˺� $n - 1$ ���׶εĸ����׶Σ�����һ���˻ᱻ�����˼��뵽�����У�����������˿��������������е��κ�һ���ˡ��ڽ׶� $i$ �� ($1 \leq i \leq n - 1$)���ý׶ε������˿������������ַ�ʽ֮һ�ѵ� $i$ ���˼��뵽�����У�</p>
<ul><li>IAmYourFriend������ $i$ ���˽���������˵����ѡ�</li>
<li>MyFriendsAreYourFriends������ $i$ ���˱�������˵�ǰ��ÿһ�����ѵ����ѡ� ע�⣬�����ʽ���Ὣ�� $i$ ���˱�������˵����ѡ�</li>
<li>WeAreYourFriends������ $i$ ���˱�������˵����ѣ�ͬʱҲ��������˵�ǰ��ÿһ�����ѵ����ѡ�</li>
</ul><p>�ڽ���������֮����������ѡһ�������������Ҳ����˵Ҫ��������ѡ��һ���ˡ���������֮��ͨ��ӵ�����Ƶ���Ȥ�����������Ӧ�����κ�һ�Ի�Ϊ���ѵ��ˡ�ÿ���˶�����һ������Ŀ��Ŷȣ���ʾΪһ������������������Ҫ�ҳ�һ�����Ŷ��ܺ�����������</p>
<h2>����</h2>
<p>�������׶ε������Լ�ÿ���˵Ŀ��Ŷ�ֵ�����ҳ�һ�����Ŷ��ܺ�������������ֻ��Ҫʵ�ֺ��� findSample��</p>
<ul><li>findSample(n, confidence, host, protocol)<ul><li>$n$: ����.</li>
<li>confidence: ��СΪ $n$ �����飻confidence[i]��ʾ�� $i$ ���˵Ŀ��Ŷȡ�</li>
<li>host: ��СΪ $n$ �����飻host[i] ��ʾ�׶� $i$ �������ˡ�</li>
<li>protocol: ��СΪ $n$ �����飻protocol[i] ��ʾ�ڽ׶� ($0 &lt; i &lt; n$) �����õķ�ʽ�Ĵ���: $0$ ���� IAmYourFriend��$1$ ���� MyFriendsAreYourFriends���� $2$ ���� WeAreYourFriends��</li>
<li>�����ڽ׶�$0$��û�������ˣ���� host[0] �� protocol[0] ��û�б�����ģ���������ĳ�����Ҳ��Ӧ�������ǡ�</li>
<li>�������Ӧ�÷����������Ŷ��ܺ͵����ֵ��</li>
</ul></li>
</ul><h2>������</h2>
<p>��Щ������ֻ��ʹ�����в��ַ�ʽ�����±���ʾ��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>������</th><th>��ֵ</th><th>$n$</th><th>���Ŷ�</th><th>���õķ�ʽ</th></tr></thead><tbody><tr><td>1</td><td>11</td><td>$2 \leq n \leq 10$</td><td>$1 \leq \text{confidence} \leq 1000000$</td><td>ȫ�����ַ�ʽ</td></tr><tr><td>2</td><td>8</td><td>$2 \leq n \leq 1000$</td><td>$1 \leq \text{confidence} \leq 1000000$</td><td>ֻ�� MyFriendsAreYourFriends</td></tr><tr><td>3</td><td>8</td><td>$2 \leq n \leq 1000$</td><td>$1 \leq \text{confidence} \leq 1000000$</td><td>ֻ�� WeAreYourFriends</td></tr><tr><td>4</td><td>19</td><td>$2 \leq n \leq 1000$</td><td>$1 \leq \text{confidence} \leq 1000000$</td><td>ֻ�� IAmYourFriend</td></tr><tr><td>5</td><td>23</td><td>$2 \leq n \leq 1000$</td><td>���п��Ŷ�ֵ��Ϊ $1$</td><td>ֻ�� MyFriendsAreYourFriends ��
IAmYourFriend ���ַ�ʽ</td></tr><tr><td>6</td><td>31</td><td>$2 \leq n \leq 100000$</td><td>$1 \leq \text{confidence} \leq 10000$</td><td>ȫ�����ַ�ʽ</td></tr></tbody></table></div>

<h2>ʵ��ϸ��</h2>
<p>����ֻ֧�� C/C++��</p>
<p>��ֻ���ύһ��Դ�ļ�ʵ�������ĺ�������������ӿ�����ѭ�����Ҫ���㻹Ҫ�ڸ��ļ��а���ͷ�ļ�friend.h��</p>
<pre><code class="sh_cpp">int findSample(int n, int confidence[], int host[], int protocol[]);</code></pre>
<h2>���ⷽʽ</h2>
<p>����ϵͳ����������¸�ʽ���������ݣ�</p>
<ul><li>�� $1$ ��: $n$</li>
<li>�� $2$ ��: $\text{confidence[0]}, \dots, \text{confidence[n-1]}$</li>
<li>�� $3$ ��: $\text{host[1]}, \text{protocol[1]}, \text{host[2]}, \text{protocol[2]}, \dots, \text{host[n-1]}, \text{protocol[n-1]}$</li>
</ul><p>����ϵͳ������� findSample �ķ���ֵ��</p>
<p><a href="/faq">����ʽ���͵���Ŀ��ô���ز���</a></p>
<p><strong>ʱ�����ƣ�</strong>$1\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$16\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20468/file/attachment.zip">����������������</a></p>
<p>ʲô��˵����1������6����ͬ�ģ�IOIԭ��Ҳ����ͬ�ģ���Ҫ������</p>
