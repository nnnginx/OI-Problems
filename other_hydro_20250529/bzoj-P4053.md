
## ��Ŀ����
С J Ҫ��������С M ��ȥ�档

�кܶ�ĵ���վ���кܶ���˫��ĵ�����·�������ǡ�

��һ��վ��һ��ֱ�����ڵ�վ��ֻҪ $1$ ���ӣ����߲���Ҫʱ�䡣

�������ͼ����������ǰ���С J ��������·�ߣ�ʹ�û��ˣ���һ����·�ϻ�ͷҲ�㻻�ˣ����������٣����������ľ����á�

## �����ʽ

��һ��һ������ $T$����������������

ÿһ�������������:

ÿ��������һ���س���ͷ���������������� `Stops:` �� `Lines:` (����������)��ͷ�����ҷֱ����վ�����·�����ƣ�֮����һ�����ź�һ���ո������

����������ÿ����·�е�����һ�У�����·�����Ƽ� ` route` ��ͷ�����������������վ�㣬֮����һ�����ź�һ���ո������

������и�����С J ��С M ��λ�á�

## �����ʽ

����ÿ��������ݣ���ӡ������һ�д���С J��������·����������������ݣ�����֤����·�����ڡ�

```input1
Stops: OxfordCircus, PiccadillyCircus, HydeParkCorner, King��sCross, GreenPark, Arsenal, Victoria, Highbury&Islington, LeicesterSquare
Lines: Blue, Cyan
Cyan route: Highbury&Islington, King��sCross, OxfordCircus, GreenPark, Victoria
Blue route: HydeParkCorner, GreenPark, PiccadillyCircus, LeicesterSquare, King��sCross, Arsenal
Johny lives at King��sCross
Michelle lives at GreenPark
Stops: OxfordCircus, PiccadillyCircus, HydeParkCorner, King��sCross, GreenPark, Arsenal, Victoria, Highbury&Islington, LeicesterSquare
Lines: Blue, Cyan
Cyan route: Highbury&Islington, King��sCross, OxfordCircus, GreenPark, Victoria
Blue route: HydeParkCorner, GreenPark, PiccadillyCircus, LeicesterSquare, King��sCross, Arsenal
Johny lives at PiccadillyCircus
Michelle lives at LeicesterSquare
Stops: OxfordCircus, PiccadillyCircus, HydeParkCorner, King��sCross, GreenPark, Arsenal, Victoria, Highbury&Islington, LeicesterSquare
Lines: Blue, Cyan
Cyan route: Highbury&Islington, King��sCross, OxfordCircus, GreenPark, Victoria
Blue route: HydeParkCorner, GreenPark, PiccadillyCircus, LeicesterSquare, King��sCross, Arsenal
Johny lives at Victoria
Michelle lives at HydeParkCorner
```

```output1
optimal travel from King��sCross to GreenPark: 1 line, 3 minutes
optimal travel from PiccadillyCircus to LeicesterSquare: 1 line, 1 minute
optimal travel from Victoria to HydeParkCorner: 2 lines, 7 minutes
```


## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ� $1\le$ վ���� $\le 3 \times 10^5$��$1\le$ ��·�ܳ��� $\le 10^6$��$1\le$ ���Ƴ��� $\le 50$�����ƿ��԰�����ĸ�����֣����ţ������źͰ�λ����ţ���֤ͼ��û���Ի���
