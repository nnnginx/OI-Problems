## 题目描述
初始在 $(0, 0)$。   
给你 $N$ 个命令串，每个命令串包含若干命令，每个命令形式是 `GO LEFT RIGHT Fk` 之一。      
`GO` 往前走 $1$。  
`LEFT` 左转 $90$ 度。    
`RIGHT` 右转 $90$ 度。     
`Fk` 执行第 $k$ 个命令串。      
 
`f1: GO F2 GO F2 GO F2`     
`f2: F3 F3 F3 F3`  
`f3: GO LEFT`  
命令轨迹如图 ：  
![eg](https://hydro.ac/d/bzoj/p/2647/file/pic1.jpg)

## 输入格式
 
第一行一个 $N$。  
接下来 $N$ 行，每行一个整数 $C_i$ 表示命令数，接下来 $C_i$ 个命令。  

## 输出格式

输出曾经到达的最远的距离，如果到了无穷远，输出 `Infinity` 。

```input1
3
6 GO F2 GO F2 GO F2
4 F3 F3 F3 F3
2 GO LEFT
```

```output1
5
```

```input2
1
2 GO F1
```

```output2
Infinity
```

## 数据规模与约定

对于 $100\%$ 的数据，$1 \leq N \leq 100$，$1 \leq C_i \leq 100$。
 
## 题目来源

鸣谢Kac
Neerc2011