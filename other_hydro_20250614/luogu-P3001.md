## ��Ŀ����
Bessie is studying her favorite subject, Macroeconomics, in cowllege. For her final project, she will be presenting research on exchange rates between countries around the world.


In order to make her presentation more lively, she would like to show the relative prices of Big Macs around the world, despite their rather unsavory contents. To illustrate, suppose that Bessie would like to find smallest value of a Big Mac in a country given its value in some initial country and exchange rates from which other country's values can be calculated (as illustrated below):




```cpp
* A Big Mac is worth 60 dollars in the United States 
* The exchange rate from US dollars to Canadian dollars is 0.2 Canadian dollars per US dollar 
* The exchange rate from US dollars to British Pounds is 5.00 British Pounds per US Dollar 
* The exchange rate from British Pounds to Canadian dollars is 0.5 Canadian dollars per British Pound 
* The exchange rate between Canadian dollars to US dollars is 5.00 US dollars per Canadian dollar and Bessie would like to find the smallest possible value of a Big Mac in Canada that can be obtained by exchanging currencies. There are two ways: 
* Going from US dollars directly to Canada dollars would yield a burger worth 60.00 US dollars * 0.2 Canadian dollars / US dollar = 12.00 Canadian dollars 
* Going from US dollars to British Pounds to Canadian dollars would yield a burger worth 60.00 US$ * 5.00 GBP / 1 US$ * 0.5 C$ / 1 GBP = 150.00 C$ (Canadian dollars). 
```
Bessie would choose the former option, since she would much rather pay 12.00 Canadian dollars instead of 150.00 Canadian dollars for a Big Mac in Canada. 

Bessie has N (1 <= N <= 2,000) countries conveniently labeled 1 to N that she would like to consider along with a list of M (1 <= M <= 25,000) exchange rates e_ij (0.1 < e_ij <= 10), each between countries i and j (1 <= i <= N; 1 <= j <= N). 

Given the value V (1 <= V <= 1,000,000,000,000), which is not necessarily an integer, of the Big Mac in her starting country A (1 <= A <= N), help her find the smallest possible value of a Big Mac in country B (1 <= B <= N; B != A) after a series of currency conversions. If there is no minimum, output 0. 

It is guaranteed that the answer is, if not 0, between 1 and 10^15.

It is also guaranteed that, for any country's currency, it is possible to get to any other country's currency.





## �����ʽ
Line 1: Five space-separated numbers: N, M, V, A, B

Lines 2..M+1: Three space-separated numbers: i, j, e\_ij


## �����ʽ
Line 1: A single positive number, the price of the Big Mac, with absolute or relative error at most 10^-6. If there is no minimum, output 0.

## ��Ŀ����
### ��Ŀ����

Bessie ����ѧϰ����ϲ���Ŀ�Ŀ��۾���ѧ����Ϊ�����һ��ѧ�ƣ�������������ֻ��ҵĻ��ʽ����о���

Ϊ���������ݽ���������������չʾһ������ BM ����Ʒ��ȫ�������Լ۸񡣾ٸ����ӣ�Bessie ��ͨ���������ҵĻ���ȥ�ҵ�һ�� BM ��һ�����ҵ���С��ֵ��

- һ�� BM ������ֵ $60$ ��Ԫ��
- ��Ԫ����ô�Ԫ�Ļ���Ϊ $1$ ��Ԫ�� $0.2$ ���ô�Ԫ��$1:0.2$����
- ��Ԫ��Ӣ���Ļ���Ϊ $1$ ��Ԫ�� $5$ Ӣ����$1:5$����
- Ӣ������ô�Ԫ�Ļ���Ϊ $1$ Ӣ���� $0.5$ ���ô�Ԫ��$1:0.5$����
- ���ô�Ԫ����Ԫ�Ļ����� $5$ ��Ԫ��һ���ô�Ԫ��$5:1$����Bessie �����ַ���ͨ�����Ҷһ��ڼ��ô���������ҵ�һ�� BM ����ͼ�ֵ��

1. ������Ԫֱ��ȥ���ô�ͨ�����ʵó�һ�� BM ֻҪ $12$ ���ô�Ԫ��
2. ������ԪȥӢ�����һ�ΪӢ������ȥ���ô󣬵ó�һ�� BM Ҫ $150$ ���ô�Ԫ��

Bessie ��ѡ��ǰһ�ַ�����Ϊ��������Ϊ�ڼ��ô���һ�� BM ֧�� $12$ ��Ԫ������ $150$ ��Ԫ��

Bessie �� $N(1\leq N\leq 2000)$ �����ҵ���Ϣ�� $M(1\leq M\leq25000)$ �ֻ��ʣ��� $i,j$ ����Ļ��ʱ�ʾΪ $e_{ij}(0.1\leq e_{ij}\leq 10)$��

����һ��ֵ $V(1\leq V\leq 10^{12})$��$V$ ��һ����һ��������$V$ �� BM ����ʼ���� A �ļ۸񣬰��� Bessie Ѱ�ҵ��� B �� BM ��͵ļ۸���������ڣ������ $0$��

�ݱ�֤��С�� $10^{15}$��Ҳ��֤���й��Ҷ�����ͨ�����ʽ�Ǯ��תΪ��Ĺ��ҵġ�

### �����ʽ

�� $1$ �У��������$N,M,V,A,B$���ֱ�һ���ո������

�� $2$ �� $M+1$ �У������� $i,j,e_{ij}$���ֱ�һ���ո������

### �����ʽ

һ�У�BM �� B ������ͼ۸񣬾�ȷ�� $10^{-6}$�����û����Сֵ����� $0$��

**ע�⣬����Ļ����ǵ����**��

��л @JJYZ\_cbh �����ķ���


```input1
3 4 60 1 2 
1 2 0.2 
1 3 5 
3 2 0.5 
2 1 5 

```

```output1
12.00 

```

