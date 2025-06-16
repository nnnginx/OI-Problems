## ��Ŀ����
ICPC2020 WF N

## ��Ŀ����
Vector embeddings are a common tool in machine learning systems.
Complex real-world concepts (for instance, words in a dictionary) are mapped onto vectors of real numbers.
If embeddings are trained properly, related concepts remain close together in the vector space, so questions like "are these two words synonyms?" can be reduced to straightforward mathematical tests.

You have been hired by Ye Olde Ice Cream Shoppe to create an embedding model for flavors, so that when they are out of an ice cream flavor they can recommend related flavors to customers.
After training your embedding on six cloud datacenters for four months, you finally had the perfect flavor model!
You were ready to revolutionize the ice cream industry on your street and, dare we say it, your neighborhood!
Well, until you accidentally dripped some free ice cream on your keyboard and deleted half the data.
The Shoppe cannot afford the 30 billion rubles needed to retrain the model, so you are in trouble.

Fortunately, you still have various training results lying around.
For a given deleted vector, the training data tells you how close it was to some known flavor vectors.
The closeness of vectors $A$ and $B$ is just the standard Euclidean distance metric (that is, the length of the vector $A - B$).
Write a tool that reconstructs embeddings which are consistent with the training results.

## �����ʽ
The first line contains two integers $d$ and $n$, where $d$ ($1 \leq d \leq 500$) is the number of dimensions of the
vectors, and $n$ ($1 \leq n \leq 500$) is the number of training results for a deleted embedding vector you want to reconstruct.
Each of the next $n$ lines describes a training result using $d + 1$ numbers $x_1, \dots, x_d$ and $e$.
In a training result, $x_1, \dots, x_d$ ($-100 \leq x_i \leq 100$) are the coordinates of a known vector, and 
$e$ ($0 \leq e \leq 5\,000$) is the Euclidean distance from that vector to the deleted one.

Your submission will be tested only with the sample inputs given below and inputs generated according to the following procedure.
First, $d$ and $n$ are chosen.
Then, $n$ input vectors and $1$ output vector, each with dimension $d$, are chosen at random.
The $d \cdot (n + 1)$ coordinates are independent and uniformly distributed in the interval $[-100,100]$.
Next, the Euclidean distance from each input vector to the output vector is computed.
Finally, the output vector is discarded.
Calculations use double-precision floating-point numbers.
Numbers obtained using this procedure appear in the input with $17$ digits after the decimal point.

## �����ʽ
Output $d$ values, the coordinates of any vector that has the given distance to each training vector with an absolute or relative error of at most $10^{-5}$.

## ��Ŀ����
**����Ŀ������**

����Ƕ���ǻ���ѧϰϵͳ�е�һ�ֳ��ù��ߡ���ʵ�����е�ĳЩ���ӵĸ������ʵ��еĵ��ʣ�ͨ�����ַ�������ӳ�䵽һ��ʵ�����ϡ�������û�����ȷ��ѵ������Ƕ�룬������ظ����������ռ��б����Ž��ܵ���ϵ�������������������ͬ����𣿡�����������Լ�Ϊ�򵥵���ѧ�����ˡ�

������� Ye Olde �����ר���ܹͣ�ר�Ÿ���Ϊ����ܿ�ζ����һ������Ƕ��ʽģ�ͣ�������һ�ֿ�ζ�ı���������Ժ����Ƕ��ʽģ�;Ϳ�����˿��Ƽ�����ζ������ı���ܡ�������������������ѵ�����ĸ����Ժ�������ӵ����һ��������ģ�ͣ���׼���øı������ڽ����ı������ҵ��������������ʱ���㲻С�İ�һЩ��ѵı���ܵε��˼����ϣ�����һ������ݱ�ɾ��������ѵ��ģ����Ҫ���� 300 ��¬������ר����Ȼ���ܲ�����ô�ߵļ۸�����������˾޴���鷳֮�С����˵��ǣ������ͨ��ʣ�µ���������ԭ����ɾ��������������أ�����һ�������ı�ɾ�������������ݻ����������ĳЩ��֪��ζ�������Ľӽ��̶ȡ��������� $A,B$ �Ľӽ��̶ȼ�Ϊ����������֮��ı�׼ŷ����þ��루������ $A-B$ �ĳ��ȣ���

���ڣ��������������Ŀռ�ά�� $d$ ����֪�������� $n$������������ $n$ ������������ $(x_{i,1},x_{i,2},\cdots,x_{i,d})$ �͵�ͬһ����ɾ���������ı�׼ŷ����þ��� $e_i$�������дһ�����������ɾ�������������ꡣ

**�������ʽ��**

��һ�������������� $d,n$���ֱ��ʾ�����ռ��ά�Ⱥ�����������  
��� $n$ �У�ÿ�� $d+1$ ��ʵ�� $x_{i,1},x_{i,2},\cdots,x_{i,d},e_i$������ǰ $d$ ��ʵ�������˵� $i$ �����������꣬�� $d+1$ ��ʵ�����ʾ�� $i$ �������뱻ɾ��������֮��ı�׼ŷ����þ��롣

���ύ�Ĵ���ֻ���������������ݺͰ����·�ʽ���ɵ����������Ͻ��в��ԣ�

- ������ $[1,500]$ ��ѡ������������Ϊ $d,n$��
- ������� $n$ �� $d$ ά����������һ�� $d$ ά����������� $d\cdot(n+1)$ ������������ $[-100,100]$ �ж����Ҿ��ȵ����ɡ�
- ����ÿ���������������������������֮��ı�׼ŷ����þ��롣
- �������������

���������������еļ���ʹ��˫���ȸ������������ַ�ʽ���ɵ�����ʵ����������С����� $17$ λ��

**�������ʽ��**

��� $d$ ��������������ɾ�����������ꡣ����Ҫ��֤������Ĵ𰸺ͱ�׼��֮������ᳬ�� $10^{-5}$��

**��������**

��������������������֡�

**�����ݷ�Χ��**

�����������ݣ�

- $1\leqslant d,n\leqslant 500$��
- $-100\leqslant x_{i,j}\leqslant 100$��
- $0\leqslant e_i\leqslant 5000$��

Translated by Eason_AC

```input1
2 3
0 0 2.5
3 0 2.5
1.5 0.5 2.5
```

```output1
1.5 -2
```

```input2
2 2
0 0 2
4 -4 6
```

```output2
1.414213562373 1.414213562373
```

```input3
4 3
0 1 2 3 2
1 2 -1 7 5
1 0.3 3.4 1.2 3.3
```

```output3
1 2 3 4
```

