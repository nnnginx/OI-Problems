## ��Ŀ����
Some major cities have subway systems in the form of a tree, i.e. between any pair of stations, there is one and only one way of going by subway. Moreover, most of these cities have a unique central station. Imagine you are a tourist in one of these cities and you want to explore all of the subway system. You start at the central station and pick a subway line at random and jump aboard the subway car. Every time you arrive at a station, you pick one of the subway lines you have not yet travelled on. If there is none left to explore at your current station, you take the subway line back on which you first came to the station, until you eventually have travelled along all of the lines twice,once for each direction. At that point you are back at the central station. Afterwards, all you remember of the order of your exploration is whether you went further away from the central station or back towards it at any given time, i.e. you could encode your tour as a binary string, where 0 encodes taking a subway line getting you one station further away from the central station, and 1 encodes getting you one station closer to the central station.

![](https://cdn.luogu.com.cn/upload/image_hosting/57sf9gvq.png)

## �����ʽ
On the first line of input is a single positive integer n, telling the number of test scenarios to follow.Each test scenario consists of two lines, each containing a string of the characters '0' and '1' of length at most 3000, both describing a correct exploration tour of a subway tree system.

## �����ʽ
exploration tours of the same subway tree system, or the text "different" if the two strings cannot be exploration tours of the same subway tree system.

## ��Ŀ����
**����Ŀ������**

һЩ��Ҫ���еĵ���ϵͳ������״�ṹ�������κ�������վ֮�䣬ֻ��һ���ҽ���һ��������·�����⣬�������Щ���ж���һ�����ص����복վ������һ�£�������Щ�����е�һ���οͣ�����Ҫ̽����������ϵͳ��������복վ���������ѡ��һ��������·�����ϵ����г���ÿ���㵽��һ����վ����ͻ�ѡ��һ������δ�������ĵ�����·������ڵ�ǰ��վû������Ҫ̽���ĵ�����·�ˣ���ͻ������һ�ε���ó�վ�ĵ�����·���أ�ֱ���������������е���·����ʻ�����Σ���ÿ��������ʻ��һ�Ρ�����ʱ����ص������복վ��֮�������ǵõ�̽��˳��ֻ�����κθ���ʱ���Ƿ������복վ��Զ�������Ҳ����˵������Խ�����ó̱���Ϊһ���������ַ��������� 0 ��ʾ����һ��������·ʹ�������복վ��Զһվ���� 1 ��ʾʹ�������복վ����һվ��

**�������ʽ��**

����ĵ�һ����һ�������� $n$����ʾ������Ҫ����Ĳ��Է�����������ÿ�����Է����������У�ÿ�а���һ���������Ϊ $3000$ �����ַ� '0' �� '1' ��ɵ��ַ����������˵�����ϵͳ����ȷ̽���ó̡�

**�������ʽ��**

����ÿ�����Է�������������ַ������Ա�ʾ��ͬ������ϵͳ��̽���ọ́������ "same"����������ַ������ܱ�ʾ��ͬ������ϵͳ��̽���ọ́������ "different"��

���������ڣ�ChatGPT��

```input1
2
0010011101001011
0100011011001011
0100101100100111
0011000111010101
```

```output1
same
different
```

