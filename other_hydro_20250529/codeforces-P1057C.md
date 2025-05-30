## Description

<div><p>There are $n$ candy boxes in front of Tania. The boxes are arranged in a row from left to right, numbered from $1$ to $n$. The $i$-th box contains $r_i$ candies, candies have the color $c_i$ (the color can take one of three values ​​— red, green, or blue). All candies inside a single box have the same color (and it is equal to $c_i$).</p><p>Initially, Tanya is next to the box number $s$. Tanya can move to the neighbor box (that is, with a number that differs by one) or eat candies in the current box. Tanya eats candies instantly, but the movement takes one second.</p><p>If Tanya eats candies from the box, then the box itself remains in place, but there is no more candies in it. In other words, Tanya always eats all the candies from the box and candies in the boxes are not refilled.</p><p>It is known that Tanya cannot eat candies of the same color one after another (that is, the colors of candies in two consecutive boxes from which she eats candies are always different). In addition, Tanya's appetite is constantly growing, so in each next box from which she eats candies, there should be strictly more candies than in the previous one.</p><p>Note that for the first box from which Tanya will eat candies, there are no restrictions on the color and number of candies.</p><p>Tanya wants to eat at least $k$ candies. What is the minimum number of seconds she will need? Remember that she eats candies instantly, and time is spent only on movements.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $s$ and $k$ ($1 \le n \le 50$, $1 \le s \le n$, $1 \le k \le 2000$) — number of the boxes, initial position of Tanya and lower bound on number of candies to eat. The following line contains $n$ integers $r_i$ ($1 \le r_i \le 50$) — numbers of candies in the boxes. The third line contains sequence of $n$ letters 'R', 'G' and 'B', meaning the colors of candies in the correspondent boxes ('R' for red, 'G' for green, 'B' for blue). Recall that each box contains candies of only one color. The third line contains no spaces.</p></div><div class="output-specification"><p>Print minimal number of seconds to eat at least $k$ candies. If solution doesn't exist, print "-1".</p></div>

## Input

<p>The first line contains three integers $n$, $s$ and $k$ ($1 \le n \le 50$, $1 \le s \le n$, $1 \le k \le 2000$) — number of the boxes, initial position of Tanya and lower bound on number of candies to eat. The following line contains $n$ integers $r_i$ ($1 \le r_i \le 50$) — numbers of candies in the boxes. The third line contains sequence of $n$ letters 'R', 'G' and 'B', meaning the colors of candies in the correspondent boxes ('R' for red, 'G' for green, 'B' for blue). Recall that each box contains candies of only one color. The third line contains no spaces.</p>

## Output

<p>Print minimal number of seconds to eat at least $k$ candies. If solution doesn't exist, print "-1".</p>

## Samples

```input1
5 3 10
1 2 3 4 5
RGBRR

```

```output1
4

```






```input2
2 1 15
5 6
RG

```

```output2
-1

```




## Note

<p>The sequence of actions of Tanya for the first example:</p><ul> <li> move from the box $3$ to the box $2$; </li><li> eat candies from the box $2$; </li><li> move from the box $2$ to the box $3$; </li><li> eat candy from the box $3$; </li><li> move from the box $3$ to the box $4$; </li><li> move from the box $4$ to the box $5$; </li><li> eat candies from the box $5$. </li></ul><p>Since Tanya eats candy instantly, the required time is four seconds.</p>
