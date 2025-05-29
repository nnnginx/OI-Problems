## Description

<div><p>Megumin is a wizard who can cast powerful magic spells that affect large areas. She is obsessed with the extremely devastating Explosion spell that can destroy everything around its target.</p><p>There are currently $n$ slimes in the wild. Each slime's location can be described in 2D Cartesian coordinates. Megumin wishes to kill at least $k$ slimes so she can earn more experience points to level up her Explosion. To do that, she can choose any circle on the plane and cast an Explosion spell which kills every slime inside or on the border of the circle.</p><p>However, the Explosion magic requires a large amount of mana to cast, and Megumin can only use it once per day. The amount of mana used is equal to the area inside the circle she chooses. What is the minimum amount of mana she needs to spend to kill $k$ slimes with a single Explosion?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 10^5$)&nbsp;！ the number of slimes and how many slimes Megumin needs to defeat. </p><p>Each of the next $n$ lines contains two integers $x$ and $y$ ($-10^9 \le x, y \le 10^9$), denoting the coordinates $(x, y)$ of a slime's location. It is guaranteed that all locations are distinct and that no three slimes lie on the same circle.</p></div><div class="output-specification"><p>Print one real number&nbsp;！ the answer.</p><p>Your answer is considered correct if its absolute or relative error does not exceed $10^{-6}$. Formally, let your answer be $a$, and the jury's answer be $b$. Your answer is accepted if and only if $\frac{|a-b|}{\max(1,|b|)} \le 10^{-6}$.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 10^5$)&nbsp;！ the number of slimes and how many slimes Megumin needs to defeat. </p><p>Each of the next $n$ lines contains two integers $x$ and $y$ ($-10^9 \le x, y \le 10^9$), denoting the coordinates $(x, y)$ of a slime's location. It is guaranteed that all locations are distinct and that no three slimes lie on the same circle.</p>

## Output

<p>Print one real number&nbsp;！ the answer.</p><p>Your answer is considered correct if its absolute or relative error does not exceed $10^{-6}$. Formally, let your answer be $a$, and the jury's answer be $b$. Your answer is accepted if and only if $\frac{|a-b|}{\max(1,|b|)} \le 10^{-6}$.</p>





```input1|
1 1
0 0
```




```input2|
3 2
0 0
100 0
2 0
```




```output1
0.000000000000000
```




```output2
3.141592653589793
```



## Note

<p>In the first example, Megumin can hit the slime with a circle centered at $(0, 0)$ with radius $0$.</p><p>In the second example, Megumin can hit the first and last slimes with a circle centered at $(1, 0)$ with radius $1$.</p>
