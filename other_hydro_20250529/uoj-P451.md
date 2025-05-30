<pre><code>“高峰期走出去地铁巴士挤满了蚂蚁，
 计程车打开车门一只蝴蝶飞进去，
 猫头鹰指挥着红灯该何时才变绿”
               ——华晨宇《世界是个动物园》</code></pre>
<p>每隔一段时间，世界上就会出现一种新的物种，现在，世界上总共有$n$种物种，为了方便描述，根据它们在世界上的出现顺序从早到晚将它们按照$1..n$的顺序编号。</p>
<p>自然界是十分友善的，在任意两种物种$x,y(1\le x&lt; y\le n)$之间，都有一个“保护关系”，这种关系是单向的，要么是$x$想保护$y$，要么是$y$想保护$x$，注意，不会存在$x,y$使得$x$和$y$都想保护对方。</p>
<p>但是，自然界同时也是十分残忍的，或天灾，或人祸，或种间竞争，动物们总是避免不了种种的灾难。</p>
<p>为了更好的抵抗到来的灾难，有些动物决定结盟。</p>
<p>结盟的规则是这样的，对于三种动物$x,y,z(x\neq y,x\neq z,y\neq z)$，如果$x$想保护$y$，$y$想保护$z$，$z$想保护$x$，那么他们就会在同一个联盟里面。</p>
<p>比如说<code>(1,2,3)</code>,<code>(2,3,4)</code>都是满足上面的条件的，那么最后<code>1,2,3,4</code>都会在同一个联盟里面。</p>
<p>然而，时至今日，由于物种的数量变得十分多，物种间的“保护关系”已经变得十分复杂了。</p>
<p>我们这样定义物种间的“保护关系”：</p>
<p>对于物种$i$，我们给出$i$与$1..i-1$的“保护关系”，具体的，给出$s_i$个区间$[l_{i,j},r_{i,j}] (1\le l_{i,j}\le r_{i,j}&lt; i)$，<strong>这些区间两两之间交集为空</strong>，对于$x\in[1,i-1]$，如果存在$j(1\le j\le s_i)$满足$x\in[l_{i,j},r_{i,j}]$，那么$i$与$x$之间的关系就是$i$想保护$x$，否则就是$x$想保护$i$。</p>
<p>而对于物种$i$与物种$x(i+1\le x\le n)$之间的“保护关系”，会在$x$与$1..x-1$的“保护关系”中被定义。</p>
<p>这样显然不重不漏地定义了两两物种之间的“保护关系”。</p>
<p>动物中的生物学家们决定探究物种在演变过程中的变化，一个很重要的课题就是每个时期联盟的数量。</p>
<p>作为动物中的佼佼者，生物学家们希望你能帮助他们求出，对于$i\in[1,n]$，在物种$i$在这个世界上出现之后动物中的联盟的数量。</p>
<h2>输入格式</h2>
<p>第一行两个整数$n$和$ty$，表示物种的数量以及是否强制在线（$ty$为$1$表示强制在线，$ty$为$0$表示不强制在线）。</p>
<p>接下来$n$行，其中第$i$行第一个整数$s_i$，表示区间的数量，接下来同一行$s_i$对整数$L_{i,j},R_{i,j}$，如果$ty=0$，那么$l_{i,j}=L_{i,j},r_{i,j}=R_{i,j}$，否则$l_{i,j}=(L_{i,j}+lastans-1)\mod i+1,r_{i,j}=(R_{i,j}+lastans-1)\mod i+1$，其中$lastans$为物种$i-1$来到这个世界后联盟的数量，特殊地，当$i=1$时，$lastans=0$.</p>
<p>$l_{i,j},r_{i,j}$的意义请参考题目。</p>
<h2>输出格式</h2>
<p>输出一行$n$个整数，其中第$i$个整数，表示物种$i$来到这个世界后联盟的数量。</p>


<pre><code class="language-input1"><code>10 0
0 
1 1 1 
1 1 1 
1 1 1 
2 4 4 1 1 
2 1 1 4 4 
2 1 1 3 6 
2 6 6 1 4 
2 4 4 1 1 
2 2 2 7 8</code>
</code></pre>

<pre><code class="language-output1"><code>1 2 3 4 5 6 7 4 5 1</code>
</code></pre>


<pre><code class="language-input2"><code>10 1
0 
1 0 0 
1 2 2 
1 2 2 
2 0 0 2 2 
2 2 2 5 5 
2 2 2 4 0 
2 7 7 2 5 
2 0 0 6 6 
2 7 7 2 3</code>
</code></pre>

<pre><code class="language-output2"><code>1 2 3 4 5 6 7 4 5 1</code>
</code></pre>
<h2>样例三</h2>
<p>见样例数据下载。</p>
<h4>限制与约定</h4>
<p>记$S$为$s_i$的和。 本题采用捆绑测试，每个子任务的时空限制以及数据范围不尽相同，请选手们认真查看。</p>
<div class="table-responsive">
<table class="table table-bordered table-text-center table-verticle-middle"><thead><tr><th>子任务编号</th><th>$n\le$</th><th>$S\le$</th><th>$ty \le $</th><th>时间限制</th><th>空间限制</th><th>分值</th></tr></thead><tbody><tr><td>1</td><td>500</td><td>$2\times 10^6​$</td><td>0</td><td>1s</td><td>512MB</td><td>9</td></tr><tr><td>2</td><td>2000</td><td>$2\times 10^6​$</td><td>0</td><td>1s</td><td>512MB</td><td>11</td></tr><tr><td>3</td><td>$10^5$</td><td>$3.5\times 10^5​$</td><td>0</td><td>1s</td><td>512MB</td><td>15</td></tr><tr><td>4</td><td>$10^5$</td><td>$3.5\times 10^5​$</td><td>1</td><td>1s</td><td>512MB</td><td>19</td></tr><tr><td>5</td><td>$2\times 10^5​$</td><td>$2\times 10^6​$</td><td>0</td><td>2s</td><td>512MB</td><td>11</td></tr><tr><td>6</td><td>$2\times 10^5​$</td><td>$2\times 10^6​$</td><td>1</td><td>2s</td><td>512MB</td><td>18</td></tr><tr><td>7</td><td>$2\times 10^5​$</td><td>$2\times 10^6​$</td><td>1</td><td>2s</td><td>16MB</td><td>17</td></tr></tbody></table></div>

<h2>提示</h2>
<p>输入输出的数据量较大，建议使用读入输出优化。</p>
<p>样例2即为样例1的加密版本.</p>
<h2>下载</h2>
<p><a href="./20856/file/attachment.zip">样例数据下载</a></p>
