## Description

<div><p><span class="tex-font-style-bf">This is the medium version of the problem. The difference in this version is that $t=1$ and we work on trees.</span></p><p>Ron and Hermione are playing a game on a tree of $n$ nodes that are initially inactive. The game consists of $t$ rounds, each of which starts with a stone on exactly one node, which is considered as activated. A move consists of picking an inactive neighbor of the node with a stone on it and moving the stone there (thus activating this neighbor). Ron makes the first move, after which he alternates with Hermione until no valid move is available. The player that cannot make a move loses the round. If both players play optimally, who wins each round of this game? </p><p>Note that all the rounds are played with the same tree; only the starting node changes. Moreover, after each round, all active nodes are considered inactive again.</p></div><div class="input-specification"><p>The first line contains integers $n$ ($2 \leq n \leq 2\times 10^5$), $t$ ($t=1$), the number of nodes in the tree and the number of rounds, respectively.</p><p>The next $n-1$ lines contain two integers $1 \leq u, v \leq n$ each, corresponding to an edge of the tree.</p><p>The next line contains $t$ integers $1 \leq u_1 , \dots, u_t \leq n$, corresponding to the node where the stone is initially put.</p></div><div class="output-specification"><p>The output consists of $t=1$ line which is either "Ron" or "Hermione".</p></div>

## Input

<p>The first line contains integers $n$ ($2 \leq n \leq 2\times 10^5$), $t$ ($t=1$), the number of nodes in the tree and the number of rounds, respectively.</p><p>The next $n-1$ lines contain two integers $1 \leq u, v \leq n$ each, corresponding to an edge of the tree.</p><p>The next line contains $t$ integers $1 \leq u_1 , \dots, u_t \leq n$, corresponding to the node where the stone is initially put.</p>

## Output

<p>The output consists of $t=1$ line which is either "Ron" or "Hermione".</p>





```input1|
5 1
1 2
1 3
3 4
3 5
1
```




```output1
Ron
```


