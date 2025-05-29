## ��Ŀ����
![Mirror](https://mivik.gitee.io/image/nurture/mirror.png)

> And it��s not the voice of all the others
>
> You��ve only said it to yourself
>
> I know what you want from me, from me
>
> I know what you��re thinking

## ��Ŀ����
> Porter Robinson: We all have these avatars that we give to our critical inner voices - we might imagine a scornful parent telling us we��ll fail, or a critic telling us our work comes up short, or a society telling us that we aren��t good enough - it��s about recognizing that most of this criticism is self-inflicted.

Mivik �ھ��п������Լ��� Inner Voice ������������һ�����Ӱ�ԳƵ��Թ��С�����Թ������⣺����������к�������У��к��ж��� $0$ ��ʼ��š�һ������ $(i,j)$ ��ͨ����û���ϰ������ҽ��� $(i\&j)=0$������ $\&$ ָ��λ�����㣨Bitwise And��[�ٶȰٿ�](https://baike.baidu.com/item/%E6%8C%89%E4%BD%8D%E4%B8%8E/9601818)������ͼ����������Թ��� $0\sim63$ �к� $0\sim 63$ �е�ͼ��

![�Թ�](https://cdn.luogu.com.cn/upload/image_hosting/das5c73w.png)

Mivik ��ץ���������Ǹ������Լ����������� Inner Voice�������Ҳ���·�ˡ�Mivik �� Inner Voice ��������Թ��е����㡣Mivik ��֪������ Mivik �� Inner Voice һֱ���ƶ�������£���������Ҫ�߹����ٸ��������ץ������ Inner Voice��Mivik ����ʼ���㣩��

����... ��Ϸ�������� Mivik �����һ���򵥡�а��� ggy ������Թ��е�ĳЩ���Ӳ��������ը����Mivik ��Ҫ������ǲ���̤����Щ���ӡ�Mivik ��Ҫ��������������߹��ķ��������ٵ�����£���������Ҫ�����Щը����

**��ע��ը�����ܻ��غϣ�����ֻ�в��һ�������ϵ�����ը������ͨ��������ӡ�����ը����������غϡ�**

## �����ʽ
��һ��һ������ $n$������ ggy ���µ�ը��������

������ $n$ �У�**���е�**�� $i$ �������Ǹ����������� $i$ ��ը�������꣨�� 1 ��ʼ��ţ���

������һ�������Ǹ����� $sx$ �� $sy$������ Mivik λ����һ����һ�С�

������һ�������Ǹ����� $ex$ �� $ey$������ Mivik �� Inner Voice λ����һ����һ�С�

## �����ʽ
��һ��һ������������ Mivik ������Ҫ���ٸ����ץ������ Inner Voice��

������һ�У�����һ������Ϊ $n$ �� 01 ������ $i$ ���ַ�Ϊ `1` ���� Mivik �������� $i$ ��ը����`0` ������Ҫ��

```input1
0
0 0
0 2
```

```output1
2

```

```input2
3
0 0
0 2
1 2
4 2
3 4
```

```output2
13
110
```

```input3
0
12 34
3 100
```

```output3
85

```

## ��ʾ
### ��������

����һ����Ȼ����û���κ�ը����Mivik �������������ץ������ Inner Voice��

��������Mivik �����·����ͼ��ʾ��

![·��](https://cdn.luogu.com.cn/upload/image_hosting/mg0hmhgs.png)

���У�ͼƬ���Ͻ�Ϊ $(0,0)$����ɫ���� Mivik ����ʼλ�ã���ɫ���� Inner Voice ��λ�ã���ɫ���� Mivik �����·������ɫ����ը������ɫ����ʵ�ǻ�ɫ + ��ɫ������ Mivik ��������ը����

### ���ݷ�Χ

����ȫ�����ݣ��� $1\le n\le 2\cdot 10^5$��$(sx,sy)\ne(ex,ey)$������֤���ڸ������κ����� $(x,y)$ ���� $x\&y=0$ �� $0\le x,y\le 10^{18}$��

Subtask 1 (10 pts)����֤ Mivik ����ֱ�ߣ�ֻ�� ��/��/��/�� �ߣ�ץ������ Inner Voice��

Subtask 2 (15 pts)����֤ $sx=sy=0$��

Subtask 3 (20 pts)����֤ $0\le(\text{���� x,y ����})\le 100$��

Subtask 4 (25 pts)����֤ $n=0$��

Subtask 5 (30 pts)�����������ơ�

