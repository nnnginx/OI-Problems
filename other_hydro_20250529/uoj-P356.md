<p>小M有两个本质不同的栈。</p>
<p>无聊的小M找来了$n$个玩具。之后小M把这$n$个玩具随机顺序加入某一个栈或把他们弹出。</p>
<p>现在小M告诉你每个玩具的入栈和出栈时间，现在她想考考小S，有多少种方案，把每个玩具分配给两个栈之一，并且存在一种满足小M告诉你的入栈和出栈时间的入栈序列。</p>
<p>可怜的小S当然不知道啦，所以他求助于你。</p>
<h2>输入格式</h2>
<p>第一行一个整数$n$。</p>
<p>接下来$n$行，每行两个整数$l_i,r_i$，表示第$i$个玩具的入栈和出栈时间。</p>
<h2>输出格式</h2>
<p>一行一个整数，表示答案<strong>对$10^9+7$取模的值</strong>。</p>


<pre><code class="language-input1">4
1 3
2 5
4 8
6 7
</code></pre>


<pre><code class="language-output1">4
</code></pre>



<pre><code class="language-input2">3
1 4
2 5
3 6
</code></pre>


<pre><code class="language-output2">0
</code></pre>




<pre><code class="language-input3">5
1 4
2 10
6 9
7 8
3 5
</code></pre>


<pre><code class="language-output3">8
</code></pre>





<pre><code class="language-input4">8
1 15
2 5
3 8
4 6
14 16
7 9
10 13
11 12
</code></pre>


<pre><code class="language-output4">16
</code></pre>


<h2>限制与约定</h2>
<p>对于所有数据，</p>
<p>$1\le n\le 10^6,1\le l_i &lt; r_i \le 2n$，$l_i,r_i$互不相同。</p>
<div class="table-responsive">
 <table class="table table-bordered table-text-center table-vertical-middle">
  <thead>
   <tr>
       <th>子任务</th>
    <th>分值</th>
    <th>$n$</th>
   </tr>
  </thead>
  <tbody>
   <tr>
    <td>1</td>
    <td>10</td>
    <td>$\le 20$</td>
   </tr>
   <tr>
    <td>2</td>
    <td>12</td>
    <td>$\le 2000$</td>
   </tr>
   <tr>
    <td>3</td>
    <td>56</td>
    <td>$\le 10^5$</td>
   </tr>
   <tr>
    <td>4</td>
    <td>22</td>
    <td>$\le 10^6$</td>
   </tr>  
  </tbody>
 </table> 
</div>

<p><strong>时间限制：</strong>$6\texttt{s}$</p>
<p><strong>空间限制：</strong>$1024\texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20782/file/attachment.zip">样例数据下载</a></p>
