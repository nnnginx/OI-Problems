## ��Ŀ����
_����û����˶�����һ���_

��������Ϊ�˻��䣬����Ϊ�˸��Ӳ��á�

���ӵ�е�ֻ����������ţ������е�һ�ж������ｻ������������Ŭ���뺹ˮ�̳ɵ�·������ȥ�����Ǵ����ѡ�񡪡�������Ϊ��ϲŭ���ֹ���

**ףÿһλ������Ĳ����߶���ȡ������ĳɼ���**


## ��Ŀ����
PION2202 ��ѡ�ִ��빫���ˡ���Ϊһ��~~������д��ʮ���Ի���Ϊ����~~���ˣ��㵱Ȼ��Ҫ���ȰѴ����еĸ����¼�����������

���ȹ�ע�Ŀ϶��Ǵ�ҵ��ļ����������ûд�ԡ����Ѿ���С E ��ÿ�������Ŀ���ƺ�ÿλѡ�ֵ� `freopen` �����������ˡ�

PION2202 һ���� $m$ ���⣬�� $n$ λѡ�ֲ��롣�������ѡ�ֳַ����ࣺ

1. ��ͨ�ˣ������������� `freopen` ��䣻
2. �������ˣ���ע�͵� `freopen` ��䣻
3. �����ˣ�������ʽ�� `freopen` ��䡣

��ʽ���أ���ͨ�˵�������Ŀ�� `freopen` ��䶼Ӧ��ǡ����

```cpp
freopen("<title>.in","r",stdin);
freopen("<title>.out","w",stdout);
```

���е� `<title>` Ӧ�滻�ɶ�Ӧ����Ŀ���ơ�

�������˵� `freopen` ����д�������һ���������һ������� `//freopen(` ��ͷ���� `);` ��β��

���һλѡ�ֵ� `freopen` ��䲻����������������������λѡ��Ϊ�����ˡ�

����Ҫ�ж�ÿλѡ������ͨ�ˣ��������˻��������ˡ�

## �����ʽ
��һ��һ�������� $T$����ʾ�������š�

�ڶ������������� $n,m$���ֱ��ʾѡ��������Ŀ����

������ $m$ �У�ÿ�а���һ������Сд��ĸ���ɵ��ַ��������е� $i$ �б�ʾ�� $i$ ����Ŀ����Ŀ���ơ���֤��Ŀ���Ƶĳ����� $1$ �� $10$ ֮�䡣

������ $n\times(2m+1)$ �У���ÿ $2m+1$ ���У���һ��Ϊ���У��� $2m$ �б�ʾһλѡ�ֵ�������Ŀ�� `freopen` ��䣬������Ŀ˳�������ǰ����Ϊ��һ��� `freopen` ��䣬�������ƣ��������Ϊ���һ��� `freopen` ��䡣

��֤���е� `freopen` ����ÿ���ַ��� ASCII ����� $33$ �� $126$ ֮�䣬�������ո�Ȳ��ɼ��ַ���

��֤ÿһ�� `freopen` ���ĳ����� $1$ �� $100$ ֮�䡣

## �����ʽ
��� $n$ �У����е� $i$ �б�ʾ�� $i$ λѡ�ֵķ��ࡣ

�������ͨ�ˣ���Ҫף�� RP++�����Ծ����һ�� `PION2202 RP++.`��

����Ǽ������ˣ��Ǿ�ֻ�����һ�� `Wrong file operation takes you to your ancestors along with your 3 years' efforts on OI.`��

����������ˣ���ף������ÿ��ĵ�ͬʱע�ⲻҪŪ���ˣ��������һ�� `Good luck and have fun.`��

```input1
3
4 4
tnalp
woem
kcarrab
hctam

freopen("tnalp.in","r",stdin);
freopen("tnalp.out","w",stdout);
freopen("woem.in","r",stdin);
freopen("woem.out","w",stdout);
freopen("kcarrab.in","r",stdin);
freopen("kcarrab.out","w",stdout);
freopen("hctam.in","r",stdin);
freopen("hctam.out","w",stdout);

freopen("tnalp.in","r",stdin);
freopen("tnalp.out","w",stdout);
//freopen("woem.in","r",stdin);
freopen("woem.out","w",stdout);
freopen("kcarrab.in","r",stdin);
//I_AK_IOI!!!
freopen("hctam.in","r",stdin);
freopen("hctam.out","w",stdout);

freopen("tnalp.in","r",stdin);
freopen("tnalp.out","w",stdout)
freopen("owem.in","r",stdin);
freopen("woem.out","w",stdout);
freopen("kcarrab.in","r",stdout);
freopen("kcarrab.out","w",stdin);
freopen("hctam.out","w",stdout);
freopen("hctam.in","r",stdin);

freopen("tnalp.in","r",stdin);//I_LOVE_CCF
freopen("tnalp.out","w",stdout);
freopen("woem.in","r",stdin);//I_HATE_THIS
freopen("woem.out","w",stdout);
freopen("kcarrab.in"/*I_FORGET_HOW_TO_FIND_BRIDGES!!!!!!*/,"r",stdin);
freopen("kcarrab.out","w",stdout);
freopen("hctam.in","r",stdin);//I_CAN_GET_ONLY_8PTSqwq
freopen("hctam.out","w",stdout);

```

```output1
PION2202 RP++.
Wrong file operation takes you to your ancestors along with your 3 years' efforts on OI.
Good luck and have fun.
Good luck and have fun.

```

## ��ʾ
**���������͡�**

��һλѡ�����е� `freopen` ��䶼����������������ͨ�ˡ�

�ڶ�λѡ��ע������Ŀ `woem` �������ļ���䣬�����Ǽ������ˡ���Ȼ��ѡ������Ŀ `kcarrab` ����������Ϊ�������Ѿ������˼������˵����������Ը�ѡ�ֱ�����Ϊ�������ˡ�

����λѡ���ĵ���� `freopen` ��䶼���������ġ�`tnalp` ������ļ�������˷ֺţ�`woem` ������� `owem`������ `kcarrab` һ���е� `stdin` �� `stdout`�������� `hctam` ����������˳���ڱ��������������ˡ�

����λѡ�ֵ� `freopen` �����Ȼ�ܹ�����������������Ϊ�������� `freopen` ��䲻ͬ���ڱ����б����������ˡ�

---

**�����ݷ�Χ��**

**�������������ԡ�**

������ 1��30 �֣���$T = 1$��$m = 1$ ����Ŀ����Ϊ `yxalag`�����ǣ��������� `No, general!` �ǲ��ܵõ������ġ�  
������ 2��30 �֣���$T = 2$����֤û�м������ˡ�  
������ 3��40 �֣���$T = 3$�����������ʡ�

���� $100\%$ �����ݣ�

- ��֤ $1\le T \le 3$��
- ��֤ $1\le n\le 1000$��
- ��֤ $1\le m \le 4$��
- ��֤��Ŀ���Ƶĳ����� $1$ �� $10$ ֮�䡣
- ��֤ÿһ�� `freopen` ���ĳ����� $1$ �� $100$ ֮�䡣

