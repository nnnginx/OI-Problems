<p>è���³���̨���е�һ���������㡣����³�ϵͳ����һ�����ι����һ���³�վ�� $n$ �����Ϊ $1$ �� $n$ ���³�����Щ�³��Թ̶��ķ����ڹ����ѭ�����С����³� $i$ �����³�վ֮����һ�������³�վ���³������� $i + 1$ ��$i &lt; n$ ʱ�����������³� $1$��$i = n$ ʱ����</p>
<p>�³����ܻᷢ�����ϡ����˵��ǣ����������޶���󱸵Ŀ����³�����������Ϊ $n + 1, n + 2$ �ȵȡ���ĳ���³���������ʱ�����ǻ��ڹ���ϵ�ͬһλ������ǰһ�������³��滻����Ҳ����˵�������С�Ŀ����³����ٸ����ӣ������ǰ�������³����³� $1$ �����˹��ϣ���ô���ǽ����³� $6$ ���滻����</p>
<p>��ϲ��ȥ�³�վ�Ϲ۲��³���վ��һ���³����������³���վ�����γɵ� $n$ ���³���ŵ����С����㵽���³�վ֮ǰ���п��ܻ���һ������³��������ϣ����ұ��滻��������������۲�������ǲ������³��������ϵġ�</p>
<p>ע�⣬�ڹ���ϵ���ͬһ���³����п��ܸ��������³����У���ȡ���ڵ��㵽�³�վʱ�����³����ȹ�վ���ٸ����ӣ����û���κ��³��������ϣ���ô $(2, 3, 4, 5, 1)$ �� $(4, 5, 1, 2, 3)$ ���������³����У����� $(4, 3, 2, 5, 1)$ �������ǣ���Ϊ�³��Ĵ������󣩡�</p>
<p>����³� $1$ �������ϣ���ô���ǿ��ܻ�۲쵽�³����� $(4, 5, 6, 2, 3)$����������³� $4$ �������϶��������³� $7$ �滻�������п��ܻ�۲쵽�³����� $(6, 2, 3, 7, 5)$������³� $7$ �ڴ˺������϶��������³� $8$ �滻������ô���ھ��п��ܻ�۲쵽�³����� $(3, 8, 5, 6, 2)$��</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>�����³�</th><th>���³�</th><th>���ܵ��³�����</th></tr></thead><tbody><tr><td>$1$</td><td>$6$</td><td>$(4, 5, 6, 2, 3)$</td></tr><tr><td>$4$</td><td>$7$</td><td>$(6, 2, 3, 7, 5)$</td></tr><tr><td>$7$</td><td>$8$</td><td>$(3, 8, 5, 6, 2)$</td></tr></tbody></table></div>

<p>һ���滻������һ���ɹ����³������ɵ����У����������Ϸ���������ͬ����ǰ��������У��滻������ $(1, 4, 7)$�����һ���滻���� $r$ ��Ӧ�Ĺ��Ϸ����������ɴ��п��ܹ۲쵽�³����� $g$���ͳ��滻���� $r$ �����³����� $g$��</p>
<h2>�³����м��</h2>
<p>��ǰ�����������У��������ĳ�����������Ƿ���һ���³����С��±����˵������Щ�������³����ж���Щ���ǡ�����Ҫʵ��һ������ valid��</p>
<ul><li>valid(n, inputSeq)<ul><li>$n$: �������г���</li>
<li>inputSeq: ��СΪ $n$ �����飻inputSeq[i] ���������еĵ� $i$ ��Ԫ�أ����� $0 \leq i \leq n - 1$��</li>
<li>������������һ���³�����ʱ������Ӧ���� $1$�����򷵻� $0$��</li>
</ul></li>
</ul><h2>������1, 2, 3</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>������</th><th>��ֵ</th><th>$n$</th><th>inputSeq</th></tr></thead><tbody><tr><td>1</td><td>5</td><td>$n \leq 100$</td><td>�� $1$ �� $n$ ����ǡ�ó���һ��</td></tr><tr><td>2</td><td>5</td><td>$n \leq 100000$</td><td>$1 \leq \text{inputSeq[i]} \leq n$</td></tr><tr><td>3</td><td>10</td><td>$n \leq 100000$</td><td>$1 \leq \text{inputSeq[i]} \leq 250000$</td></tr></tbody></table></div>

<h2>����</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>������</th><th>inputSeq</th><th>����ֵ</th><th>��ע</th></tr></thead><tbody><tr><td>1</td><td>$(1, 2, 3, 4, 5, 6, 7)$</td><td>$1$</td><td></td></tr><tr><td>1</td><td>$(3, 4, 5, 6, 1, 2)$</td><td>$1$</td><td></td></tr><tr><td>1</td><td>$(1, 5, 3, 4, 2, 7, 6)$</td><td>$0$</td><td>$1$����ǡ�ó�����$5$֮ǰ</td></tr><tr><td>1</td><td>$(4, 3, 2, 1)$</td><td>$0$</td><td>$4$ ����ǡ�ó����� $3$ ֮ǰ</td></tr><tr><td>2</td><td>$(1, 2, 3, 4, 5, 6, 5)$</td><td>$0$</td><td>�������³���Ŷ��� $5$</td></tr><tr><td>3</td><td>$(2, 3, 4, 9, 6, 7, 1)$</td><td>$1$</td><td>�滻������ $(5, 8)$</td></tr><tr><td>3</td><td>$(10, 4, 3, 11, 12)$</td><td>$0$</td><td>$4$ ����ǡ�ó����� $3$ ֮ǰ</td></tr></tbody></table></div>

<h2>�滻����</h2>
<p>�ڽ������������������У�����빹��һ���ܹ����ɸ����³����еĿ��ܵ��滻���С����������������滻���ж����ԡ�����Ҫʵ��һ������ replacement��</p>
<ul><li>replacement(n, gondolaSeq, replacementSeq)<ul><li>$n$ ���³����еĳ��ȡ�</li>
<li>gondolaSeq: ��СΪ $n$ �����飻gondolaSeq ��֤��һ���³����У��� gondolaSeq[i] �������еĵ� $i$ ��Ԫ�أ����� $0 \leq i \leq n - 1$��</li>
<li>����Ӧ�����滻���еĳ��� $l$��</li>
<li>replacementSeq: һ���㹻����ܴ����滻���е����飻��Ӧ�����滻�����еĵ� $i$ ��Ԫ�ش�ŵ� replacementSeq[i] ��Ϊ���ؽ�������� $0 \leq i \leq l - 1$��</li>
</ul></li>
</ul><h2>������4, 5, 6</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>������</th><th>��ֵ</th><th>$n$</th><th>gondolaSeq</th></tr></thead><tbody><tr><td>4</td><td>5</td><td>$n \leq 100$</td><td>$1 \leq \text{gondolaSeq[i]} \leq n + 1$</td></tr><tr><td>5</td><td>10</td><td>$n \leq 1000$</td><td>$1 \leq \text{gondolaSeq[i]} \leq 5000$</td></tr><tr><td>6</td><td>20</td><td>$n \leq 100000$</td><td>$1 \leq \text{gondolaSeq[i]} \leq 250000$</td></tr></tbody></table></div>

<h2>����</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>������</th><th>gondolaSeq</th><th>����ֵ</th><th>replacementSeq</th></tr></thead><tbody><tr><td>4</td><td>$(3, 1, 4)$</td><td>$1$</td><td>$(2)$</td></tr><tr><td>4</td><td>$(5, 1, 2, 3, 4)$</td><td>$0$</td><td>$()$</td></tr><tr><td>5</td><td>$(2, 3, 4, 9, 6, 7, 1)$</td><td>$2$</td><td>$(5, 8)$</td></tr></tbody></table></div>

<h2>�滻���м���</h2>
<p>�ڽ��������ĸ��������У��������������ܹ����ɸ������У��п������³����У�Ҳ�п��ܲ��ǣ��Ŀ����滻���е���Ŀ��������� $1000000009$ ȡģ������Ҫʵ��һ������ countReplacement��</p>
<ul><li>countReplacement(n, inputSeq)<ul><li>$n$: �������еĳ��ȡ�</li>
<li>inputSeq: ��СΪ $n$ �����飻inputSeq[i] ���������еĵ� $i$ ��Ԫ�أ����� $0 \leq i \leq n - 1$��</li>
<li>�������������һ���³����У�������ܹ����ɸ��³����еĿ��ܵ��滻���е���Ŀ���п��ܻ�ǳ��󣩣�<strong>Ȼ�󽫸���ֵ�� $1000000009$ ȡģ��Ϊ����ֵ</strong>������������в���һ���³����У�����Ӧ���� $0$���������������һ���³����У�����û���³��������ϣ�����Ӧ���� $1$��</li>
</ul></li>
</ul><h2>������7, 8, 9, 10</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>������</th><th>��ֵ</th><th>$n$</th><th>inputSeq</th></tr></thead><tbody><tr><td>7</td><td>5</td><td>$4 \leq n \leq 50$</td><td>$1 \leq \text{inputSeq[i]} \leq n + 3$</td></tr><tr><td>8</td><td>15</td><td>$4 \leq n \leq 50$</td><td>$1 \leq \text{inputSeq[i]} \leq 100$����ʼ�³� $1, \dots, n$ �������� $n - 3$ �����ᷢ�����ϡ�</td></tr><tr><td>9</td><td>15</td><td>$n \leq 100000$</td><td>$1 \leq \text{inputSeq[i]} \leq 250000$</td></tr><tr><td>10</td><td>10</td><td>$n \leq 100000$</td><td>$1 \leq \text{inputSeq[i]} \leq 1000000000$</td></tr></tbody></table></div>

<h2>����</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>������</th><th>inputSeq</th><th>����ֵ</th><th>�滻����</th></tr></thead><tbody><tr><td>7</td><td>$(1, 2, 7, 6)$</td><td>$2$</td><td>$(3, 4, 5)$ �� $(4, 5, 3)$</td></tr><tr><td>8</td><td>$(2, 3, 4, 12, 6, 7, 1)$</td><td>$1$</td><td>$(5, 8, 9, 10, 11)$</td></tr><tr><td>9</td><td>$(4, 7, 4, 7)$</td><td>$0$</td><td>inputSeq����һ���³�����</td></tr><tr><td>10</td><td>$(3, 4)$</td><td>$2$</td><td>$(1, 2)$ �� $(2, 1)$</td></tr></tbody></table></div>

<h2>ʵ��ϸ��</h2>
<p>����ֻ֧�� C/C++��</p>
<p>��ֻ���ύһ��Դ�ļ�ʵ�������ĺ������ڸ��ļ���Ӧʵ��ǰ������������������������ֻ�������еĲ���������ҲҪ����ȫ��������������ѭ����������ӿڡ��㻹��Ҫ����ͷ�ļ� gondola.h��</p>
<pre><code class="sh_cpp">int valid(int n, int inputSeq[]);
int replacement(int n, int gondolaSeq[], int replacementSeq[]);
int countReplacement(int n, int inputSeq[]);</code></pre>
<h2>���ⷽʽ</h2>
<p>����ϵͳ����������¸�ʽ���������ݣ�</p>
<ul><li>�� $1$ ��: $T$����ĳ�����Ҫ������������ţ�$ 1 \leq T \leq 10$����</li>
<li>�� $2$ ��: $n$���������еĳ��ȡ�</li>
<li>�� $3$ ��: ��� $T$ ��4��5����6�����а��� $\text{gondolaSeq[0]}, \dots, \text{gondolaSeq[n-1]}$��������а���$\text{inputSeq[0]}, \dots, \text{inputSeq[n-1]}$��</li>
</ul><p><a href="/faq">����ʽ���͵���Ŀ��ô���ز���</a></p>
<p><strong>ʱ�����ƣ�</strong>$1\texttt{s}$</p>
<p><strong>�ռ����ƣ�</strong>$256\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20467/file/attachment.zip">����������������</a></p>
