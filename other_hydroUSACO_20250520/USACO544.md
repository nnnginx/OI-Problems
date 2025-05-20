翻译  
一个正方形的镇区分为 $N\times N$ 个小方块（1 <= N <= 7）。农场位于方格的左上角，集市位于左下角。贝茜穿过小镇，从左上角走到左下角，刚好经过每个方格一次。当 N=3 时，贝茜的漫游路径可能如下图所示：  
  
```  
----------------  
|    |    |    |
| F**********  |
|    |    | *  |
------------*---  
|    |    | *  |
|  *****  | *  |
|  * | *  | *  |
---*---*----*---  
|  * | *  | *  |
|  M | ******  |
|    |    |    |
----------------  
```  
  
写一个程序，对于给出的 N 值，计算贝茜从农场走到集市有多少种唯一的路径。  
## INPUT FORMAT  
行 1: 一个整数 N （1 <= N <= 7）  
## OUTPUT FORMAT  
只有一行。输出一个整数表示唯一路径的数量。  
## SAMPLE INPUT  
3  
## SAMPLE OUTPUT  
2  
  
## Description  
A square township has been divided up into N2 square plots (1 <= N <= 7). The Farm is located in the upper left plot and the Market is located in the lower left plot. Betsy takes her tour of the township going from Farm to Market by walking through every plot exactly once. Shown below is one possible tour for Betsy when N=3.  
  
```  
----------------  
|    |    |    |
| F**********  |
|    |    | *  |
------------*---  
|    |    | *  |
|  *****  | *  |
|  * | *  | *  |
---*---*----*---  
|  * | *  | *  |
|  M | ******  |
|    |    |    |
----------------  
```  
  
Write a program that will count how many unique tours Betsy can take in going from Farm to Market for any value of N.  
## INPUT FORMAT  
Line 1: A single integer N (1 <= N <= 7)  
## SAMPLE INPUT (file betsy.in)  
3  
## OUTPUT FORMAT  
A single line with a single integer, the number of unique tours.  
## SAMPLE OUTPUT (file betsy.out)  
2  