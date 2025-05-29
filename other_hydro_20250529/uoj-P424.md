<p>如果一个序列满足序列长度为$n$，序列中的每个数都是$1$到$m$内的整数，且所有$1$到$m$内的整数都在序列中出现过，则称这是一个挺好序列。</p>
<p>对于一个序列$A$，记$f_A(l, r)$为$A$的第$l$个到第$r​$个数中最大值的下标（如果有多个最大值，取下标最小的）。</p>
<p>两个序列$A$和$B$同构，当且仅当$A$和$B$长度相等，且对于任意$i\le j$，均有$f_A(i,j)=f_B(i,j)$。</p>
<p>给出$n,m$，求有多少种不同构的挺好序列。答案对$998244353​$取模。</p>
<h2>输入格式</h2>
<p>一行两个正整数$n,m$。</p>
<h2>输出格式</h2>
<p>一行一个整数，表示有多少种不同构的挺好序列。</p>


<pre><code class="language-input1"><code>3 2</code>
</code></pre>

<pre><code class="language-output1"><code>4</code>
</code></pre>

<p>一共$6$种挺好序列：$2\ 1\ 1$，$1\ 2\ 1$，$1\ 1\ 2$，$1\ 2\ 2$，$2\ 1\ 2$，$2\ 2\ 1$。其中$2\ 1\ 1$和$2\ 2\ 1$同构，$1\ 2\ 1$和$1\ 2\ 2$同构，所以一共有$4$种不同构的挺好序列。</p>


<pre><code class="language-input2"><code>8 5</code>
</code></pre>

<pre><code class="language-output2"><code>1341</code>
</code></pre>


<pre><code class="language-input3"><code>100000 99999</code>
</code></pre>

<pre><code class="language-output3"><code>944488805</code>
</code></pre>


<pre><code class="language-input4"><code>300 200</code>
</code></pre>

<pre><code class="language-output4"><code>430256456</code>
</code></pre>


<pre><code class="language-input5"><code>2000 1000</code>
</code></pre>

<pre><code class="language-output5"><code>267823945</code>
</code></pre>


<pre><code class="language-input6"><code>100000 50000</code>
</code></pre>

<pre><code class="language-output6"><code>779381353</code>
</code></pre>
<h2>限制与约定</h2>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>子任务</th>
    <th>$n,m\leq$</th>
    <th>特殊性质</th>
    <th>分值</th>
    </tr></thead><tbody><tr><td>1</td>
    <td>$8$</td>
    <td></td>
    <td>$10$</td>
  </tr><tr><td>2</td>
    <td>$100000$</td>
    <td>$m\ge n-1$</td>
    <td>$10$</td>
  </tr><tr><td>3</td>
    <td>$300$</td>
    <td></td>
    <td>$30$</td>
  </tr><tr><td>4</td>
    <td>$2000$</td>
    <td></td>
    <td>$20$</td>
  </tr><tr><td>5</td>
    <td>$100000$</td>
    <td></td>
    <td>$30$</td>
  </tr></tbody></table></div>

<p><strong>时间限制</strong>：$\texttt{5s}$</p>
<p><strong>空间限制</strong>：$\texttt{512MB}$</p>
<h2>下载</h2>
<p><a href="./20829/file/attachment.zip">样例数据下载</a></p>
