## ��Ŀ����
[ҡҷ����](https://music.163.com/#/song?id=22699115)��

���ֺγ�����һ����������

## ��Ŀ����
�㲢����αα�����������Ҫ��һ�����⡣


```cpp
#include <bits/stdc++.h>
using namespace std;

int n;
unsigned int a[6],b[6];
char s[207];
signed main(){
	scanf("%s",s+1);
	n=strlen(s+1);
	a[1]=1;
	for(int _=1;_<=n;_++){
		char ch=s[_];
		for(int i=1;i<=5;i++) b[i]=0; 
		if(ch=='L'){
			b[2]+=a[1];
			b[2]+=a[3];
			b[4]+=a[5];
			b[2]+=a[4];
			b[4]+=a[2];
		}
		if(ch=='R'){
			b[1]+=a[2];
			b[3]+=a[1];
			b[3]+=a[5];
			b[4]+=a[2];
			b[4]+=a[3];
			b[5]+=a[2];
			b[5]+=a[4];
		}
		for(int i=1;i<=5;i++) a[i]=b[i];
	}
	printf("%u\n",a[1]);
	return 0;
}
```

������С D ��Ƶģ�׼�����㽻���ĳ���

��ΪС D �������ý����⣬�������㹹��һ������ʹ�øó�������ǡ��Ϊ $n$��

## �����ʽ
����һ�У�һ������ $n$��

## �����ʽ
���һ�У�һ���ַ�������ʾ�ṩ��С D �����롣

**�뱣֤���ַ����ǿգ�������ܳ�������֮��Ľ����**

���ַ������Ȳ��ܳ��� $200$�������޷�ͨ����Ӧ���Ե㡣

**��ֻ��Ҫ�������һ�������������ַ������ɻ�÷�����**

����޷���ʾ��ĳ������������һ�� `-1`��


```input1
3
```

```output1
RLRLLLRLLLLR
```

```input2
3
```

```output2
LLRLLRLLRLLR
```

```input3
11776
```

```output3
RLRLRLLLRLRRLRLRLRLRLRLRLRLRLRLR
```

```input4
16
```

```output4
LRLRLRLRRLLRLR
```

```input5
47
```

```output5
RLRRLLRLRRLLRLRLLRRRLRRRRLR
```

```input6
720
```

```output6
RLRRRLRRLRLRRRLRRLLLRLLLRLRLLLR
```

```input7
176374
```

```output7
RRLLRRLRRLLRLLRRLLRLLRRLRLRLRRLLRLLRLLLLRLRLLRLLRLLRLLRLRLLRLR
```

## ��ʾ
### ��������

�����ֱ�Ӱ��ַ����������������Ȿ��ĳ�����Ϲ��ģ�����һ��ʵ�����壬������Ϊ J ����ڸ��������޷���֪�㡣

### ���ݷ�Χ

���⹲ $20$ �����Ե㡣

����ǰ $20\%$ �������� $n\le 10$��

����ǰ $40\%$ �������� $n\le 10^5$��

����ǰ $60\%$ �����ݣ���֤�ڶ�Ӧ��Χ��������ɡ�

�����������ݣ���֤ $0 \le n\le 10^9$������ַ���������С D �ĳ�����Ȼ�����

