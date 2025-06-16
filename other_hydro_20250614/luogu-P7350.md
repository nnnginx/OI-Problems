## ��Ŀ����
Tommy �ļ���ϵͳ�������µ��ַ�����ϣ�㷨��

```cpp
int Hash(std::string s, int base, int mod) {
  int result = 0;
  for(int i=0; i<s.length(); i++)
    result = (1ll * result * base + s[i]) % mod;
  return result;
}
```

���� $\texttt{base}$ �� $\texttt{mod}$ �Ǹ������������� $257\le\texttt{base}\le\texttt{mod}\le10^9+9$������ $\texttt{mod}$ ��һ��������

���� Dream Ҫ�ƽ� Tommy �����ģ�����Ҫ�ҵ�һ���ʺϵĹ�ϣ��ײ������ $\texttt{base}$��$\texttt{mod}$����һ���ַ��� $S$������һ��һ�����ȵ��ַ��� $T$ ʹ�� $|S|=|T|$��$\texttt{hash(S)=hash(T)}$������ $S$ �� $T$ ������һ��λ�ò�ͬ��

����ж���Ϸ��� $T$���������һ�����ɡ�

## �����ʽ
��һ�У����������� $\texttt{base}$ �� $\texttt{mod}$��  
�ڶ��У�һ����Сд��ĸ��ɵ��ַ��� $S$��

## �����ʽ
һ�У�һ����Сд��ĸ��ɵ��ַ��� $T$����ʾ�𰸡�

```input1
257 997
aabdccbabdcdcadbcabcabaabdbbddbaabcadabcbcdacbbaac
```

```output1
lmzaeccihyailccmzzaxshssgbvjvhthllyofzudraatifnzxy
```

## ��ʾ
#### ���ݹ�ģ��Լ��

��� $S$ ��һ���ַ�����$|S|$ �����ĳ��ȡ� 

����ǰ $10\%$ �����ݣ�$\texttt{mod}=997$��  
����ǰ $40\%$ �����ݣ�$|S|=2\times10^5$ ���� $S$ �����  
���� $100\%$ �����ݣ�$50\le|S|\le2\times10^5$��$257\le\texttt{base}<\texttt{mod}\le10^9+9$��$\texttt{mod}$ ��һ��������

#### ˵��

[Minecraft OI Round 4](https://www.luogu.com.cn/contest/33344) D          
idea & solution��w33z8kqrqk8zzzx33 check��MatKave

