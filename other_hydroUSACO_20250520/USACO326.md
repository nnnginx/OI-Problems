## 题目描述  
农夫John发现做出全威斯康辛州最甜的黄油的方法：糖。把糖放在一片牧场上，他知道N（1<=N<=500）只奶牛会过来舔它，这样就能做出能卖好价钱的超甜黄油。当然，他将付出额外的费用在奶牛上。  
农夫John很狡猾。像以前的Pavlov，他知道他可以训练这些奶牛，让它们在听到铃声时去一个特定的牧场。他打算将糖放在那里然后下午发出铃声，以至他可以在晚上挤奶。  
农夫John知道每只奶牛都在各自喜欢的牧场（一个牧场不一定只有一头牛）。给出各头牛在的牧场和牧场间的路线，找出使所有牛到达的路程和最短的牧场（他将把糖放在那）  
## 输入格式：  
第一行: 三个数：奶牛数N，牧场数（2<=P<=800），牧场间道路数C(1<=C<=1450)  
第二行到第N+1行: 1到N头奶牛所在的牧场号  
第N+2行到第N+C+1行： 每行有三个数：相连的牧场A、B，两牧场间距离D（1<=D<=255），当然,连接是双向的  
## 输出格式：  
一行 输出奶牛必须行走的最小的距离和  
## 输入样例#1：   
```  
3 4 5  
2  
3  
4  
1 2 1  
1 3 5  
2 3 7  
2 4 3  
3 4 5  
```  
## 输出样例#1：   
```  
8  
```  
## 说明  
样例图形  
```  
          P2  
P1 @--1--@ C1  
         |
         |   
       5  7  3  
         |   
         |     C3  
       C2 @--5--@  
          P3    P4  
```  
放在4号牧场最优  