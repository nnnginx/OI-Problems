<p><strong>����һ���ύ����</strong></p>
<p>�����������ӵ�ר�ҡ������������ɸ����Ӻ���ǩ�����ӱ�����ڷ���һ��$R$��$C$�еĸ����ÿ������ǡ����һ�����ӡ�������ɫΪ��ɫ($P$),��ɫ($W$),��ɫ($G$)��</p>
<p>��ÿ�λ�ѡ���������������ӣ����������ӱ���������ֱ����(��������)��ˮƽ����(��������)���߶Խ��߷���(�����������£��������������)�����磬�����ѡ������ֱ������������ӣ���ᰴ����-��-�µ�˳�����ν����Ӵ�����ǩ�ϡ�һ������ֻ�ܱ�����һ����ǩ�ϡ�</p>
<p>һ��������Ư���ĵ��ҽ�����ǩ�ϴ������ӵ���ɫ����Ϊ��-��-�̻�����-��-�ۡ�</p>
<p>����Ҫ�����������Ư�������ӡ�</p>
<h2>�����ʽ</h2>
<p>����һ���ύ���⣬���� $6$ ���������ݣ���Щ��������Ϊ <code>input_01.txt</code> ~ <code>input_06.txt</code>��</p>
<p>��һ������������$R,C$��</p>
<p>������$R$�У�ÿ��$C$���ַ�����ʾ���ӵ���ɫ����$i+1$�еĵ�$j$���ַ������ŵ�$i$�е�$j$�е�������ɫ��</p>
<h2>�����ʽ</h2>
<p>����ÿ���������ݣ�����Ҫ�ύ��Ӧ������ļ� <code>output_01.txt</code> ~ <code>output_06.txt</code>��</p>
<p>$R$�У�ÿ��һ������Ϊ$C$�Ľ�����<samp>'P','W','G','|','-','/','\'</samp>���ַ�������������:</p>
<ul><li>���ַ�Ϊ<samp>'|'</samp>����ʾһ��ʹ���Ϸ��ĸ��ӣ���ǰ���ӣ��·��ĸ��ӵ�һ������</li>
<li>���ַ�Ϊ<samp>'-'</samp>����ʾһ��ʹ���󷽵ĸ��ӣ���ǰ���ӣ��ҷ��ĸ��ӵ�һ������</li>
<li>���ַ�Ϊ<samp>'\'</samp>����ʾһ��ʹ�����Ϸ��ĸ��ӣ���ǰ���ӣ����·��ĸ��ӵ�һ������</li>
<li>���ַ�Ϊ<samp>'/'</samp>����ʾһ��ʹ�����Ϸ��ĸ��ӣ���ǰ���ӣ����·��ĸ��ӵ�һ������</li>
<li>�����ַ�Ϊ�����и����ӵ���ɫ��</li>
</ul>

<pre><code class="language-input1"><code class="sh_plain">3 4
PWGP
WGPW
GWPG</code>
</code></pre>

<pre><code class="language-output1"><code class="sh_plain">P-GP
WGP|
G-PG</code>
</code></pre>

<p>ע�ⲻ�ܰ���'WGP'��˳�����ӡ�</p>


<pre><code class="language-input2"><code class="sh_plain">3 4
PWWP
WWWW
PGGP</code>
</code></pre>

<pre><code class="language-output2"><code class="sh_plain">PWWP
W\/W
PGGP</code>
</code></pre>
<h2>���ֱ�׼</h2>
<p>����ÿ�����Ե㣬���Ǹ����ĸ�����$S,X,Y,Z$����������:</p>
<div class="table-responsive">
    <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>���Ե���</th><th>$S$</th><th>$X$</th><th>$Y$</th><th>$Z$</th></tr></thead><tbody><tr><td>$1$</td><td>$15$</td><td>44000</td><td>47000</td><td>47220</td></tr><tr><td>$2$</td><td>$15$</td><td>39000</td><td>41700</td><td>41980</td></tr><tr><td>$3$</td><td>$15$</td><td>45000</td><td>51000</td><td>51390</td></tr><tr><td>$4$</td><td>$15$</td><td>18000</td><td>19000</td><td>19120</td></tr><tr><td>$5$</td><td>$20$</td><td>43000</td><td>48200</td><td>48620</td></tr><tr><td>$6$</td><td>$20$</td><td>44000</td><td>46000</td><td>46500</td></tr></tbody></table></div>

<p>����ÿ�����Ե�:</p>
<ul><li>�����������Ϸ�����ĵ÷�Ϊ0����������ķ�����Ư�������Ӵ�����Ϊ$N$��</li>
<li>�� $N &lt; X$,��ĵ÷�Ϊ 0��</li>
<li>�� $X \le N &lt; Y$����ĵ÷�Ϊ $\frac{N-X}{2(Y-X)} \times S$��</li>
<li>�� $Y \le N &lt; Z$����ĵ÷�Ϊ $(\frac{1}{2}+\frac{N-Y}{2(Z-Y)}) \times S$��</li>
<li>�� $Z \le N$����ĵ÷�Ϊ $S$��</li>
</ul><h2>���ݷ�Χ</h2>
<p>�����������ݣ�����$3 \le R,C \le 500$��</p>
<p><a href="http://uoj.ac/download.php?type=problem&amp;id=511">������������</a></p>
