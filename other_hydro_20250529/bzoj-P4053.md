
## 题目描述
小 J 要坐地铁到小 M 家去玩。

有很多的地铁站，有很多条双向的地铁线路连接它们。

从一个站到一个直接相邻的站都只要 $1$ 分钟，换线不需要时间。

给你地铁图，你的任务是帮助小 J 安排他的路线，使得换乘（在一条线路上回头也算换乘）次数尽量少，且让他坐的尽量久。

## 输入格式

第一行一个整数 $T$，代表数据组数。

每一组测试数据如下:

每组数据用一个回车开头，接下来的两行以 `Stops:` 和 `Lines:` (不包含引号)开头，并且分别包含站点和线路的名称，之间用一个逗号和一个空格隔开。

接下来对于每条线路有单独的一行，以线路的名称加 ` route` 开头，后面包含它经过的站点，之间用一个逗号和一个空格隔开。

最后两行告诉你小 J 与小 M 的位置。

## 输出格式

对于每组测试数据，打印单独的一行代表小 J的最优线路（详情请见样例数据），保证最优路径存在。

```input1
Stops: OxfordCircus, PiccadillyCircus, HydeParkCorner, King’sCross, GreenPark, Arsenal, Victoria, Highbury&Islington, LeicesterSquare
Lines: Blue, Cyan
Cyan route: Highbury&Islington, King’sCross, OxfordCircus, GreenPark, Victoria
Blue route: HydeParkCorner, GreenPark, PiccadillyCircus, LeicesterSquare, King’sCross, Arsenal
Johny lives at King’sCross
Michelle lives at GreenPark
Stops: OxfordCircus, PiccadillyCircus, HydeParkCorner, King’sCross, GreenPark, Arsenal, Victoria, Highbury&Islington, LeicesterSquare
Lines: Blue, Cyan
Cyan route: Highbury&Islington, King’sCross, OxfordCircus, GreenPark, Victoria
Blue route: HydeParkCorner, GreenPark, PiccadillyCircus, LeicesterSquare, King’sCross, Arsenal
Johny lives at PiccadillyCircus
Michelle lives at LeicesterSquare
Stops: OxfordCircus, PiccadillyCircus, HydeParkCorner, King’sCross, GreenPark, Arsenal, Victoria, Highbury&Islington, LeicesterSquare
Lines: Blue, Cyan
Cyan route: Highbury&Islington, King’sCross, OxfordCircus, GreenPark, Victoria
Blue route: HydeParkCorner, GreenPark, PiccadillyCircus, LeicesterSquare, King’sCross, Arsenal
Johny lives at Victoria
Michelle lives at HydeParkCorner
```

```output1
optimal travel from King’sCross to GreenPark: 1 line, 3 minutes
optimal travel from PiccadillyCircus to LeicesterSquare: 1 line, 1 minute
optimal travel from Victoria to HydeParkCorner: 2 lines, 7 minutes
```


## 数据规模与约定

对于 $100\%$ 的数据， $1\le$ 站点数 $\le 3 \times 10^5$，$1\le$ 线路总长度 $\le 10^6$，$1\le$ 名称长度 $\le 50$，名称可以包括字母，数字，减号，单引号和按位与符号，保证图中没有自环。
