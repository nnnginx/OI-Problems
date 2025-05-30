<p>蒜斜最近发现了一个线上 24 点<a href="https://live.bilibili.com/23058701">对战平台</a>。他最近每天都会在上面和牛逼网友们对战 24 点，但是总是输多赢少。</p>
<p>于是，蒜斜打算来特训一下 24 点水平，你能陪他一起吗？</p>
<p><strong>在本题中，只允许使用加减乘除这四种运算，可以使用括号，计算过程中也可以出现小数</strong></p>
<h4>Small Task</h4>
<p>下发文件 <code>24point1.in</code> 中包含了 $30$ 道 24 点题，你需要提交一个长度为 $30$ 的只包含 <code>YN</code> 的字符串，分别表示每一道题有解（<code>Y</code>）还是无解（<code>N</code>）。</p>
<p>提交文件：<code>24point1.out</code>。</p>
<h4>Large Task</h4>
<p>蒜斜在做题的时候发现，给自己的计算过程设置一个上下界会大幅度加快他的求解速度。具体来说，蒜斜会想好两个数字 $l, r( l \leq r)$，在运算的过程中，如果中间结果不在区间 $[l,r]$ 范围内了，就放弃这个中间结果。</p>
<p>这是一个例子，如果 $l, r$ 分别取 $0$ 和 $24$，那么中间结果 <code>3-4</code>, <code>(3+7)*4</code>, <code>9*3</code> 都会被放弃。</p>
<p>设置上下界的坏处在于，可能会有一些 24 点题的解会被放弃掉。比方说，对于 24 点题 $[3, 5, 7, 8]$，在 $l = 0, r = 24$ 的时候，解 <code>((5*7)-3)-8</code> 会被放弃，因为它中间结果出现了 $32$；解 <code>(3*7)-(5-8)</code> 也会被放弃，因为它中间结果出现了 -3。不过好在，这个问题还是能被解出来的，因为 <code>((3*7)-5)+8</code> 的所有结果都没有超出这个范围。</p>
<p>现在，蒜斜想要决定 $l, r$ 的值，使得对于所有有解的 24 点题，都存在一个所有中间结果（包括初始给定的四个数字）都在 $[l, r]$ 范围内的解。在这题中，我们只考虑数字范围为 $1, 2, \dots, 12, 13$ 的 24 点题。</p>
<p>这样的区间有很多，你需要提交 $r - l$ 的最小值，四舍五入保留十位小数。</p>
<p>提交文件：<code>24point2.out</code>。</p>
<h2>下载</h2>
<p><a href="./21046/file/attachment.zip">下发文件下载</a></p>
