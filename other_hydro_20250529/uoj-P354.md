<p><strong>这是一道<del>送分</del>提交答案题。</strong></p>
<p>在打败了AlphaGo之后，SingleDog们决定选出一个新的狗群首领，建立起崭新的战后秩序。</p>
<p>但是他们在研究了美国大选Trump的先例之后，发现每个独立的选民能获取的信息都是有限的，他们很好奇，这种情况下，选民还能不能选出正确的选择呢？</p>
<h2>任务一</h2>
<p>我们把选举的过程抽象成以下的模型：</p>
<p>$n = 15$ 个选民围成一圈，每个人额头上有一个数字 $0$ 或者 $1$，自己看不见自己额头上的数字，但是可以看见所有其他人头上的数字。</p>
<p>每个人投一票给 $0$ 或者 $1$，目标是要投出所有人额头上数字的异或和的正确值，最终投票的结果就是票数最多的一个。</p>
<p>请你为每个人选择一个策略，在所有 $2^n = 32768$ 的可能的情况中，使得严格小于 $7000$ 个情况投票结果无法投出正确值。</p>
<h2>任务二</h2>
<p>在研究了任务一之后，狗群决定加大难度。</p>
<p>在任务一的模型中，请你为每个人选择一个策略，使得在所有 $2^n = 32768$ 的可能的情况中，只有严格小于 $2100$ 个情况投票结果无法投出正确值。</p>
<h2>任务三</h2>
<p>SingleDog们对于这个正确率还是很不满意，他们认为，如果每个选民可以投任意 $x$ 票（$0 \leq x \leq 10^8$）来表示他们支持的情感的强烈程度，那么情况就会有所好转。</p>
<p>那么如果把任务一的模型中每人只能投一票，改为每人可以投任意 $0 \leq x \leq 10^8$ 票呢？</p>
<p><strong>请留意这个任务中每人可以投任意 $0 \leq x \leq 10^8$ 票。</strong></p>
<p>你能使只有严格小于 $3$ 个情况投票结果无法投出正确值吗？（平票的情况算做错误）</p>
<h2>任务四</h2>
<p>但是理想模型和狗群现实还是有很大的差距，往往选民获取的信息只有一半甚至更少。</p>
<p>现在 $C(n, k)$ 个人围成一圈，圈里是一个长度为 $n = 12$ 的01串，每个人可以看到自己编号对应的一个大小为 $k = 7$ 的位的集合（假设一个人可以看到的集合是 $S$，那么我们定义 $f(S)=\sum_{x \in S} 2^{x-1}$，第 $i$ 个人就是 $f(S)$ 第 $i$ 小的人）。</p>
<p>他们的目标是要选出对应的01串的每一位异或起来是 $0$ 还是 $1$，现在每个人可以投任意 $x$ 票（$0 \leq x \leq 10^8$）。</p>
<p>你能保证在全部 $2^{12} = 4096$ 种可能中，只有严格少于 $80$ 种无法选出正确的异或和吗？（平票的情况算做错误）</p>
<h2>格式</h2>
<p>对于全部的四个任务，你需要提交你的答案文件，其中包含每个动物的投票策略。</p>
<h4>任务一、任务二</h4>
<p>这个文件的第 $i$ 行是一个长度为 $2^{n - 1}$ 的01串，代表第 $i$ 个动物的投票策略。</p>
<p>将一个动物能看到的每个位置的情况，按照位置编号大到小的顺序从左往右排列，可以看做一个二进制数（即二进制数中 $2^{i-1}$ 对应的位，表示从小到大第 $i$ 个看到的bit是0还是1）。</p>
<p>比如一个人看到的三个位置编号是 ${6,3,1}$，这三个bit按照编号递减顺序分别是 $1$、$0$、$0$ 时对应的数就是 $4$。</p>
<p>而在01串中，这个数字对应的下标位置，代表了这个动物看到这个场景时的决策。</p>
<p>比如 $n = 2$ 的情况，$01$ 表示如果看到的是 $0$ 就投票给 $0$ 反之投票给 $1$。</p>
<h4>任务三、任务四</h4>
<p>文件的第 $i$ 行变为 $2^{n - 1}$ 或者 $2^k$ 个数字，每个数字表示对应情况下头投的票数, 正数表示投给1，负数表示投给0，需要在 $-10^8$ 到 $10^8$ 之间。</p>
<h2>各对应任务的分数</h2>
<div class="table-responsive">
 <table class="table table-bordered table-text-center table-vertical-middle"><thead><tr><th>子任务</th>
    <th>分值</th>
   </tr></thead><tbody><tr><td>1</td>
    <td>22</td>
   </tr><tr><td>2</td>
    <td>24</td>
   </tr><tr><td>3</td>
    <td>18</td>
   </tr><tr><td>4</td>
    <td>36</td>
   </tr></tbody></table></div>


<h2>如何测试你的输出</h2>
<p>在终端中先切换到该试题的目录下：（windows用户请使用cmd）（假设你把输入输出文件、checker什么的都放在了vote这个文件夹下）</p>
<p><code>cd vote</code></p>
<p>我们提供checker这个工具来测试你的输出文件是否是可接受的。使用这个工具的方法是，在终端中运行</p>
<p><code>g++ checker.cpp -o checker</code></p>
<p><code>./checker vote&lt;case_no&gt;.in your_answer.out your_answer.out</code></p>
<p>其中case_no是测试数据的编号。</p>
<p>在你调用这个程序后，checker将根据你给出的输出文件给出测试的结果。</p>
<p><strong>注意比赛时提交此题显示的成绩就是最终成绩。</strong></p>
<h2>下载</h2>
<p><a href="./20780/file/attachment.zip">checker下载</a></p>
