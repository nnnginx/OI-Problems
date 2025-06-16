## ��Ŀ����
### ������������������е���ʾ����ô������������������

![](https://cdn.luogu.com.cn/upload/image_hosting/n87yncfw.png)

## ��Ŀ����
lhm ������һ���ַ��� $a$ �������Ӵ� $b$��������Ҫ����ַ��� $a$��

�� $c(s,b)$ ��ʾ���ַ��� $s$ ��ѡ��һЩ�����ص��ġ��� $b$ ��ͬ���Ӵ�������Ӵ�������

���� $a$ ���Ϊ $k$ �飬�� $i$ ���Ϊ $p_i$������Ҫ��֤��
- $k \geq 2$��
- $c(p_{i+1},b)>c(p_i,b)\ (i \in[1,k-1])$��
- $c(p_1,b)\geq 1$��

���ֲ�ַ�����ͬ���ҽ�����ֳ����������Ȼ� $\exist i$����Ӧ�� $c(p_i,b)$ ���ȡ�

��ͬ�Ĳ�ַ����������𰸶� $899678209$ ȡģ��

## �����ʽ
�������ݹ����С�

��һ��һ���ַ��� $a$������������ʾ��

�ڶ���һ���ַ��� $b$������������ʾ��

## �����ʽ
������ݹ�һ�С�

һ��һ����������ʾ��ֵķ������� $899678209$ ȡģ�Ľ����

```input1
noinoinonoinoiionoinoinoionoi
noi
```

```output1
10
```

## ��ʾ
���������͡�

��ֵķ�ʽ�ֱ�Ϊ��

`noi noinonoi noiionoinoinoionoi`�������ֱ�Ϊ $1,2,5$��

`noi noinonoin oiionoinoinoionoi`�������ֱ�Ϊ $1,2,4$��

`noino inonoinoiion oinoinoionoi`�������ֱ�Ϊ $1,2,3$��

`noi noinonoinoi ionoinoinoionoi`�������ֱ�Ϊ $1,3,4$��

`noi noinonoinoiionoinoinoionoi`�������ֱ�Ϊ $1,7$��

`noinoi nonoinoiionoinoinoionoi`�������ֱ�Ϊ $2,6$��

`noinoinonoi noiionoinoinoionoi`�������ֱ�Ϊ $3,5$��

`noin oinonoinoiionoinoinoionoi`�������ֱ�Ϊ $1,6$��

`noinoinono inoiionoinoinoionoi`�������ֱ�Ϊ $2,5$��

`noinoinonoin oiionoinoinoionoi`�������ֱ�Ϊ $3,4$��

**��ʾ��������������˵�����Բ���Ӵ�**��

�����ݹ�ģ��Լ����

����ϸ�Ķ�������

**�������������ԡ�**  

�� $n = c(a,b)$��$|a|=l_1$��$|b|=l_2$��  

| Subtask | �������� | �ռ����� | ��ֵ | 
| :----------: | :----------: | :----------: | :----------: |
| 1 | $l_1\leq 30$ | 256MiB | 9 |
| 2 | $n \le 300$ | 256MiB | 11 |
| 3 | $n \le 2000$ | 256MiB | 17 |
| 4 | $n \le 25000$ | 256MiB | 37 |
| 5 | �� | 64MiB | 26 |

���� $100\%$ �����ݣ�$0\le n\le2\times10^5$��$2\le l_2\le l_1\le10^6$��$b_1 \neq b_{l_2}$��$a$ �� $b$ ֻ����Сд��ĸ��

