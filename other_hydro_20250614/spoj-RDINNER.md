<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Brian the Computer Science Nerd is going on a date with his girlfriend, Anatevka! His romantic location of choice is a Chinese restaurant.</p>
<p>At this restaurant, $N$ ($1 \leq N \leq 15$) different dishes are available, and Brian would like to order each one exactly once. The waiter will come to his table to take orders $N$ times - the $i$th time he comes will be $W_i$ ($1 \leq W_1 &lt; W_2 &lt; \dots &lt; W_N \leq 10^9$) minutes after the start of the meal. He has quite a poor memory, so each time he comes by, Brian will have a chance to order exactly one new dish.</p>
<p>Dish $i$ takes $T_i$ ($1 \leq T_i \leq 10^9$) minutes to prepare, which means that it will generally come exactly that many minutes after being ordered, delivered by a different waiter who will not take orders. However, meals are guaranteed to arrive in the same order in which they were ordered - this means that, if meal $i$ was ordered before meal $j$, but meal $j$ is ready before meal $i$, then meal $j$ will instead arrive at the same time as meal $i$.</p>
<p>Now, Brian considers time spent waiting for the first meal after the start of the dinner, as well as for each subsequent meal after the previous one, to be idle time. Of course, these are the worst parts of the date, as they require actually engaging in conversation rather than consuming sustenance. In order to impress Anatevka with his optimal ordering skills, he'd like to minimize the length of the largest continuous stretch of idle time throughout the dinner.</p>
<h3>Input</h3>
<p>Line 1: 1 integer, $N$</p>
<p>Line 2: $N$ integers, $W_{1..N}$</p>
<p>Line 3: $N$ integers, $T_{1..N}$</p>
<h3>Output</h3>
<p>1 integer, the minimal length possible for the longest stretch of idle time throughout the meal, in minutes</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">3<br>1 5 6<br>4 2 3</span>

<strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">4</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>Brian's optimal strategy is to order dish 3, then 2, then 1. These dishes will then arrive 4, 7, and 10 minutes into the dinner, respectively. The longest stretch of idle time is then 4 minutes long.</p>
<p>As a further example, if Brian were to order dish 3, then 1, then 2, the last 2 dishes would both arrive 9 minutes into the dinner, with dish 2 being held up by dish 1.</p>