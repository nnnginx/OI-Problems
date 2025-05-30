## 题目描述
Farmer John's cows love their video games! FJ noticed that after playing these games that his cows produced much more milk than usual, surely because contented cows make more milk.

The cows disagree, though, on which is the best game console. One cow wanted to buy the Xbox 360 to play Halo 3; another wanted to buy the Nintendo Wii to play Super Smash Brothers Brawl; a third wanted to play Metal Gear Solid 4 on the PlayStation 3. FJ wants to purchase the set of game consoles (no more than one each) and games (no more than one each -- and within the constraints of a given budget) that helps his cows produce the most milk and thus nourish the most children.

FJ researched N (1 <= N <= 50) consoles, each with a console price P\_i (1 <= P\_i <= 1000) and a number of console-specific games G\_i (1 <= G\_i <= 10). A cow must, of course, own a console before she can buy any game that is specific to that console. Each individual game has a game price GP\_j (1 <= GP\_j price <= 100) and a production value (1 <= PV\_j <= 1,000,000), which indicates how much milk a cow will produce after playing the game. Lastly, Farmer John has a budget V (1 <= V <= 100,000) which is the maximum amount of money he can spend. Help him maximize the sum of the production values of the games he buys.

Consider one dataset with N=3 consoles and a V=$800 budget. The first console costs $300 and has 2 games with cost $30 and $25 and production values as shown:

Game #    Cost    Production Value

1       $30          50

2       $25          80

The second console costs $600 and has only 1 game:

Game #    Cost    Production Value

1       $50          130

The third console costs $400 and has 3 games:

Game #    Cost    Production Value

1       $40         70

2       $30         40

3       $35         60

Farmer John should buy consoles 1 and 3, game 2 for console 1, and games 1 and 3 for console 3 to maximize his expected production at 210:

```cpp
                                Production Value
        Budget:     $800      
        Console 1  -$300
           Game 2   -$25              80
        Console 3  -$400
           Game 1   -$40              70
           Game 3   -$35              60
      -------------------------------------------
        Total:         0 (>= 0)      210
```


## 输入格式
\* Line 1: Two space-separated integers: N and V

\* Lines 2..N+1: Line i+1 describes the price of and the games

available for console i; it contains: P\_i, G\_i, and G\_i pairs of space-separated integers GP\_j, PV\_j


## 输出格式
\* Line 1: The maximum production value that Farmer John can get with his budget.


## 题目大意
农夫约翰的奶牛们打游戏上瘾了！本来约翰是想要按照调教兽的做法拿她们去电击戒瘾的，可后来他发现奶牛们玩游戏之后比原先产更多的奶。很明显，这是因为满足的牛会产更多的奶。

但是，奶牛们因何者为最好的游戏主机而吵得不可开交。约翰想要在给定的预算内购入一些游戏平台和一些游戏，使他的奶牛们生产最多的奶牛以养育最多的小牛。

约翰考察了 $N$ 种游戏主机，第 $i$ 种主机的价格是 $P_i$，该主机有 $G_i$ 个独占游戏。很明显，奶牛必须先买进一种游戏主机，才能买进在这种主机上运行的游戏。在每种主机中，游戏 $j$ 的价格为 $\mathit{GP}_j$，每头奶牛在玩了该游戏后的牛奶产量为 $\mathit{PV}_j$。

农夫约翰的预算为 $V$。请帮助他确定应该买什么游戏主机和游戏，使得他能够获得的产出值的和最大。

### 样例说明 1
假设 现在有 $N=3$ 种主机，预算为 $V=800$。第一种主机的售价为 $300$，并且有两款游戏：

|游戏编号|$GP_j$|$PV_j$|
|-|-|-|
|1|$30|50|
|2|$25|80|

第二种主机的售价为 $600$，并且只有一款游戏：

|游戏编号|$GP_j$|$PV_j$|
|-|-|-|
|1|$50|130|

第二种主机的售价为 $400$，并且有三款游戏：

|游戏编号|$GP_j$|$PV_j$|
|-|-|-|
|1|$40|70|
|2|$30|40|
|3|$35|60|

理想方案：
```cpp
                              产量
           预算:    $800      
           主机 1  -$300
           游戏 2   -$25       80
           主机 3  -$400
           游戏 1   -$40       70
           游戏 3   -$35       60
      -------------------------------------------
          总和：   0 (≥ 0)     210
```

```input1
3 800 
300 2 30 50 25 80 
600 1 50 130 
400 3 40 70 30 40 35 60 

```

```output1
210 

```

