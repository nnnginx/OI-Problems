## ��Ŀ����
![Something Comforting](https://mivik.gitee.io/image/nurture/something_comforting.png)

> Cause getting made you want more
>
> And hoping made you hurt more
>
> Someone tell me
>
> Something comforting

## ��Ŀ����
Porter Robinson ���������ʱ�������� Something Comforting ���׸裬Mivik ��������ʱ�������һ��������������ص��⡣�� Mivik �������ģ���Ϊ�������������������ˣ�

Mivik ��Ҫ�������һ�� **�Ϸ�** ���������У����� Mivik ����һ�ᣬд����������㷨��

```cpp
#include <algorithm>
#include <string>

std::string generate(int n) { // ����һ������Ϊ n * 2 ����������
	const int len = n * 2;
	bool arr[len]; // 0 ���������ţ�1 ����������
	for (int i = 0; i < n; ++i) arr[i] = 0;
	for (int i = n; i < len; ++i) arr[i] = 1;
	std::random_shuffle(arr, arr + len); // ��������������
	for (int i = 0, j, sum = 0; i < len; ) {
		sum += arr[i]? -1: 1;
		if (sum < 0) { // �����˲��Ϸ���λ��
			for (j = i + 1; j < len; ++j) {
				sum += arr[j]? -1: 1;
				if (sum == 0) break;
			}
			// ���� i �ǵ�һ�����Ϸ���λ�ã�j �� i �����һ���Ϸ���λ��
			// ( ( ) ) ) ) ( ( ( ) ( )
			//         i     j
			for (int k = i; k <= j; ++k)
				arr[k] ^= 1; // ���������ȫ����ת
			i = j + 1;
		} else ++i;
	}
	std::string ret;
	for (int i = 0; i < len; ++i)
		ret += arr[i]? ')': '(';
	return ret;
}
```

P.S. Ϊ�˸����������û������������飬[����](https://www.luogu.com.cn/paste/wof8zjn8) �ṩ�˶������ԶԸ��㷨��������

Mivik ʮ�ֿ��ģ���Ϊ����㷨�������ɺϷ����������С�����һ������ͷ�������㷨���ɵ��������в������ȣ�Ҳ����˵���� $n$ �̶�ʱ�����кϷ����������г��ֵĸ��ʲ������ȡ����磬Mivik ���ֵ� $n=3$ ʱ��`()()()` �����ɵĸ���ҪԶ���� `((()))`��

���� Mivik ������һ�� $n$ ��һ������Ϊ $2n$ �� **�Ϸ�** �������У����� `std::random_shuffle` ����������������˵��`shuffle`���ܹ���������ش���һ�����飬���������������������ͨ�����ĵ��㷨�����ɵĸ����Ƕ��١����� Mivik ��ϲ��С��������Ҫ���������ʶ� $998244353$ ȡģ�Ľ��������㲻֪����ν�һ��������������ȡģ�����Բο� [������ȡģ](https://www.luogu.com.cn/problem/P2613)��

## �����ʽ
��һ��һ������ $n$������ͬ���档

����������һ������Ϊ $2n$ �ĺϷ��������У�����ͬ���档

## �����ʽ
���һ��һ������������������ʶ� $998244353$ ȡģ�Ľ����

```input1
1
()
```

```output1
1
```

```input2
3
()(())
```

```output2
598946612
```

## ��ʾ

### ��������

����һ��$n$ Ϊ 1 ʱ������������ֻ���ܻ����� `()` ��һ�ֺϷ����������У���˸���Ϊ 1��

### ���ݷ�Χ

����ȫ�����ݣ��� $1\le n\le 5\cdot 10^5$����������������кϷ���

Subtask 1��20 pts������֤ $1\le n\le 5$��

Subtask 2��30 pts������֤ $1\le n\le 1000$��

Subtask 3��50 pts�������������ơ�


