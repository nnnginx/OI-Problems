<script type="text/x-mathjax-config">
MathJax.Hub.Config({
  tex2jax: {
    inlineMath: [['$','$'], ['\\(','\\)']],
    skipTags: ["script","noscript","style","textarea","code"]
  }
});
</script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

<p align="justify">
Though it might be hard to imagine, the inhabitants of a small country Additivia do not know of such thing as change, which probably has to do with them not knowing subtraction either. When they buy something, they always need to have the exact amount of addollars, their currency. The only other option, but not a really attractive one, is over-paying.

</p><p align="justify">
Professor Adem, one of the Additivian mathematicians came up with an algorithm for keeping a balanced portfolio. The idea is the following. 
Suppose you have more coins of value $v_1$ than coins of value $v_2$. In this case you should try to spend at least as many coins of value $v_1$ as those of value $v_2$ on any buy you make. Of course spending too many $v_1$ coins is not a good idea either, but to make the algorithm simpler professor Adem decided to ignore the problem. The algorithm became an instant hitand professor Adem is now designing a kind of "electronic portfolio" with built-in Adem's algorithm. All he needs now is a software for these machines, that will decide whether a given amount ofaddollars can be paid using a given set of coins according to the rules of Adem's algorithm. Needless to say, you are his chosen programmer for the task.

<font color="#0000FF"></font></p><h2><font color="#0000FF">Problem</font></h2>

<p align="justify">
Write a program that reads the description of a set of coins and an amount of addollars to be paid, and determines whether you can pay that amount according to Professor Adem's rules.

</p><h3>Input</h3>
<p align="justify">
The input starts with the amount of addollars to be paid $x$, where $1 \le x \le 100,000$. The number of different coin values $k$ follows, where $1 \le k \le 5$. The values of the coins $v_1, \ldots, v_k$ follow, where $1 \le v_i \le 10,000$. 

</p><p align="justify">
Notice that the order among coin values is significant: you need to spend at least as many coins of value $v_1$ as coins of value $v_2$, at least as many coins of value $v_2$ as those of value $v_3$, and so on. You may assume 
that you have a sufficiently large number of coins of each value.

</p><h3>Output</h3>
<p align="justify">
Your program should output for each test case either a single word "<tt>YES</tt>", if the given amount can be paid according to the rules, or a single word "<tt>NO</tt>" otherwise.

</p><h3>Example</h3>
<pre><b>Input:</b>
13 3 9 2 1

<b>Output:</b>
NO
</pre>