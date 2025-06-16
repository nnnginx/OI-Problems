## ��Ŀ����
Recently, BaoBao has learned the Shortest Path Fast Algorithm (SPFA, or more formally, Bellman-Ford-Moore Algorithm) to solve the shortest path problem efficiently. He realizes that the algorithm looks so similar to the Dijkstra's algorithm after replacing the FIFO queue with priority queue, and shows you the below pseudo code.

![](https://cdn.luogu.com.cn/upload/image_hosting/yunmac9g.png)

By picking the best vertex from $Q$ we mean picking the vertex with the smallest priority value (in case that multiple vertices have the smallest priority value, pick the vertex with the largest index among them).

You, the future computer scientist, find the BaoBao-modified SPFA algorithm works so slow in some carefully construted graph. However, BaoBao is sure that his algorithm works well, unless you show him a simple undirected graph that makes the variable $\tt{cnt}$ in the SPFA function no less than a certain $k$ $\textbf{at some time}$. For convenience, the source vertex of the SPFA function is specified to be vertex $1$.

Just teach him a lesson!

## �����ʽ
There is only one test case in each test file.

The first and only line of the input contains a single integer $k$ where $k = 1$ for the sample test case and $k = 10^5$ for the only secret test case.

## �����ʽ
Output several lines in the following format to describe the input data of a simple undirected graph that makes the variable $\tt{cnt}$ in the SPFA function no less than $k$ $\textbf{at some time}$.

The first line contains two integers $n$ ($1 \le n \le 100$) and $m$ ($0 \le m \le 10^3$), indicating the number of vertices and edges in the graph.

Then $m$ lines follow, the $i$-th of which contains three integers $u_i$, $v_i$ ($1 \le u_i, v_i \le n$) and $w_i$ ($1 \le w_i \le 10^6$), indicating that the $i$-th edge in the graph has a weight of $w_i$ and connects the $u_i$-th and the $v_i$-th vertices.

Note that a simple graph contains no self-loops and no multiple edges.

## ��Ŀ����
**����Ŀ������**

���������ѧϰ�����·�������㷨��SPFA�������ʽ��˵��������-����-Ħ���㷨������Ч�ؽ�����·�����⡣����ʶ������������ȶ��д����Ƚ��ȳ����У����㷨�������� Dijkstra �㷨�ǳ����ƣ�������չʾ�������α���롣

![](https://cdn.luogu.com.cn/upload/image_hosting/yunmac9g.png)

ѡ�� $Q$ ����Ѷ�����ζ��ѡ�������С���ȼ�ֵ�Ķ��㣨����ж�����������С���ȼ�ֵ����ѡ�������������Ķ��㣩��

��Ϊδ���ļ������ѧ�ң��㷢�ֱ����޸ĺ�� SPFA �㷨��ĳЩ���Ĺ����ͼ�������ٶȷǳ�����Ȼ��������ȷ�������㷨�ܺã�����������չʾһ���򵥵�����ͼ���ڸ�ͼ�У�SPFA �����еı��� $\tt{cnt}$ ��ĳ��ʱ�̲�����ĳ�� $k$��Ϊ���������SPFA ������Դ���㱻ָ��Ϊ���� $1$��

�͸�������ѵ�ɣ�

**�������ʽ��**

ÿ�������ļ���ֻ��һ������������

����ĵ�һ�а���һ������ $k$������ $k = 1$ Ϊʾ������������$k = 10^5$ ΪΨһ�����ܲ���������

**�������ʽ��**

������������¸�ʽ����������ͼ���������ݣ�ʹ�� SPFA �����еı��� $\tt{cnt}$ ��ĳ��ʱ�̲����� $k$��

��һ�а����������� $n$��$1 \le n \le 100$���� $m$��$0 \le m \le 10^3$������ʾͼ�еĶ������ͱ�����

Ȼ�󣬸��� $m$ �У��� $i$ �а����������� $u_i$��$v_i$��$1 \le u_i, v_i \le n$���� $w_i$��$1 \le w_i \le 10^6$������ʾͼ�еĵ� $i$ ���ߵ�Ȩ��Ϊ $w_i$�������˵� $u_i$ ���͵� $v_i$ �����㡣

ע�⣬��ͼ�������Ի����رߡ�

**����ʾ˵����**

Ϊ�������������Դӱ�����վ�ϸ��������α�����Ӧ�� $\tt{C++}$ ���롣�����뱣��Ϊ $\tt{spfa.cpp}$��ʹ�� $\text{g++ spfa.cpp -O2 -o spfa}$ ���б��룬�㽫�õ�һ����Ϊ $\tt{spfa}$ �Ŀ�ִ���ļ������� $\tt{spfa}$�����������ṩ�����ı�׼���룬������ӡ�� $\tt{cnt}$ �� $\textbf{����}$ ֵ������ʾ�������������ӡ�� $4$������ζ��ʾ�����������ͨ�����ܲ���������

ע�⣬�����Ĵ��벻��������������Ч�ԣ����磬���������������Ƿ������һ����ͼ������ʹ��ִ���ļ���ӡ��һ���ܴ��ֵ�������������Ч������Ȼ����ʧ�ܲ��ԡ�

���������ڣ�[ChatGPT](https://chatgpt.com/)��

```input1
1
```

```output1
4 6
1 2 1
2 3 2
3 4 3
4 1 4
1 3 5
2 4 6
```

## ��ʾ
For your convenience, you can copy the $\tt{C++}$ code, which corresponds to the given pseudo code, from the contest website. Save the code as $\tt{spfa.cpp}$, use $\text{g++ spfa.cpp -O2 -o spfa}$ to compile it and you will get an executable file named $\tt{spfa}$. Run $\tt{spfa}$, feed your output to its standard input and it will print out the $\textbf{final}$ value of $\tt{cnt}$. Given the sample output it will print out $4$, which means the sample output is not sufficient to pass the secret test case.

Note that the given code does not check the validity of your output (for example it does not check if your output is really a simple graph). You might still fail the test if your output is invalid, even if the executable prints out a large value.

