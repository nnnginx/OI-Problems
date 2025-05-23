## 描述  
农夫约翰已经决定建造电网。他已经把他的农田围成一些奇怪的形状，现在必须找出安放电源的最佳位置。  
对于每段电网都必须从电源拉出一条电线。电线可以穿过其他电网或者跨过其他电线。电线能够以任意角度铺设，从电源连接到一段电网的任意一点上（也就是，这段电网的端点上或者在其之间的任意一点上）。这里所说的“一段电网”指的是呈一条线段状的电网，并不是连在一起的几段电网。若几段电网连在一起，那么也要分别给这些电网提供电力。  
已知所有的 F（1 <= F <= 150）段电网的位置（电网总是和坐标轴平行，并且端点的坐标总是整数，0 <= X,Y <= 100）。你的程序要计算连接电源和每段电网所需的电线的最小总长度，还有电源的最佳坐标。  
电源的最佳坐标可能在农夫约翰的农田中的任何一个位置，并不一定是整数。  
## INPUT FORMAT  
第一行包括 F ——电网的数量。 下面的 F 行每行包括两个 X，Y 对，表示这段电网的两个端点。  
(ps:数据中有电网是点的情况，即 68 97 68 97，这貌似与题目叙述不符，请注意 //from Error)（路人甲：貌似照做就行了，不用管，。。。）  
## OUTPUT FORMAT  
只有一行，输出三个浮点数，每个保留1位小数。假定你的电脑的输出库会正确地对小数进行四舍五入。  
这三个数是：电源最佳坐标的 X 值， 电源最佳坐标的 Y 值，和 需要的电线的总长度（要最小）。  
## SAMPLE INPUT (file fence3.in)  
```  
3  
0 0 0 1  
2 0 2 1  
0 3 2 3  
```  
## SAMPLE OUTPUT (file fence3.out)  
```  
1.0 1.6 3.7  
```  
  
## Description  
Farmer John has decided to construct electric fences. He has fenced his fields into a number of bizarre shapes and now must find the optimal place to locate the electrical supply to each of the fences.  
A single wire must run from some point on each and every fence to the source of electricity. Wires can run through other fences or across other wires. Wires can run at any angle. Wires can run from any point on a fence (i.e., the ends or anywhere in between) to the electrical supply.  
Given the locations of all F (1 <= F <= 150) fences (fences are always parallel to a grid axis and run from one integer gridpoint to another, 0 <= X,Y <= 100), your program must calculate both the total length of wire required to connect every fence to the central source of electricity and also the optimal location for the electrical source.  
The optimal location for the electrical source might be anywhere in Farmer John's field, not necessarily on a grid point.  
## INPUT FORMAT  
The first line contains F, the number of fences.  
F subsequent lines each contain two X,Y pairs each of which denotes the endpoints of a fence.  
## SAMPLE INPUT (file fence3.in)  
```  
3  
0 0 0 1  
2 0 2 1  
0 3 2 3  
```  
## OUTPUT FORMAT  
On a single line, print three space-separated floating point numbers, each with a single decimal place. Presume that your computer's output library will round the number correctly.  
The three numbers are:  
the X value of the optimal location for the electricity,  
the Y value for the optimal location for the electricity, and  
the total (minimum) length of the wire required.  
## SAMPLE OUTPUT (file fence3.out)  
```  
1.0 1.6 3.7  
```  