## ��Ŀ����
Always known for being quite tech-savy, Farmer John is testing out his new automated drone-mounted cow locator camera, which supposedly can take a picture of his field and automatically figure out the location of cows. Unfortunately, the camera does not include a very good algorithm for finding cows, so FJ needs your help developing a better one.


The overhead image of his farm taken by the camera is described by an $N \times N$ grid of characters, each in the range $A \ldots Z$, representing one of 26 possible colors. Farmer John figures the best way to define a potential cow location (PCL) is as follows: A PCL is a rectangular sub-grid (possibly the entire image) with sides parallel to the image sides, not contained within any other PCL (so no smaller subset of a PCL is also a PCL).  Furthermore, a PCL must satisfy the following property: focusing on just the contents of the rectangle and ignoring the rest of the image, exactly two colors must be present, one forming a contiguous region and one forming two or more contiguous regions.



```cpp
AAAAA
ABABA
AAABB
```



For example, a rectangle with contents would constitute a PCL, since the A's form a single contiguous region and the B's form more than one contiguous region. The interpretation is a cow of color A with spots of color B. 

A region is "contiguous" if you can traverse the entire region by moving repeatedly from one cell in the region to another cell in the region taking steps up, down, left, or right. 

Given the image returned by FJ's camera, please count the number of PCLs.


## �����ʽ
The first line of input contains $N$, the size of the grid ($1 \leq N \leq 20$).

The next $N$ lines describe the image, each consisting of $N$ characters.


## �����ʽ
Print a count of the number of PCLs in the image.


## ��Ŀ����
## ��Ŀ����

Farmer John һֱ�Ծ�ͨ�����������������ڲ��������������˻����ص���ţ��λ�������������˵��������������ز��Զ�ȷ����ţ��λ�á����ҵ��ǣ�������㷨�����ó�Ѱ����ţ����� Farmer John ��Ҫ��İ���������һ�����õ��㷨��

��������ũ������ͼ��һ�� $N \times N$ ���ַ�����������ÿ���ַ��� $A \ldots Z$ ��Χ�ڣ����� 26 �ֿ��ܵ���ɫ֮һ��Farmer John ��Ϊ������Ǳ����ţλ�ã�PCL������ѷ�ʽ���£�һ�� PCL ��һ�����������񣨿���������ͼ�񣩣������ͼ��ı�ƽ�У����Ҳ��������κ����� PCL �У���� PCL �Ľ�С�Ӽ�����Ҳ�� PCL�������⣬PCL ���������������ԣ�����ע�����ڵ����ݲ�����ͼ������ಿ�֣�����ǡ�ô���������ɫ������һ����ɫ�γ�һ������������һ����ɫ�γ������������������

���磬һ�����ε��������£�

```
AAAAA  
ABABA  
AAABB  
```

�⽫����һ�� PCL����Ϊ A �γ�һ���������򣬶� B �γɶ���������򡣽���Ϊһֻ��ɫΪ A ����ţ������ɫΪ B �İߵ㡣

һ�������ǡ������ġ����������ͨ�����ϡ����¡�����������ƶ�����һ�������еĵ�Ԫ�񷴸��ƶ�����һ�������еĵ�Ԫ����������������

���� Farmer John ��������ص�ͼ������� PCL ��������

## �����ʽ

����ĵ�һ�а��� $N$����ʾ����Ĵ�С��$1 \leq N \leq 20$����

�������� $N$ ������ͼ��ÿ�а��� $N$ ���ַ���

## �����ʽ

���ͼ���� PCL ��������

## ˵��/��ʾ

����������У����� PCL �ֱ����������µľ��Σ�

```
ABB  
BBB  
AAB  
ABB
```

��

```
BC  
BC  
BB  
BC  
```

```input1
4
ABBC
BBBC
AABB
ABBC
```

```output1
2
```

## ��ʾ
In this example, the two PCLs are the rectangles with contents

```cpp
ABB
BBB
AAB
ABB
```


and

```
BC
BC
BB
BC
```

