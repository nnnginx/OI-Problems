## ��Ŀ����
����һ�� [`std::freopen`](https://zh.cppreference.com/w/cpp/io/c/freopen) ��䣬�����������ļ����ơ�

��ʽ���أ�[`std::freopen`](https://zh.cppreference.com/w/cpp/io/c/freopen) ��䶼Ӧ��ǡ����

```cpp
std::freopen("<title>","<mode>",<stream>);
```

���� `<title>` Ϊ��������ļ����ơ������ٰ���һ���ַ�������ֻ���ܰ������м����ַ���
- ��дӢ���ַ���
- СдӢ���ַ���
- ���������֣�
- Ӣ�İ�Ǿ�� `.`��

`<mode>` Ϊ�ļ����ʱ�ǣ���ֻ����Ϊ `r`��`w`��`a` �е�һ�֡�`<stream>` Ϊ�ļ�������ֻ����Ϊ `stdin`��`stdout`��`stderr` �е�һ�֡�
	
����Ҫ�ش� $T$ ��ѯ�ʡ�

## �����ʽ
**���ⵥ�����Ե��ں��ж���ѯ�ʡ�**

��һ��һ�������� $T$������ѯ�ʴ�����

����ÿ��ѯ�ʣ�һ��һ���ַ���������һ�� [`std::freopen`](https://zh.cppreference.com/w/cpp/io/c/freopen) ��䡣

## �����ʽ
����ÿ��ѯ�ʣ����һ��һ���ַ�����������������ļ����ơ�

```input1
9
std::freopen("5k.sync.closer","r",stdin);
std::freopen("5k.sync.closer","r",stdout);
std::freopen("5k.sync.closer","r",stderr);
std::freopen("5k.sync.closer","w",stdin);
std::freopen("5k.sync.closer","w",stdout);
std::freopen("5k.sync.closer","w",stderr);
std::freopen("5k.sync.closer","a",stdin);
std::freopen("5k.sync.closer","a",stdout);
std::freopen("5k.sync.closer","a",stderr);

```

```output1
5k.sync.closer
5k.sync.closer
5k.sync.closer
5k.sync.closer
5k.sync.closer
5k.sync.closer
5k.sync.closer
5k.sync.closer
5k.sync.closer

```

## ��ʾ
**�������������ԡ�**

���� $100\%$ �����ݣ�

- $1 \le T \le 1000$��
- ÿ�����ĳ��Ⱦ������� $1000$��

���岿�ַַ������£�

- Subtask 1 (30pts)����֤�ļ���Ϊ `5k.sync.closer`��
- Subtask 2 (30pts)����֤�ļ�������Ϊ $1$��
- Subtask 3 (40pts)�����������ơ�

