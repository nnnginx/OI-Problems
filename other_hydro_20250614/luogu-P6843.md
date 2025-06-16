## ��Ŀ����
һ���ļ� $\tt file$ ����Ҫ��һ�������ܶ��ļ� $\tt dir1,dir2,\cdots,dirj$ ��Ŀ¼�У�����ļ��� absolute file path Ϊ $\tt/dir1/dir2/\cdots/dirj/file$����Ŀ¼�� $\tt /$ ��ʾ��ÿһ�����ڸ�Ŀ¼�µ��ļ��� absolute file path ����ʽΪ $\tt /file$��

��������ָ��һ���ѱ�������Ŀ¼�����Կ���һ����ݷ�ʽ�������Է���������Ŀ¼�£�ע�⣬�������Ӳ���ָ���ļ������磬������ $\tt /$ �·�һ��ָ�� $\tt /$ �ķ������� $\tt hello$����ô��$\tt /dir/file$��$\tt /hello/dir/file$��$\tt /hello/hello/dir/dile$ ��ָ��ͬһ���ļ� $\tt file$������磬������ $\tt /dir$ �·�һ��ָ�� $\tt /$ �ķ������� $\tt hi$����ô��$\tt /dir/file$��$\tt /dir/hi/dir/file$��$\tt /dir/hi/dir/hi/dir/file$ ��ָ��ͬһ���ļ� $\tt file$����������ָ����һ�㣬��һ�㣬����ͬ�㶼���ԣ����ǲ����� $\tt ./$��$\tt ../$��$\tt //$ ֮��Ĳ�����

�������ʣ��Ƿ���ͨ������һ����Ϊ $s$ �ķ�������ʹ���ҵ�һ���ļ��� absolute file path ����ǡ��Ϊ $k$��

## �����ʽ
��һ���������� $n,m,k$ �������Ŀ¼֮���Ŀ¼�����ļ�����Ҫ����ڵ�·�����ȡ�        
�ڶ���һ������ $s$ ����������ӳ���       
������ $n$ ��ÿ���������� $p_i,l_i$ ����һ��Ŀ¼�����Ŀ¼���Ϊ $l_i$����Ŀ¼���Ϊ $p_i$��        
������ $m$ ��ÿ���������� $p_j,l_j$������һ���ļ�������ļ��ĳ���Ϊ $l_j$����Ŀ¼���Ϊ $p_j$��

## �����ʽ
$m$ ��ÿ��һ���ַ��������Ƿ���ͨ������һ����Ϊ $s$ �ķ�������ʹ���ҵ����Ϊ $j$ ���ļ��� absolute file path ����ǡ��Ϊ $k$������ǵĻ���� $\tt YES$��������� $\tt NO$��

```input1
2 4 22
2
0 1
1 5
2 13
2 10
1 4
0 7
```

```output1
YES
YES
YES
NO
```

## ��ʾ
#### ���� 1 ����

���������������Ϊ $\tt LL$��Ŀ¼����Ϊ $\tt a$��$\tt bbbbb$���ļ�����Ϊ $\tt ccccccccccccc$��$\tt dddddddddd$��$\tt eee$��$\tt fffffff$����Ŀ¼�°���Ŀ¼ $\tt a$ ���ļ� $\tt fffffff$��Ŀ¼ $\tt a$ �°���Ŀ¼ $\tt bbbbb$ ���ļ� $\tt eee$��Ŀ¼ $\tt bbbbb$ �����ļ� $\tt ccccccccccccc$ �� $\tt dddddddddd$�����������󻯵ı�����

```plain
/
|-- a
| |-- bbbbb
| | |-- ccccccccccccc
| | +-- dddddddddd
| +-- eeee
+-- fffffff
```

- ���ڵ� $1$ ���ļ�������������·��Ϊ $\tt /a/bbbbb/ccccccccccccc$��
- ���ڵ� $2$ ���ļ�������������·��Ϊ $\tt /a/LL/bbbbb/dddddddddd$��
- ���ڵ� $3$ ���ļ�������������·��Ϊ $\tt /a/LL/a/LL/a/LL/a/eeee$��
- ���ڵ� $4$ ���ļ���������������·����

#### ���ݹ�ģ��Լ��

**�������������ԡ�**

- Subtask 1��33 pts����$n,m \le 500$��
- Subtask 2��33 pts����$n,m \le 3 \times 10^3$������������౻����һ�Ρ�
- Subtask 3��34 pts�������������ơ�

���� $100\%$ �����ݣ�$1 \le k,s \le 10^6$��$1\le m,n\le 3\times 10^3$��

#### ˵��

������ [BalticOI 2015 Day2 A File Paths](https://boi.cses.fi/files/boi2015_day2.pdf)��

