<p>Byteasar, king of Byteotia, has finally decided to retire.    He has two sons, however, and is unable to decide which one    one of them should succeed him. Therefore he plans to split    the kingdom into two halves, making each son a ruler.</p>
<p>After the division, watchtowers have to be built along    the roads connecting the halves. Obviously, building them    will be costly, so ideally there should be as little roads    between the halves as possible.</p>
<p>Luckily, Byteotia consists of an even number of towns, connected    by roads. Resulting from the division, each half-kingdom should    contain half the towns. Each road connects (directly) two towns.    The roads do not meet nor cross outside towns, though they can    lead through flyovers or tunnels. Every two towns are directly    connected by at most one road.</p>
<p>Which exact towns should lie in which half of the kingdom is a    matter of great importance. You may assume that the land outside    the towns can be partitioned in such a way that the roads connecting    towns lying in the same half will not cross the border.    On the other hand, one watchtower has to be built by each road    connecting towns from different halves.</p>
<h2>Task</h2>
<p>Write a programme that:</p>
<ul>
<li> reads the descriptions of towns and the roads connecting them from 	 the standard input, </li>
<li> determines such a partition of kingdom into halves that both the halves 	 contain an equal number of towns and the number of roads connecting 	 towns lying in different halves is minimum, </li>
<li> writes out the result to the standard output. </li>
</ul>
<p>If more than one optimum partition exists, your programme should pick      one of them arbitrarily.</p>
<h2>Input</h2>
<p>The first line of the standard input contains two integers      <span><img src="./22186/file/IbmINZ3p.png" alt=""></span> and <span><img src="./22186/file/u6TThH66.png" alt=""></span>, separated by a single space, denoting the number of      towns and number of roads respectively,      <span><img src="./22186/file/T5EJS6MT.png" alt=""></span>, <span><img src="./22186/file/M2O7MufP.png" alt=""></span>, <span><img src="./22186/file/qa66giLg.png" alt=""></span>.      The towns are numbered from <span><img src="./22186/file/M1iH6adw.png" alt=""></span> to <span><img src="./22186/file/JViBUDMQ.png" alt=""></span>.      Each of the following <span><img src="./22186/file/LMJhr2iv.png" alt=""></span> lines contains two integers separated by      a single space.      The line no. <span><img src="./22186/file/VEt2Fl9T.png" alt=""></span> (for <span><img src="./22186/file/7btp6VbT.png" alt=""></span>) contains the numbers      <span><img src="./22186/file/8bdp9gK1.png" alt=""></span> and <span><img src="./22186/file/JMQqBjU4.png" alt=""></span>, <span><img src="./22186/file/6LMiMB2D.png" alt=""></span>.      These denote a road connecting <span><img src="./22186/file/H4qNeJOu.png" alt=""></span> and <span><img src="./22186/file/crZ0u3UG.png" alt=""></span>.</p>
<h2>Output</h2>
<p>Your programme should write out exactly one line to the standard output.      It should contain <span><img src="./22186/file/Ow9kOPGq.png" alt=""></span> integers separated by single spaces.      These should be the numbers of towns belonging to the same half of the      kingdom the town no. <span><img src="./22186/file/JcxMkmj1.png" alt=""></span> does, in an increasing order.</p>
<h2>Example</h2>
<p>For the input data:</p>
<pre>6 8
1 2
1 6
2 3
2 5
2 6
3 4
4 5
5 6
</pre>
<p>the correct result is:</p>
<pre>1 2 6
</pre>
<p><img src="./22186/file/Xd2Pwtmn.png" alt=""></p>
<p>The dashed line in the figure shows the optimum partition,    which requires building as little as <span><img src="./22186/file/gmczpfNf.png" alt=""></span> watchtowers.</p>