## 问题描述  
奶牛 Bessie 意识到：为了保持好的体形，她需要更多地进行锻炼。她需要你帮助她选择在农场里每天用来晨跑的路线。  
农场由 N 块草地组成（$1\leq N\leq2\times10^5$），方便起见编号为 1…N，由 M 条双向的小路连接（$1\leq M\leq 2\times 10^5$）。作为一种遵循规律的生物，奶牛们倾向于使用其中特定的 N−1 条小路作为她们日常在草地之间移动的路线——她们管这些叫“常规的”小路。从每块草地出发都可以仅通过常规的小路到达所有其他草地。  
为了使她的晨跑更加有趣，Bessie 觉得她应该选择一条包含一些非常规的小路的路线。然而，使用常规的小路能够使她感到舒适，所以她不是很想在她的路线中使用过多非常规的小路。经过一些思考，她认为一条好的路线应当形成一个简单环（能够不经过任何草地超过一次的情况下回到起点），其中包含恰好两条非常规的小路。  
请帮助 Bessie 计算她可以使用的好的路线的数量。两条路线被认为是相同的，如果它们包含的小路的集合相等。  
## 输入格式  
输入的第一行包含 N 和 M。  
以下 M 行每行包含两个整数 ai 和 bi，描述了一条小路的两端。其中前 N−1 条是常规的小路。  
## 输出格式  
输出 Bessie 可以选择的路线的总数。  
## 输入样例  
```  
5 8  
1 2  
1 3  
1 4  
1 5  
2 3  
3 4  
4 5  
5 2  
```  
## 输出样例  
```  
4  
```  