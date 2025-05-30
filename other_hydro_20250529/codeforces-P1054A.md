## Description

<div><p>Masha lives in a multi-storey building, where floors are numbered with positive integers. Two floors are called adjacent if their numbers differ by one. Masha decided to visit Egor. Masha lives on the floor $x$, Egor on the floor $y$ (not on the same floor with Masha).</p><p>The house has a staircase and an elevator. If Masha uses the stairs, it takes $t_1$ seconds for her to walk between adjacent floors (in each direction). The elevator passes between adjacent floors (in each way) in $t_2$ seconds. The elevator moves with doors closed. The elevator spends $t_3$ seconds to open or close the doors. We can assume that time is not spent on any action except moving between adjacent floors and waiting for the doors to open or close. If Masha uses the elevator, it immediately goes directly to the desired floor.</p><p>Coming out of the apartment on her floor, Masha noticed that the elevator is now on the floor $z$ and has closed doors. Now she has to choose whether to use the stairs or use the elevator. </p><p>If the time that Masha needs to get to the Egor's floor by the stairs is <span class="tex-font-style-bf">strictly</span> less than the time it will take her using the elevator, then she will use the stairs, otherwise she will choose the elevator.</p><p>Help Mary to understand whether to use the elevator or the stairs.</p></div><div class="input-specification"><p>The only line contains six integers $x$, $y$, $z$, $t_1$, $t_2$, $t_3$ ($1 \leq x, y, z, t_1, t_2, t_3 \leq 1000$)&nbsp;— the floor Masha is at, the floor Masha wants to get to, the floor the elevator is located on, the time it takes Masha to pass between two floors by stairs, the time it takes the elevator to pass between two floors and the time it takes for the elevator to close or open the doors.</p><p>It is guaranteed that $x \ne y$.</p></div><div class="output-specification"><p>If the time it will take to use the elevator is <span class="tex-font-style-bf">not greater</span> than the time it will take to use the stairs, print «<span class="tex-font-style-tt">YES</span>» (without quotes), otherwise print «<span class="tex-font-style-tt">NO</span>&gt; (without quotes).</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The only line contains six integers $x$, $y$, $z$, $t_1$, $t_2$, $t_3$ ($1 \leq x, y, z, t_1, t_2, t_3 \leq 1000$)&nbsp;— the floor Masha is at, the floor Masha wants to get to, the floor the elevator is located on, the time it takes Masha to pass between two floors by stairs, the time it takes the elevator to pass between two floors and the time it takes for the elevator to close or open the doors.</p><p>It is guaranteed that $x \ne y$.</p>

## Output

<p>If the time it will take to use the elevator is <span class="tex-font-style-bf">not greater</span> than the time it will take to use the stairs, print «<span class="tex-font-style-tt">YES</span>» (without quotes), otherwise print «<span class="tex-font-style-tt">NO</span>&gt; (without quotes).</p><p>You can print each letter in any case (upper or lower).</p>

## Samples

```input1
5 1 4 4 2 1

```

```output1
YES
```






```input2
1 6 6 2 1 1

```

```output2
NO
```






```input3
4 1 7 4 1 2

```

```output3
YES
```




## Note

<p>In the first example:</p><p>If Masha goes by the stairs, the time she spends is $4 \cdot 4 = 16$, because she has to go $4$ times between adjacent floors and each time she spends $4$ seconds. </p><p>If she chooses the elevator, she will have to wait $2$ seconds while the elevator leaves the $4$-th floor and goes to the $5$-th. After that the doors will be opening for another $1$ second. Then Masha will enter the elevator, and she will have to wait for $1$ second for the doors closing. Next, the elevator will spend $4 \cdot 2 = 8$ seconds going from the $5$-th floor to the $1$-st, because the elevator has to pass $4$ times between adjacent floors and spends $2$ seconds each time. And finally, it will take another $1$ second before the doors are open and Masha can come out. </p><p>Thus, all the way by elevator will take $2 + 1 + 1 + 8 + 1 = 13$ seconds, which is less than $16$ seconds, so Masha has to choose the elevator.</p><p>In the second example, it is more profitable for Masha to use the stairs, because it will take $13$ seconds to use the elevator, that is more than the $10$ seconds it will takes to go by foot.</p><p>In the third example, the time it takes to use the elevator is equal to the time it takes to walk up by the stairs, and is equal to $12$ seconds. That means Masha will take the elevator.</p>
