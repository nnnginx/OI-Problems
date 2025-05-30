<p>动物园里饲养了很多动物，饲养员小 A 会根据饲养动物的情况，按照《饲养指南》购买不同种类的饲料，并将购买清单发给采购员小 B。 </p>
<p>具体而言，动物世界里存在 $2^k$ 种不同的动物，它们被编号为 $0 \ldots 2^k − 1$。动物园里饲养了其中的 $n$ 种，其中第 $i$ 种动物的编号为 $a_i$。</p>
<p>《饲养指南》中共有 $m$ 条要求，第 $j$ 条要求形如“如果动物园中饲养着某种动物，满足其编号的二进制表示的第 $p_j$ 位为 $1$，则必须购买第 $q_j$ 种饲料”。其中饲料共有 $c$ 种，它们从 $1 \ldots c$ 编号。本题中我们将动物编号的二进制表示视为一个 $k$ 位 01 串，第 $0$ 位是最低位，第 $k − 1$ 位是最高位。 </p>
<p>根据《饲养指南》，小 A 将会制定饲料清单交给小 B，由小 B 购买饲料。清单形如一个 $c$ 位 01 串，第 $i$ 位为 $1$ 时，表示需要购买第 $i$ 种饲料；第 $i$ 位为 $0$ 时，表示不需要购买第 $i$ 种饲料。 实际上根据购买到的饲料，动物园可能可以饲养更多的动物。更具体地，如果将当前未被饲养的编号为 $x$ 的动物加入动物园饲养后，饲料清单没有变化，那么我们认为动物园当前还能饲养编号为 $x$ 的动物。</p>
<p>现在小 B 想请你帮忙算算，动物园目前还能饲养多少种动物。</p>
<h2>输入格式</h2>
<p>第一行包含四个以空格分隔的整数 $n,~m,~c,~k$。</p>
<p>分别表示动物园中动物数量、《饲养指南》要求数、饲料种数与动物编号的二进制表示位数。 </p>
<p>第二行 $n$ 个以空格分隔的整数，其中第 $i$ 个整数表示 $a_i$。</p>
<p>接下来 $m$ 行，每行两个整数 $p_i,~q_i$ 表示一条要求。</p>
<p>数据保证所有 $a_i$ 互不相同，所有的 $q_i$ 互不相同。</p>
<h2>输出格式</h2>
<p>输出仅一行，一个整数表示答案。</p>


<pre><code class="language-input1">3 3 5 4 
1 4 6
0 3 
2 4
2 5
</code></pre>


<pre><code class="language-output1">13
</code></pre>


<p>动物园里饲养了编号为 $1,~4,~6$ 的三种动物，《饲养指南》上的三条要求为：</p>
<ol>
<li><p>若饲养的某种动物的编号的第 $0$ 个二进制位为 $1$，则需购买第 $3$ 种饲料。 </p>
</li>
<li><p>若饲养的某种动物的编号的第 $2$ 个二进制位为 $1$，则需购买第 $4$ 种饲料。 </p>
</li>
<li><p>若饲养的某种动物的编号的第 $2$ 个二进制位为 $1$，则需购买第 $5$ 种饲料。 </p>
</li>
</ol>
<p>饲料购买情况为：</p>
<ol>
<li><p>编号为 $1$ 的动物的第 $0$ 个二进制位为 $1$，因此需要购买第 $3$ 种饲料； </p>
</li>
<li><p>编号为 $4,~6$ 的动物的第 $2$ 个二进制位为 $1$，因此需要购买第 $4,~5$ 种饲料。 </p>
</li>
</ol>
<p>由于在当前动物园中加入一种编号为 $0,2,3,5,7,8,\ldots,15$ 之一的动物，购物清单都不会改变，因此答案为 $13$。</p>


<pre><code class="language-input2">2 2 4 3
1 2 
1 3
2 4
</code></pre>


<pre><code class="language-output2">2
</code></pre>

<h2>样例三</h2>
<p>详见附加文件 <code>ex_zoo3.in/ans</code>。</p>
<h2>限制与约定</h2>
<p>对于 $20\%$ 的数据：$k \le n \le 5，m \le 10，c \le 10$，所有的 $p_i$ 互不相同。 </p>
<p>对于 $40\%$ 的数据：$n \le 15，k \le 20，m \le 20，c \le 20$。</p>
<p>对于 $60\%$ 的数据：$n \le 30，k \le 30，m \le 1000$。</p>
<p>对于 $100\%$ 的数据：$0 \le n,~m \le 10^6，0 \le k \le 64，1 \le c \le 10^8$。</p>
<p><strong>时间限制</strong>：$1 \texttt{s}$</p>
<p><strong>空间限制</strong>：$256 \texttt{MB}$</p>
<h2>下载</h2>
<p><a href="./20975/file/attachment.zip">样例数据下载</a></p>
