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
A set of laboratory mice is being trained to escape a maze. The maze is made up of cells, and each cell is connected to some other cells. However, there are obstacles in the passage between cells and therefore there is a time penalty to overcome the passage Also, some passages allow mice to go one-way, but not the other way round.

</p><p align="justify">
Suppose that all mice are now trained and,  when placed  in  an  arbitrary cell in the maze, take a path that leads them to  the  exit cell in minimum time.

</p><p align="justify">
We are going to conduct the following experiment: a mouse is placed in each cell  of the maze and a count-down timer is started. When the timer stops we count the number of mice out of the maze.

<font color="#0000FF"></font></p><h2><font color="#0000FF">Problem</font></h2>

<p align="justify">
Write a program that, given a description of the maze and the time limit, predicts the number of mice that will exit the maze. Assume that there are no bottlenecks is the maze, i.e. that all cells have room for an arbitrary number of mice.

</p><h3>Input</h3>

<p align="justify">
The maze cells are numbered $1, 2, \ldots, N$, where $N$ is the total number of cells. You can assume that $N \le 100$.

</p><p align="justify">
The first three input lines contain  $N$, the number of cells in the maze, $E$, the number of the exit cell, and the starting value $T$  for the count-down timer (in some arbitrary time unit).

</p><p align="justify">
The fourth line contains the number $M$ of connections in the maze, and is followed by $M$ lines, each specifying a connection with three integer numbers: two cell numbers $a$ and $b$ (in the range $1, \ldots, N$) and the number of time units it takes to travel from $a$ to $b$.

</p><p align="justify">
Notice that each connection is one-way, i.e., the mice can't travel from $b$ to $a$ unless there is another line specifying that passage.
Notice also that the time required to travel in each direction might be different.

</p><h3>Output</h3>

<p align="justify">
The output consists of a single line with 
the number of mice that reached the exit cell $E$ in at most $T$ time units.

</p><h3>Example</h3>
<pre><b>Input:</b>
4 
2 
1
8
1 2 1
1 3 1
2 1 1
2 4 1
3 1 1
3 4 1
4 2 1
4 3 1

<b>Output:</b>
3
</pre>