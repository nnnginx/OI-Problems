## ��Ŀ����
When moving, ants form rows so that each ant except the first is behind another ant. It is not widely known what happens when two rows of ants moving in opposite directions run into each other in a passage too narrow for both rows to pass through. One theory says that, in that situation, ants will jump over each other.
From the moment the rows meet, each second every ant jumps over (or gets jumped over, as they agree upon) the ant in front of himself so that the two ants swap places, but only if the other ant is moving in the opposite direction. Find the order of the ants after T seconds.

## �����ʽ
The first line contains two integers N1 and N2, the numbers of ants in the first and second rows, respectively.
The next two rows contain the orders of ants in the first and second row (first to last). Each ant is uniquely determined by an uppercase letter of the English alphabet (this letter is unique between both rows).
The last line of input contains the integer T (0 �� T �� 50).

## �����ʽ
Output the order of the ants after T seconds on a single line. Our viewpoint is such that the first row of ants comes from our left side and the other one from our right side.

## ��Ŀ����
�������ƶ�ʱ�������ų�һ�У�ÿ�����ϳ��˵�һ�����϶�����һ�����Ϻ��档������֪���������������෴�ķ������ƶ�ʱ����һ��̫խ��ͨ���У����Ŷ�����ͨ����һ��������Ϊ������������£����ϻ������Է���ÿ��һ��ʱ�䣬ÿһ�����϶���������������ȥ����������ͬ���һ�����������Լ�ǰ�棬�����������Ͻ���λ�ã�����ֻ�е���һֻ���ϳ��෴�ķ����ƶ�ʱ����T����ҵ����ϵ�˳��
�����ʽ:
��һ�а�����������N1��N2���ֱ��ڵ�һ�к͵ڶ����е����ϵ������������������а�����һ�к͵ڶ����е�����˳�򣨵�һ�����һ�У���ÿһ�����϶�����һ����д��ĸ��Ӣ����ĸ��Ψһ�����ģ���������ĸ������֮����Ψһ�ģ�����������һ�а�������T(TС��50����
�����ʽ:
��һ���������T������ϵ�˳�����ǵĹ۵��ǣ���һ�������������ǵ���࣬��һ���������ǵ��Ҳࡣ

��л@��֮���� �ṩ�ķ���

```input1
3 3
ABC
DEF
0
```

```output1
CBADEF
```

```input2
3 3
ABC
DEF
2
```

```output2
CDBEAF
```

```input3
3 4
JLA
CRUO
3
```

```output3
CARLUJO
```

