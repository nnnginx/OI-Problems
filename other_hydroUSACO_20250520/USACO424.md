## Description  
秀·谢夫（小奶牛）在花花公子杂志上中了大奖，于是她从农村搬到了城郊的一座别墅中。可是她还常常怀念乡村的生活，总想回到原来的农村逛逛。为了环保，秀决定骑上为她量身定做的奶牛自行车（特殊的自行车，专门为牛蹄设计）。  
秀大约有一吨重。同样的，秀在普通的奶牛自行车上，要想骑得平平稳稳，也不是一件容易的事。因此，调节奶牛自行车的变速器让秀心力憔悴。  
帮助秀选择她的奶牛自行车前面 F （$1 \le F \le 5$）个齿轮和后面 R （$1 \le R \le 10$）个齿轮，使她的  
$F\timesR$ 奶牛自行车符合下面的标准：  
前面齿轮的型号（齿的数量）必须在给定的范围内。  
后面齿轮的型号（齿的数量）必须在给定的范围内。  
在每一种齿轮组合中，传动比率就是前面齿轮的齿数除以后面齿轮的齿数所得的商。  
最大的传动比率至少是最小的三倍。  
齿轮组合的转动比率（已排好序）相邻两项的差的的方差（见下面的例子） 应该达到最小。  
按照下面的公式计算平均数与方差（xi 代表数据） ：  
### $$\bar{x}=\frac{1}{n}\sum_{i=1}^n x_i$$  
### $$F=\frac{1}{n}\sum_{i=1}^n (x_i-\bar{x})^2$$  
计算并确定最佳齿轮组合（其中 F 个前齿轮，R 个后齿轮），使方差最小。  
  
> Having made a fortune on Playbov magazine, Hugh Heifer has moved from his original field in the country to a fashionable yard in the suburbs. To visit fond pastoral memories, he wishes to cowmmute back to his old stomping grounds. Being environmentally minded, Hugh wishes to transport himself using his own power on a Cowcycle (a bicycle specially fitted for his neatly manicured hooves).  
> Hugh weighs over a ton; as such, getting smoothly up to speed on traditional cowcycle gear sets is a bit challenging. Changing among some of the widely spaced gear ratios causes exertion that's hard on Hugh's heart.  
> Help Hugh outfit his Cowcycle by choosing F (1 <= F <= 5) gears (sprockets) in the front and R (1 <= R <= 10) gears in the rear of his F * R speed cowcycle subject to these rules:  
> The possible sizes (number of teeth) for the F front gears are specified.  
> The possible sizes (number of teeth) for the R rear gears are specified.  
> At any given gear setting, the gear ratio is the quotient of the number of teeth on the front gear and the number of teeth on the rear gear (i.e., number of front gear teeth divided by number of rear gear teeth)  
> The largest gear ratio must be at least three times the smallest.  
> The variance (see below) of the set of DIFFERENCES between successive (i.e., after sorting) gear ratios should be minimized.  
Calculate the mean and variance of a set of differences (xi in this formula) by the following formulae:  
> Deduce and print the optimal sets of F front gears and R rear gears so that the variance is minimized (and the ratios span a factor of at least 3x).  
  
## INPUT FORMAT  
第一行是 F 和 R，表示前齿轮和后齿轮的数量。  
第二行包括 4 个数字：F1，F2（25 <= F1 < F2 <= 80），R1，R2（5 <= R1 < R2 <= 40）。从 F1 到 F2 型号的前齿轮都是可用的；从 R1 到 R2 型号的后齿轮都是可用的。至少会有一组合法的解。  
  
> The first line contains F and R, the numbers of front and rear gears. The second line contains four numbers: F1, F2 (25 <= F1 < F2 <= 80), R1, and R2 (5 <= R1 < R2 <= 40). All front gears from F1 through F2 are available; all rear gears from R1 through R2 are available. There will exist at least one legal set of gears.  
  
## SAMPLE INPUT  
```  
2 5  
39 62 12 28  
```  
## OUTPUT FORMAT  
在第一行从小到大输出前齿轮的型号，用空格分开。在第二行从小到大输出后齿轮的型号，同样用空格分开。当然，齿轮的齿数一定是整数。  
如果有多个解，输出前齿轮齿数最小的那一个（第一个齿轮齿数最小的，若第一个齿轮齿数相等，输出第二个齿轮齿数最小的……依此类推）。如果所有的前齿轮齿数都相等，照着上面的办法处理后齿轮（其实就是把第一个，第二个……齿轮分别设为第一，第二……个关键字来排序）。  
  
> Display the number of teeth on the set of F chosen front gears, from smallest to largest, on the first line of output (separated by spaces). Display the number of teeth on the set of R chosen rear gears, from smallest  
to largest, on the second line of output. All gears have an integer number of teeth, of course.  
> If multiple optimal answers exist, output the answer with the smallest front gear set (smallest first gear, or smallest second gear if first gears match, etc.). Likewise, if all first gears match, output the answer  
with the smallest rear gear set (similar rules to the front gear set).  
  
## SAMPLE OUTPUT  
```  
39 53  
12 13 15 23 27  
```  
## Comment  
这个问题最大的挑战就是“读懂题目”。慢慢读，不要想一步登天。如果你读不懂题目，还是得一遍一遍的把它读进去。  
问题要我们找出“最佳齿轮组合”，即传动比率最接近平均数的组合。考虑下面的测试数据：  
2 5  
39 62 12 28  
这意味着有 2 个前齿轮，型号范围在 39..62 ；5个后齿轮，型号范围在 12..28。程序必须检查所有前齿轮组成的有序对（共 62-39+1=24 种齿轮），和所有后齿轮组成的五元组（共 28-12+1=17 种齿轮）。根据组合数学原理，总共有 24!/22!/2! x 17!/5!/12! = 656,880 种可能（我是这么认为的）。  
对于每一种可能，做下面的计算。举个例子来说，对于枚举到的第一种情况：前齿轮是 39 和 40，后齿轮是 12，13，14，15 和 16。  
首先，计算所有可能的传动比率：  
  
```  
39/12 = 3.25000000000000000000  
39/13 = 3.00000000000000000000  
39/14 = 2.78571428571428571428  
39/15 = 2.60000000000000000000  
39/16 = 2.43750000000000000000  
40/12 = 3.33333333333333333333  
40/13 = 3.07692307692307692307  
40/14 = 2.85714285714285714285  
40/15 = 2.66666666666666666666  
40/16 = 2.50000000000000000000  
```  
  
然后，对它们进行排序：  
  
```  
39/16 = 2.43750000000000000000  
40/16 = 2.50000000000000000000  
39/15 = 2.60000000000000000000  
40/15 = 2.66666666666666666666  
39/14 = 2.78571428571428571428  
40/14 = 2.85714285714285714285  
39/13 = 3.00000000000000000000  
40/13 = 3.07692307692307692307  
39/12 = 3.25000000000000000000  
40/12 = 3.33333333333333333333  
```  
  
然后，计算差的绝对值：  
  
```  
2.43750000000000000000 - 2.50000000000000000000 = 0.06250000000000000000  
2.50000000000000000000 - 2.60000000000000000000 = 0.10000000000000000000  
2.60000000000000000000 - 2.66666666666666666666 = 0.06666666666666666666  
2.66666666666666666666 - 2.78571428571428571428 = 0.11904761904761904762  
2.78571428571428571428 - 2.85714285714285714285 = 0.07142857142857142857  
2.85714285714285714285 - 3.00000000000000000000 = 0.14285714285714285715  
3.00000000000000000000 - 3.07692307692307692307 = 0.07692307692307692307  
3.07692307692307692307 - 3.25000000000000000000 = 0.17307692307692307693  
3.25000000000000000000 - 3.33333333333333333333 = 0.08333333333333333333   
```  
  
然后计算平均数和方差。  
平均数是（我是这么认为的）0.0995370370370370370366666.。方差大约是 0.00129798488416722。  
当然这个例子是错误的，因为它的最大传动比率没有比最小传动比率大3倍。  
找出一个组合，拥有最小的方差，同时最大传动比率至少是最小传动比率的3倍。  
  
> The challenge in this problem is "reading the problem". Don't read further if you are working on that level of challenge. If the problem is just completely unclear to you, read in.  
The problem wants you to find "an optimal set of gear ratios" such that the spacing between the ratios is most uniform. Consider the test case above:  
2 5  
39 62 12 28  
This specifies two front gears from the set 39..62; five rear gears from the set 12..28. The program must examine all possible pairs of 62-39+1=24 front gears and all possible quintuples from 28-12+1=17 rear  
gears. Combinatorically, The total number of possibilities is (24 take 2) times (17 take 5), which is 24!/22!/2! x 17!/5!/12! which is 656,880 possibilities (I think).  
For each of these possibilities, calculations like the following. This example considers in some sense the "first" case: front gears of 39 and 40, rear gears of 12, 13, 14, 15, and 16.  
First, calculate all the possible ratios:  
```  
39/12 = 3.25000000000000000000  
39/13 = 3.00000000000000000000  
39/14 = 2.78571428571428571428  
39/15 = 2.60000000000000000000  
39/16 = 2.43750000000000000000  
40/12 = 3.33333333333333333333  
40/13 = 3.07692307692307692307  
40/14 = 2.85714285714285714285  
40/15 = 2.66666666666666666666  
40/16 = 2.50000000000000000000  
```  
Then, sort them:  
```  
39/16 = 2.43750000000000000000  
40/16 = 2.50000000000000000000  
39/15 = 2.60000000000000000000  
40/15 = 2.66666666666666666666  
39/14 = 2.78571428571428571428  
40/14 = 2.85714285714285714285  
39/13 = 3.00000000000000000000  
40/13 = 3.07692307692307692307  
39/12 = 3.25000000000000000000  
40/12 = 3.33333333333333333333  
```  
Then, calculate the absolute value of the differences:  
```  
2.43750000000000000000 - 2.50000000000000000000 = 0.06250000000000000000  
2.50000000000000000000 - 2.60000000000000000000 = 0.10000000000000000000  
2.60000000000000000000 - 2.66666666666666666666 = 0.06666666666666666666  
2.66666666666666666666 - 2.78571428571428571428 = 0.11904761904761904762  
2.78571428571428571428 - 2.85714285714285714285 = 0.07142857142857142857  
2.85714285714285714285 - 3.00000000000000000000 = 0.14285714285714285715  
3.00000000000000000000 - 3.07692307692307692307 = 0.07692307692307692307  
3.07692307692307692307 - 3.25000000000000000000 = 0.17307692307692307693  
3.25000000000000000000 - 3.33333333333333333333 = 0.08333333333333333333  
```  
Then, calculate the mean and variance of the set of numbers on the right, above. The mean is (I think): 0.0995370370370370370366666. The variance is approximately 0.00129798488416722.  
Of course this set of gears is not valid, since it does not have a 3x span from highest gear to lowest.  
Find the set of gears that minimizes the variance and has a 3x or greater span.   