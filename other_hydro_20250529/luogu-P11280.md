## ��Ŀ����
**[English statement](https://www.luogu.com.cn/problem/T533492). You must submit your code at the Chinese version of the statement.**

������ [#3406. ��2020-2021 ��ѵ����ҵ��Tom & Jerry](https://loj.ac/p/3406)����

��˵�öԣ����ǣ�
> Tom and Jerry is an American animated media franchise and series of comedy short films created in 1940 by William Hanna and Joseph Barbera. Best known for its 161 theatrical short films by Metro-Goldwyn-Mayer, the series centers on the rivalry between the titular characters of a cat named Tom and a mouse named Jerry. Many shorts also feature several recurring characters.
> 
> In its original run, Hanna and Barbera produced 114 Tom and Jerry shorts for MGM from 1940 to 1958. During this time, they won seven Academy Awards for Best Animated Short Film, tying for first place with Walt Disney's Silly Symphonies with the most awards in the category. After the MGM cartoon studio closed in 1957, MGM revived the series with Gene Deitch directing an additional 13 Tom and Jerry shorts for Rembrandt Films from 1961 to 1962. Tom and Jerry became the highest-grossing animated short film series of that time, overtaking Looney Tunes. Chuck Jones produced another 34 shorts with Sib Tower 12 Productions between 1963 and 1967. Five more shorts have been produced since 2001, making a total of 166 shorts.
>
> A number of spin-offs have been made, including the television series The Tom and Jerry Show (1975), The Tom and Jerry Comedy Show (1980�C1982), Tom & Jerry Kids (1990�C1993), Tom and Jerry Tales (2006�C2008), and The Tom and Jerry Show (2014�C2021). In 1992, the first feature-length film based on the series, Tom and Jerry: The Movie, was released. 13 direct-to-video films have been produced since 2002. In 2021, a a live-action/animated hybrid film was released. In 2019, a musical adaptation of the series, titled Tom and Jerry: Purr-Chance to Dream, debuted in Japan, in advance of Tom and Jerry's 80th anniversary.

## ��Ŀ����
Terry �� Jom ��һ�� $n$ ���� $m$ ���ߵ��С�����������ͨͼ�ϲ��ģ�ͼ�ĸ�Ϊ $r$������ѭ���¹���

- Terry ���֣�
- ����������ͼ���ƶ���ÿ��ֻ����һ���ߣ�Ҳ����˯����ɶ�����ɣ���
- Terry �����ߵ� Jom ���ڵĽ�㣨������Ϊֻ�� Terry ��Ͷ����ʱ�Żᱻץ��������� Terry ���ƶ������ $u$ �� Jom ��ͬһ�غ�Ҳ�ƶ��� $u$ �ǺϷ��ģ���

���� $q$ ��ѯ�ʣ�ÿ��ѯ�ʸ��� Terry �� Jom ����� $a, b$������Ҫ�ش� Terry �ܷ񵽴�������� $r$����

## �����ʽ
��һ�а����������� $n, m, r$����ʾ�����������͸��ı�ţ�

������ $m$ �У�ÿ�а����������� $(u, v)$ ��ʾһ���ߣ�ע����ܴ����ر߻��Ի�����

������һ�а���һ������ $q$����ʾѯ������

������ $q$ �У�ÿ�а����������� $a, b$����ʾ Terry �� Jom ����㡣

## �����ʽ
��Ϊ����ǩ���⣬������Ӧ���ڿ�ͷ��� `I'm here!`��

������ $q$ �еĵ� $i$ �У�����ڵ� $i$ ��ѯ���� Terry �ܵ��������� `Terry`��������� `Jom`��

```input1
5 4 3
4 3
3 2
1 5
1 2
2
1 2
5 4
```

```output1
I'm here!
Jom
Jom
```

```input2
5 5 4
1 4
4 3
3 2
4 5
5 3
2
3 1
5 1
```

```output2
I'm here!
Terry
Terry
```

## ��ʾ
#### ����ʾ��

���� IO ���ϴ���ѡ��ʹ�ýϿ�Ķ��������ʽ��

#### �����ݷ�Χ��

**�������������ԡ�**

| �������� | $n, m, q \le$ |     ��������     | ��ֵ |
| :--------: | :-----------: | :--------------: | :--------: |
|    $0$     |       $10^6$       | A |    $1$     |
|    $1$     |     $10$      |        ��        |    $9$     |
|    $2$     |       $10^6$       |  B  |    $15$    |
|    $3$     |       $10^6$       | C |    $15$    |
|    $4$     |       $10^6$       |        ��        |    $60$    |

- �������� A��$q = 0$��
- �������� B����֤ͼ��һ������
- �������� C����֤ͼ��һ���ջ���

�����������ݣ����㣺

- $1 \le n, m \le 10^6$��
- $0 \le q \le 10^6$��
- $1 \le r, u, v, a, b \le n$��
- ������ͼ��һ��������ͨͼ��

