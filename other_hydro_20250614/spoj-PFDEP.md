<script type="text/x-mathjax-config">
MathJax.Hub.Config({
  tex2jax: {
    inlineMath: [['$','$'], ['\\(','\\)']],
    skipTags: ["script","noscript","style","textarea","code"]
  }
});
</script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

<p>project managers, such as the UNIX utility <tt>make</tt>, are used to maintain large software projects made up from many components. Users write a <i>project file</i> specifying which components (called <i>tasks</i>) depend on others and the project manager can automatically update the components in the correct order.</p>

<font color="#0000FF"><h2>problem</h2></font>

<p>Write a program that reads a project file and outputs the order in which the tasks should be performed.</p>

<h3>Input</h3>
<p>
For simplicity we represent each task by an integer number from $1, 2, \ldots, N$ (where $N$ is the total number of tasks). The first line of input specifies the number $N$ of tasks and the number $M$ of rules, such that $N \le 100$, $M \le 100$.
</p>

<p>
The rest of the input consists of $M$ <i>rules</i>, one in each line, specifying dependencies using the following syntax: 
</p>

<pre>$T_0$ $k$ $T_1$ $T_2$ $\ldots$ $T_k$
</pre>

<p>
This rule means that task number $T_0$ depends on $k$ tasks $T_1, T_2, \ldots, T_k$ (we say that task $T_0$ is the <i>target</i> and $T_1, \ldots, T_k$ are <i>dependents</i>).
</p>

<p>
Note that tasks numbers are separated by single spaces and that rules end with a newline. Rules can appear in any order, but each task can appear as target only once.
</p>

<p>
Your program can assume that there are no circular dependencies in the rules, i.e. no task depends directly or indirectly on itself.
</p>

<h3>Output</h3>
<p>
The output should be a single line with the permutation of the tasks $1 \ldots N$ to be performed, ordered by dependencies (i.e. no task should appear before others that it depends on).
</p>

<p>
To avoid ambiguity in the output, tasks that do not depend on each other should be ordered by their number (lower numbers first).
</p>

<h3>Example</h3>

<pre><b>Input:</b>
5 4
3 2 1 5
2 2 5 3
4 1 3
5 1 1

<b>Output:</b>
1 5 3 2 4
</pre>