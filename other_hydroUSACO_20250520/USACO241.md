## 题目描述  
两只牛逃跑到了森林里。农夫John开始用他的专家技术追捕这两头牛。你的任务是模拟他们的行为(牛和John)。  
追击在10x10的平面网格内进行。一个格子可以是：  
一个障碍物, 两头牛(它们总在一起), 或者 农民John. 两头牛和农民John可以在同一个格子内(当他们相遇时)，但是他们都不能进入有障碍的格子。  
一个格子可以是：  
. 空地  
* 障碍物  
C 两头牛  
F 农民John  
这里有一个地图的例子：  
```  
*...*.....  
......*...  
...*...*..  
..........  
...*.F....  
*.....*...  
...*......  
..C......*  
...*.*....  
.*.*......  
```  
牛在地图里以固定的方式游荡。每分钟，它们可以向前移动或是转弯。如果前方无障碍(地图边沿也是障碍)，它们会按照原来的方向前进一步。否则它们会用这一分钟顺时针转90度。 同时，它们不会离开地图。  
农民John深知牛的移动方法，他也这么移动。  
每次(每分钟)农民John和两头牛的移动是同时的。如果他们在移动的时候穿过对方，但是没有在同一格相遇，我们不认为他们相遇了。当他们在某分钟末在某格子相遇，那么追捕结束。  
读入十行表示农夫John,两头牛和所有障碍的位置的地图。每行都只包含10个字符，表示的含义和上面所说的相同，你可以确定地图中只有一个'F'和一个'C'.'F'和'C'一开始不会处于同一个格子中。  
计算农夫John需要多少分钟来抓住他的牛，假设牛和农夫John一开始的行动方向都是正北（即上）。 如果John和牛永远不会相遇，输出0。  
## 输入格式：  
每行10个字符，表示如上文描述的地图。  
## 输出格式：  
输出一个数字，表示John需要多少时间才能抓住牛们。如果John无法抓住牛，则输出0。  
## 输入样例#1：   
```  
*...*.....  
......*...  
...*...*..  
..........  
...*.F....  
*.....*...  
...*......  
..C......*  
...*.*....  
.*.*......  
```  
## 输出样例#1：   
```  
49  
```  