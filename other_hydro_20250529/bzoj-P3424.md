## 题目描述

Byteasar lives in Byteburg, a city famous for its milk bars on every corner. One day Byteasar came up with an idea of a "milk multidrink": he wants to visit each milk bar for a drink exactly once. Ideally, Byteasar would like to come up with a route such that the next bar is always no further than two blocks (precisely: intersections) away from the previous one. 

The intersections in Byteburg are numbered from 1 to N, and all the streets are bidirectional. Between each pair of intersections there is a unique direct route, ie, one that does not visit any intersection twice. Byteasar begins at the intersection no. 1 and finishes at the intersection no. N. **Your task is to find any route that satisfies Byteasar's requirements if such a route exists.**
 
给一棵树，输出遍历序列a[]，要求每个节点被访问到到恰好一次  要求从1号节点出发，结束在n号节点 要求对于所有i,a[i]与a[i+1]的距离 小于等于2 

## 输入格式

In the first line of the standard input there is a single integer N(2<=N<=500000) , denoting the number of intersections in Byteburg. Each of the following N-1 lines holds a pair of distinct integers Ai and Bi(1<=Ai,Bi<=N)  separated by a single space, that represent the street linking the intersections no. Ai and Bi. 


## 输出格式

If there is no route satisfying Byteasar's requirements, your program should print a single word "<tt> **BRAK** </tt>" (Polish for none), without the quotation marks to the standard output. Otherwise, your program should print N lines to the standard output, the i-th of which should contain the number of the i-th intersection on an arbitrary route satisfying Byteasar's requirements. Obviously, in that case the first line should hold the number 1, and the N-th line - number N. 

```input1
12
1 7
7 8
7 11
7 2
2 4
4 10
2 5
5 9
2 6
3 6
3 12
```

```output1
1
11
8
7
4
10
2
9
5
6
3
12

```
## 提示
没有写明提示
## 题目来源
鸣谢Wcmg提供SPJ 译文
								
							
						
					
				
				
				
			
		
	
