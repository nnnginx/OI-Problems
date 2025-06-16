<p>为了简便计算，天文学家们使用儒略日（Julian day）来表达时间。所谓儒略日，其定义为从<strong>公元前 4713 年 1 月 1 日正午 12 点到此后某一时刻间所经过的天数</strong>，不满一天者用小数表达。若利用这一天文学历法，则每一个时刻都将被均匀的映射到数轴上，从而得以很方便的计算它们的差值。</p>
<p>现在，给定一个不含小数部分的儒略日，请你帮忙计算出该儒略日（一定是某一天的中午 12 点）所对应的公历日期。</p>
<p>我们现行的公历为格里高利历（Gregorian calendar），它是在公元 1582 年由教皇格里高利十三世在原有的儒略历（Julian calendar）的基础上修改得到的（注：儒略历与儒略日并无直接关系）。具体而言，现行的公历日期按照以下规则计算：</p>
<ol>
<li>公元 1582 年 10 月 15 日（含）以后：适用格里高利历，每年一月 $31$ 天、 二月 $28$ 天或 $29$ 天、三月 $31$ 天、四月 $30$ 天、五月 $31$ 天、六月 $30$ 天、七月 $31$ 天、八月 $31$ 天、九月 $30$ 天、十月 $31$ 天、十一月 $30$ 天、十二月 $31$ 天。其中，闰年的二月为 $29$ 天，平年为 $28$ 天。当年份是 $400$ 的倍数，或 日期年份是 4 的倍数但不是 100 的倍数时，该年为闰年。</li>
<li>公元 1582 年 10 月 5 日（含）至 10 月 14 日（含）：不存在，这些日期被删除，该年 10 月 4 日之后为 10 月 15 日。</li>
<li>公元 1582 年 10 月 4 日（含）以前：适用儒略历，每月天数与格里高利历 相同，但只要年份是 $4$ 的倍数就是闰年。</li>
<li>尽管儒略历于公元前 45 年才开始实行，且初期经过若干次调整，但今天人类习惯于按照儒略历最终的规则反推一切 1582 年 10 月 4 日之前的时间。注意，<strong>公元零年并不存在</strong>，即公元前 1 年的下一年是公元 1 年。因此公元前 1 年、前 5 年、前 9 年、前 13 年……以此类推的年份应视为闰年。</li>
</ol>
<h2>输入格式</h2>
<p>第一行一个整数 $Q$，表示询问的组数。</p>
<p>接下来 $Q$ 行，每行一个非负整数 $r_i$，表示一个儒略日。</p>
<h2>输出格式</h2>
<p>对于每一个儒略日 $r_i$，输出一行表示日期的字符串 $s_i$。共计 $Q$ 行。 $s_i$ 的格式如下：</p>
<ol>
<li><p>若年份为公元后，输出格式为 <code>Day Month Year</code>。其中日（Day）、月（Month）、年（Year）均不含前导零，中间用一个空格隔开。例如：公元
2020 年 11 月 7 日正午 12 点，输出为 <code>7 11 2020</code>。</p>
</li>
<li><p>若年份为公元前，输出格式为 <code>Day Month Year BC</code>。其中年（Year）输出该年份的数值，其余与公元后相同。例如：公元前 841 年 2 月 1 日正午 12
点，输出为 <code>1 2 841 BC</code>。</p>
</li>
</ol>


<pre><code class="language-input1">3 
10
100
1000
</code></pre>


<pre><code class="language-output1">11 1 4713 BC 
10 4 4713 BC
27 9 4711 BC
</code></pre>



<pre><code class="language-input2">3 
2000000 
3000000
4000000
</code></pre>


<pre><code class="language-output2">14 9 763 
15 8 3501
12 7 6239
</code></pre>

<h2>样例三</h2>
<p>详见附加文件 <code>ex_julian3.in/ans</code>。</p>
<h2>限制与约定</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$Q=$</th>
<th style="text-align:center;">$r_i\le$</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">$365$</td>
</tr>
<tr>
<td style="text-align:center;">$2$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">$10^4$</td>
</tr>
<tr>
<td style="text-align:center;">$3$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">$10^5$</td>
</tr>
<tr>
<td style="text-align:center;">$4$</td>
<td style="text-align:center;">$10000$</td>
<td style="text-align:center;">$3\times 10^5$</td>
</tr>
<tr>
<td style="text-align:center;">$5$</td>
<td style="text-align:center;">$10000$</td>
<td style="text-align:center;">$2.5\times 10^6$</td>
</tr>
<tr>
<td style="text-align:center;">$6$</td>
<td style="text-align:center;">$10^5$</td>
<td style="text-align:center;">$2.5\times 10^6$</td>
</tr>
<tr>
<td style="text-align:center;">$7$</td>
<td style="text-align:center;">$10^5$</td>
<td style="text-align:center;">$5\times 10^6$</td>
</tr>
<tr>
<td style="text-align:center;">$8$</td>
<td style="text-align:center;">$10^5$</td>
<td style="text-align:center;">$10^7$</td>
</tr>
<tr>
<td style="text-align:center;">$9$</td>
<td style="text-align:center;">$10^5$</td>
<td style="text-align:center;">$10^9$</td>
</tr>
<tr>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;">$10^5$</td>
<td style="text-align:center;">年份答案不超过 $10^9$</td>
</tr>
</tbody>
</table>
</div>
<p><strong>时间限制</strong>：$1 \texttt{s}$</p>
<p><strong>空间限制</strong>：$256 \texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20974/file/attachment.zip">样例数据下载</a></p>
