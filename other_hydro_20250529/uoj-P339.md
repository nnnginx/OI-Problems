<h2>��Ŀ����</h2>
<p>СY��һ���������ɵ�OIer��������������ģ�͡�</p>
<p>СY�Ķ�����ģ���У�ÿ����㶼����һ����ţ�СY������ϲ����һ��������ģ�͹�����ǽ�ϣ������������棬���������ֱ������������·������·���������Ҳ���������������ҹ���Ϊ�������ģ�͸������ۣ�СYѡ����һ������ö��������������������С�����ҷ�������ν���������С������ָ��������Ľ�������е��ֵ�����С��</p>
<p>һ�죬���ģ�Ͳ�С�ı������˵��ϣ����˵��ǣ����н��ͱ߶�ûˤ�����������벻�����ģ��ԭ������ô���ҵ��ˣ�Ҳ����˵�����벻���������ڵ�ı���ˡ�</p>
<p>СY���æ��׼���廪��ѵ������û̫��ʱ�䴦�������飬��ֻ���ҵ�ͬ���������ɵ����æ��ԭ���Ķ�����ģ�͡�</p>
<h2>��Ŀ����</h2>
<p>����СY�Ķ�����ģ�ͣ����ı��Ϊ $1$ ~ $n$ ������Ҫ��������ܵ���С���������������СY����İں�����ģ�͡�</p>
<h2>�����ʽ</h2>
<p>�ӱ�׼����������ݡ�</p>
<p>��һ��Ϊһ�������� $n$ ����ʾ��ĸ�����</p>
<p>��� $n$ �У�ÿ�����ɸ�������</p>
<p>�� $i+1$ �еĵ�һ������Ϊ $k_i$ ����ʾ���Ϊ $i$ �Ľ��Ķ�������� $k_i$ ������ $a_{i,j}$ ����ʾ���Ϊ $i$ �Ľ������Ϊ $a_{i,j}$ �Ľ��֮����һ���ߡ�</p>
<p>ͬһ���������������Ԫ��֮�䣬��ǡ��һ���ո������</p>
<h2>�����ʽ</h2>
<p>�������׼�����</p>
<p>�����һ�У� $n$ ����������ʾ�ֵ�����С�����������</p>


<pre><code class="language-input1"><code class="sh_plain">4
3 2 3 4
1 1
1 1
1 1</code>
</code></pre>

<pre><code class="language-output1"><code class="sh_plain">2 1 3 4</code>
</code></pre>

<p>������һ�����Ž����£�</p>
<p><img class="img-responsive center-block" src="//img.uoj.ac/problem/339/339-optimal.webp" style="width:120px;" alt="���Ž�"></p>
<p>���н��$4$Ϊ�������$1$Ϊ���$4$������ӣ����$2,3$�ֱ�Ϊ���$1$�����Ҷ��ӡ�</p>
<h2>������Լ��</h2>
<p>���⹲20�����Ե㣬ÿ�����Ե�5�֡��������Ե�����ݷ�Χ���£�</p>
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th rowspan="1">���Ե���</th><th rowspan="1">$n \le$</th><th rowspan="1">$k_i$</th><th rowspan="1">��������</th></tr></thead><tbody><tr><td rowspan="1">1</td><td rowspan="1">5</td><td rowspan="8">1,2,3</td><td rowspan="8">��</td></tr><tr><td rowspan="1">2</td><td rowspan="1">10</td></tr><tr><td rowspan="1">3</td><td rowspan="1">15</td></tr><tr><td rowspan="1">4</td><td rowspan="1">20</td></tr><tr><td rowspan="1">5</td><td rowspan="1">100</td></tr><tr><td rowspan="1">6</td><td rowspan="1">1000</td></tr><tr><td rowspan="1">7</td><td rowspan="1">2000</td></tr><tr><td rowspan="1">8</td><td rowspan="1">5000</td></tr><tr><td rowspan="1">9</td><td rowspan="1">1000000</td><td rowspan="4">1,2</td><td rowspan="1">���$i$����$i-1$����</td></tr><tr><td rowspan="1">10</td><td rowspan="1">100000</td><td rowspan="3">��</td></tr><tr><td rowspan="1">11</td><td rowspan="1">300000</td></tr><tr><td rowspan="1">12</td><td rowspan="1">1000000</td></tr><tr><td rowspan="1">13</td><td rowspan="1">100000</td><td rowspan="2">1,3</td><td rowspan="1">��֤�������</td></tr><tr><td rowspan="1">14</td><td rowspan="1">1000000</td><td rowspan="1">��</td></tr><tr><td rowspan="1">15</td><td rowspan="1">20000</td><td rowspan="6">1,2,3</td><td rowspan="2">��֤�������</td></tr><tr><td rowspan="1">16</td><td rowspan="1">200000</td></tr><tr><td rowspan="1">17</td><td rowspan="1">100000</td><td rowspan="4">��</td></tr><tr><td rowspan="1">18</td><td rowspan="1">500000</td></tr><tr><td rowspan="1">19</td><td rowspan="1">800000</td></tr><tr><td rowspan="1">20</td><td rowspan="1">1000000</td></tr></tbody></table><p>������ݵ����ɷ�ʽ���£�</p>
<p>���ڵ�13�����Ե㣬��һ��������������ʼ��ÿ�����һ�����ϵĶ���Ϊ1�Ľ�㣨��Ҷ��㣩��������������ֱ֮�������Ľ�㣬ֱ����������� $n$ ����㡣��Ȼ����������Ե��У�$n$ ��һ��ż����</p>
<p>���ڵ�15�͵�16�����Ե㣬��һ��һ����������ʼ��ÿ�����һ�����ϵĶ���������2�Ľ�㣬������һ����ֱ֮�������Ľ�㣬ֱ����������� $n$ ����㡣</p>
<h2>��ʾ</h2>
<p>�����ṩ��һ��ֻ���������������ܵĳ��� binary_sample.cpp��</p>
<p>���ڸó����˵������ readme.txt��</p>
<p>������ڴ���ʱʹ�øó���Ĵ��룬Ҳ���Բ�ʹ�ã��⽫����ĵ÷��޹ء�</p>
<p><strong>ʱ������</strong>��$1\texttt{s}$</p>
<p><strong>�ռ�����</strong>��$512\texttt{MB}$</p>
<h2>����</h2>
<p><a href="./20765/file/attachment.zip">�������ݼ������ļ�����</a></p>
