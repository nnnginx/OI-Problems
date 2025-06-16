## 题目描述

This problem considers how mighty countries arise from humble beginnings. Consider a two-dimensional map of the area. On this map there are n cities. Each city $i$ is in a distinct location with coordinates $(x_i, y_i)$ on the map. The city has also a number $s_i$ of soldiers in it under the command of a general.

The influence city $i$ exerts to another location $(x,y)$ is computed as $s_i$ divided by the squared distance between it and $(x,y)$ . It is as if the mass of soldiers in city $i$ exerted a gravitational pull to all map locations around it. City $i$ is threatened by another city $j$ if the influence exerted by city $j$ on the location $(x_i, y_i)$ of city $i$ exceeds its number of soldiers $s_i$ : then city $j$ can dispatch enough soldiers to overpower all the soldiers defending city $i$. If city $i$ is not threatened by any other city $j$, then its grateful citizens elect its invincible general as their king, and turn their city into the capital of his kingdom.

On the other hand, if some city $j$ threatening city $i$ exerts strictly more influence on its location $(x_i, y_i)$ than any other city $k$, then the citizens of city $i$ have no choice: city $i$ must surrender to city $j$. Henceforth city $i$ must obey the same capital as city $j$ obeys; however, the $s_i$ soldiers in city $i$ do not join the army of city $j$ or the capital. Otherwise city $i$ is saved by mutual distrust of the equally threatening cities $j$ and $k$: If one of them would attack and overpower city $i$, then the other would in turn attack and overpower the battle-weary first attackers. However, the citizens of city $i$ can no longer elect its general as their king, because he has failed in his duty to keep the city safe from threats. Thus they must turn their city into the capital of a democracy instead.

Your task is to write a program, which takes the information about the cities on the map as inputs, and outputs for each city $i$ one of the three outcomes:

• It is the capital of a kindgom.

• It is the capital of a democracy.

• It obeys city $j$ as its capital.

## 输入格式

The input is read from a text file named `countries.in`. 

The first line consists of one integer $n$, the number of cities.

The following $n$ lines give the information on the $n$ cities, each city as its own line. 

Line $i + 1$ gives the information on city $i$ as the three integers $x_i, y_i, s_i$ which are separated by single space characters. 

## 输出格式

The output is written into a text file named `countries.out`.

The output consists of $n$ lines, where line i consists of the outcome for city $i$:

• The character `K` if city $i$ is the capital of a kingdom.

• The character `D` if city $i$ is the capital of a democracy.

• The number $1 ≤ j ≤ n$ of the city which city $i$ obeys as its capital if city $i$ had to surrender.


```input1
5
2 5 14
2 3 2
3 2 7
1 1 2
2 1 3
```

```output1
K
D
K
3
3
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq n \leq 10^3$，$0 \leq x_i, y_i, s_i \leq 10^3$。

