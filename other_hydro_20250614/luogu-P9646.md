## ��Ŀ����
Paper-cutting is one of the oldest and most popular folk arts in China. It can be geographically divided into a southern and a northern style. The southern style, represented by works from Yangzhou in Jiangsu Province and Yueqing in Zhejiang Province, features ingenious and beautiful designs, exquisite carving and interesting shapes. The northern style, mainly from Yuxian and Fengning in Hebei Province and best represented by works from northern Shaanxi, features exaggerated shapes, vigorousness, vivid depictions, and diverse patterns.

There are basic cut-outs, consisting of a single image, and symmetrical designs, that are usually created by some folding over a proportioned crease, and then cutting a shape, so that when unfolded, it forms a symmetrical design. Chinese paper cuttings are usually symmetrical. The paper cutouts are usually in an even number series of $2$, $4$, $24$, etc.

You are given a piece of paper in the shape of a matrix of size $n \times m$. It is partitioned into $n \times m$ blocks of size $1 \times 1$. The piece of paper can be folded in the following way:

- You choose a vertical line between two of its columns or a horizontal line between two of its rows. This line splits the paper into two sides. 
- You use the line as the folding axis and fold the smaller side of the paper onto the larger one going over the axis. If both sides of the paper are of equal size, you may fold from either side.

You would like to make a paper-cutting masterpiece from this paper. At first, you fold the paper using the method above several times (including zero times). Then you use scissors to cut the paper. Each time you cut, you can cut out a connected component from the folded paper (even if the component is not reachable from outside) and throw it away. Note that two $1 \times 1$ blocks are connected if they share an edge.

Given the final look of the paper, which is a matrix of size $n \times m$ containing $0$s and $1$s, you would like to know the minimum number of cuts needed when using the scissors. 


## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$, indicating the number of test cases. For each test case:

The first line contains two integers $n$ and $m$ ($1 \le n \times m \le 10^6$): the size of the paper.

Each of the next $n$ lines contains a binary string of length $m$, where $\texttt{0}$ means the $1 \times 1$ block is cut out and $\texttt{1}$ means the $1 \times 1$ block remains on the final paper-cutting.

It is guaranteed that the sum of $n \times m$ over all test cases does not exceed $10^6$.

## �����ʽ
For each test case output one line containing one integer, indicating the minimum number of cuts needed.

## ��Ŀ����
��ֽ���й�����ϡ����ܻ�ӭ���������֮һ�����ڵ����Ͽ��Է�Ϊ�Ϸ����ͱ�������Խ������ݡ��㽭������ƷΪ������Ϸ��������������ۣ���̾�����������Ȥ����������Ժӱ�ε�ء�����Ϊ���壬���±���ƷΪ�������Ϳ��š����ƻֺꡢ�̻�������ͼ��������

�����Ĳü��ɵ���ͼ����ɣ����жԳƵ���ƣ�ͨ����ͨ���ڳɱ������ۺ����۵���Ȼ��ó�һ����״����չ��ʱ�����γ��˶ԳƵ���ơ��й���ֽͨ���ǶԳƵġ���ֽͨ���� $2$�� $4$ �� $24$ ��ż��ϵ�С�

���õ�һ�Ŵ�СΪ $n \times m$ ��ֽ�� ��������Ϊ $n \times m$ ����СΪ $1 \times 1$ �Ŀ��ڡ�����ֽ���԰����·�ʽ�۵���

- ����������֮��ѡ��һ����ֱ�ߣ�Ҳ����������֮��ѡ��һ��ˮƽ�ߡ������߰�ֽ�ֳ����档

- ������������Ϊ�Գ��ᣬ��С��һ���۵����һ���ϡ����ֽ�������С��ȣ������߶��ۡ�

����������ֽ��һ����ֽ���������ȣ�ʹ������������ֽ���۵����Σ�������Σ���Ȼ�����ü�����ֽ��ÿ�μ���ʱ�������Դ��۵���ֽ�ϼ��г�һ�����ӵĲ��֣���ʹ�������޷��Ӵ����ò��ֲ������ӵ�����ע�⣬������� $ 1\times 1$ �Ŀ鹲��һ���ߣ������������ӵġ�

ֽ�ŵ����������һ������ $0$ �� $1$ �Ĵ�СΪ $n \times m$ �ľ�������֪����Ҫʹ�ü���ʱ����С�ü�������

## �����ʽ

�ж���������ݡ�����ĵ�һ�а���һ������ $T$ ����ʾ�������ݵ�����������ÿ���������ݣ�

��һ�а����������� $n$ �� $m$ ( $1 \le n \times m \le 10^6$ )��ʾֽ�ŵĴ�С��

�������� $n$ ���е�ÿһ�ж�����һ������Ϊ $m$ ��01�ַ��������� $\texttt{0}$ ��ʾ $1\times 1$ �鱻���е��� $\texttt{1}$ ��ζ�� $1 \times 1$ �鱣�������ļ�ֽ�ϡ�

��֤���в������ݵ� $n \times m$ ֮�Ͳ����� $10^6$ ��

## �����ʽ

����ÿ�������������һ�У����а���һ����������ʾ�������С�ü�������

## ���� #1

### �������� #1

```
3
2 5
11001
11001
5 7
1001100
0110011
0101101
0010010
1000000
3 2
11
11
11
```

### ������� #1

```
1
4
0
```

## ��ʾ

��������һ,�����ͨ�����ַ�ʽ��Ψһ�� $0$ ����:
$$\begin{array}{ccc|cc} 1&1&0&0&1\\1&1&0&0&1\end{array} \to \begin{array}{ccc} 1&1&0\\ \hline 1&1&0\end{array} \to \begin{array}{ccc} 1&1&0\end{array}$$

����������������԰������·�ʽ�۵����ü��� $0$ �� $4$ ����ͨ�飺
$$\begin{array}{cccc|ccc} 1&0&0&1&1&0&0\\0&1&1&0&0&1&1\\0&1&0&1&1&0&1\\0&0&1&0&0&1&0\\1&0&0&0&0&0&0\end{array} \to \begin{array}{cccc} 1&0&0&1\\0&1&1&0\\0&1&0&1\\0&0&1&0\\1&0&0&0\end{array}$$

```input1
3
2 5
11001
11001
5 7
1001100
0110011
0101101
0010010
1000000
3 2
11
11
11
```

```output1
1
4
0
```

## ��ʾ
For the first sample test case, you can fold in the following way and cut the only $0$ out:
$$\begin{array}{ccc|cc} 1&1&0&0&1\\1&1&0&0&1\end{array} \to \begin{array}{ccc} 1&1&0\\ \hline 1&1&0\end{array} \to \begin{array}{ccc} 1&1&0\end{array}$$

For the second sample test case, you can fold in the following way and cut the $4$ connected components of $0$s out:
$$\begin{array}{cccc|ccc} 1&0&0&1&1&0&0\\0&1&1&0&0&1&1\\0&1&0&1&1&0&1\\0&0&1&0&0&1&0\\1&0&0&0&0&0&0\end{array} \to \begin{array}{cccc} 1&0&0&1\\0&1&1&0\\0&1&0&1\\0&0&1&0\\1&0&0&0\end{array}$$

