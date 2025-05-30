<p>对于一个城市来说，排水系统是极其重要的一个部分。</p>
<p>有一天，小 C 拿到了某座城市排水系统的设计图。排水系统由 $n$ 个排水结点（它们从 $1 \sim n$ 编号）和若干个单向排水管道构成。每一个排水结点有若干个管道用于汇集其他排水结点的污水（简称为该结点的汇集管道），也有若干个管道向其他的排水结点排出污水（简称为该结点的排出管道）。</p>
<p>排水系统的结点中有 $m$ 个污水接收口，它们的编号分别为 $1, 2, \cdots , m$，污水只能从这些接收口流入排水系统，并且这些结点没有汇集管道。排水系统中还有若干个最终排水口，它们将污水运送到污水处理厂，没有排出管道的结点便可视为一个最终排水口。</p>
<p>现在各个污水接收口分别都接收了 1 吨污水，污水进入每个结点后，会均等地从当前结点的每一个排出管道流向其他排水结点，而最终排水口将把污水排出系统。</p>
<p>现在小 C 想知道，在该城市的排水系统中，每个最终排水口会排出多少污水。该城市的排水系统设计科学，管道不会形成回路，即不会发生污水形成环流的情况。</p>
<h2>输入格式</h2>
<p>第一个两个用单个空格分隔的整数 $n，m$。分别表示排水结点数与接收口数量。</p>
<p>接下来 $n$ 行，第 $i$ 行用于描述结点 $i$ 的所有排出管道。其中每行第一个整数 $d_i$ 表示其排出管道的数量，接下来 $d_i$ 个用单个空格分隔的整数 $a_1, a_2, \cdots , a_{d_i}$ 依次表示管道的目标排水结点。</p>
<p>保证不会出现两条起始结点与目标结点均相同的管道。</p>
<h2>输出格式</h2>
<p>输出若干行，按照编号从小到大的顺序，给出每个最终排水口排出的污水体积。其中体积使用分数形式进行输出，即每行输出两个用单个空格分隔的整数 $p,q$，表示排出的污水体积为 $\frac p q$。要求 $p$ 与 $q$ 互素，$q = 1$ 时也需要输出 $q$。</p>


<pre><code class="language-input1">5 1
3 2 3 5
2 4 5
2 5 4
0
0
</code></pre>


<pre><code class="language-output1">1 3
2 3
</code></pre>

<h2>样例解释一</h2>
<p>1 号结点是接收口，4、5 号结点没有排出管道，因此是最终排水口。  </p>
<p>1 吨污水流入 1 号结点后，均等地流向 2、3、5 号结点，三个结点各流入 $\frac{1}{3}$ 吨污水。  </p>
<p>2 号结点流入的  $\frac{1}{3}$ 吨污水将均等地流向 4、5 号结点，两结点各流入  $\frac{1}{6}$ 吨污水。  </p>
<p>3 号结点流入的  $\frac{1}{3}$ 吨污水将均等地流向 4、5 号结点，两结点各流入  $\frac{1}{6}$ 吨污水。  </p>
<p>最终，4 号结点排出  $\frac{1}{6} +  \frac{1}{6} =  \frac{1}{3}$  吨污水，5 号结点排出 $\frac{1}{3} + \frac{1}{6} +  \frac{1}{6} =  \frac{2}{3}$  吨污水</p>
<h2>样例二</h2>
<p>见附加文件中的 <code>ex_water2.in/ans</code>。</p>
<h2>样例三</h2>
<p>见附加文件中的 <code>ex_water3.in/ans</code>。</p>
<h2>限制与约定</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle">
<thead>
<tr>
<th style="text-align:center;">测试点编号</th>
<th style="text-align:center;">$n \le$</th>
<th style="text-align:center;">$m \le$</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center;">$1 \sim 3$</td>
<td style="text-align:center;">$10$</td>
<td style="text-align:center;">$1$</td>
</tr>
<tr>
<td style="text-align:center;">$4 \sim 6$</td>
<td style="text-align:center;">$1000$</td>
<td style="text-align:center;">$1$</td>
</tr>
<tr>
<td style="text-align:center;">$7 \sim 8$</td>
<td style="text-align:center;">$10^5$</td>
<td style="text-align:center;">$1$</td>
</tr>
<tr>
<td style="text-align:center;">$9 \sim 10$</td>
<td style="text-align:center;">$10^5$</td>
<td style="text-align:center;">$10$</td>
</tr>
</tbody>
</table>
</div>
<p>对于所有测试点，保证 $1 \le n \le 10^5，1 \le m \le 10，0 \le d_i \le 5$。  </p>
<p>数据保证，污水在从一个接收口流向一个最终排水口的过程中，不会经过超过 $10$ 个中间排水结点（即接收口和最终排水口不算在内）。</p>
<p><strong>时间限制</strong>：$1 \texttt{s}$</p>
<p><strong>空间限制</strong>：$512 \texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20984/file/attachment.zip">附加文件下载</a></p>
