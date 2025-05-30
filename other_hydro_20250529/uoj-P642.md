<p>虽然在算法竞赛中不常用，但是面向对象确实是 c++ 编程中非常重要的一部分。</p>
<p><img src="https://img.uoj.ac/problem/642/oop.jpg" alt="面向对象" class="img-responsive center-block"></p>
<p>在北京大学信科的培养方案中，面向对象编程是每一名本科生的必修课。今天，蒜斜在整理他以前的课程资料的时候，找到了他学习面向对象编程时的大作业代码。然而，因为一些未知的原因，代码里的一些内容丢失了。</p>
<p>于是蒜斜找到了你，希望你能帮他复原一下这个代码。复原的方式有很多，于是他希望你能告诉他不同的复原方式有多少种。</p>
<h2>问题描述</h2>
<p>给出一个损坏的 c++ 代码。因为数据丢失的原因，这个代码里存在一些未知的空缺。空缺有两类：</p>
<ol>
<li>修饰符空缺，用 <code>/*MissingModifier*/</code> 表示。在原本程序中，这一类空缺对应的一定是标识符 <code>private</code>, <code>protected</code> 和 <code>public</code> 中的一个。</li>
<li>函数空缺，用 <code>/*MissingMethod*/</code> 表示。在原本程序中，这一类空缺对应的一定是一个形如 <code>method#Num</code> 的函数名，其中 <code>#Num</code> 对应了一个正整数。</li>
</ol>
<p>给定一个损坏的 c++ 代码，你需要计算有多少种填写空缺的方案，使得填写后的程序是可以正常通过编译的。这个方案数可能会很大，因此你只需要输出方案数对 $998244353$ 取模后的结果。</p>
<h2>例子</h2>
<p>下面给出了一个损坏的 c++ 代码。</p>
<pre><code class="sh_cpp">class Class1 {
  void method1() {
    /*MissingMethod*/();
  }
  /*MissingModifier*/:
  void method2() {}
};
class Class2: /*MissingModifier*/ Class1 {
  /*MissingModifier*/:
  void method3() {}
  /*MissingModifier*/:
  void method4() {}
};
int main() {
  Class2 o2;
  o2./*MissingMethod*/();
}</code></pre>
<p>我们按照从上到下的顺序依次把 <code>/*MissingModifier*/</code> 命名为 $x_1, x_2,x_3,x_4$，把 <code>/*MissingMethod*/</code> 命名为 $y_1,y_2$。不难发现 $y_1$ 的填法和其他空缺的填法无关，它始终可以取 <code>method1</code> 或者 <code>method2</code>。因此我们可以先忽略这个空缺，然后在最后把答案乘以 $2$。</p>
<p>对 $y_2$ 的取值分类讨论：</p>
<ol>
<li><code>method1</code>。这时一定无法编译通过，因为 <code>method1</code> 是 <code>Class1</code> 的私有函数。</li>
<li><code>method2</code>。因为是通过 <code>O2</code> 调用的 <code>method2</code>，所以可以得到 $x_1,x_2$ 一定都是 <code>public</code>。此时对 $x_3,x_4$ 的填法没有要求，因此方案数为 $9$。</li>
<li><code>method3</code>。可以得到 $x_3$ 一定是 <code>public</code>。此时对 $x_1,x_2,x_4$ 的填法没有要求，因此方案数为 $27$。</li>
<li><code>method4</code>。与 <code>method3</code> 同理，可以得到方案数为 $27$。</li>
</ol>
<p>因此，总的方案数为 $(9+27+27) \times 2 = 126$。</p>
<h2>限制与约定</h2>
<p>本题的两个部分各给出了一个部分程序（见下发文件下载），分别为 <code>oo1.in</code> 和 <code>oo2.in</code>。对于每一个部分，你只需要提交一个数字，表示对应部分程序的答案。</p>
<p>为了节约大家的时间，这儿给出输入程序的一部分性质：</p>
<ol>
<li>保证存在一种填写空缺的方法可以使得输入程序能够通过编译。</li>
<li>输入程序中除了主函数 <code>main</code> 以外，所有的函数均为成员函数。</li>
<li>输入程序中没有使用虚函数和静态函数。</li>
<li>输入程序中所有的修饰符 <code>public</code>, <code>protected</code> 和 <code>private</code> 均被替换为了空缺 <code>/*MissingModifier*/</code>。</li>
<li>输入程序中所有的函数调用均被替换为了空缺 <code>/*MissingMethod*/</code>，所有函数声明中的函数名均没有被替换。</li>
<li>输入程序中所有类按照出现顺序依次命名为 <code>Class1</code>, <code>Class2</code> 等等。所有成员函数按照出现顺序依次命名为 <code>method1</code>, <code>method2</code> 等等。</li>
<li>除了 <code>Class1</code> 以外，其他所有类均有一个父类。</li>
<li>所有类均不包含任何成员变量。</li>
<li>输入程序中类的数量不超过 $300$ 个，成员函数总数以及函数调用总数不超过 $1000$ 个。</li>
</ol>
<p>在 small task 中，输入程序 <code>oo1.in</code> 还保证：</p>
<ol>
<li>主函数 <code>main</code> 为空。</li>
<li>在每一个成员函数的声明之前，均有一个修饰符空缺 <code>/*MissingModifier*/:</code>。</li>
</ol>
<h2>下载</h2>
<p><a href="./21043/file/attachment.zip">输入程序下载</a></p>
