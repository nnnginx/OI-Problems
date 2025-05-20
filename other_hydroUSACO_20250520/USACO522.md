## ����  
ũ��Լ���Ѿ�����������������Ѿ�������ũ��Χ��һЩ��ֵ���״�����ڱ����ҳ����ŵ�Դ�����λ�á�  
����ÿ�ε���������ӵ�Դ����һ�����ߡ����߿��Դ��������������߿���������ߡ������ܹ�������Ƕ����裬�ӵ�Դ���ӵ�һ�ε���������һ���ϣ�Ҳ���ǣ���ε����Ķ˵��ϻ�������֮�������һ���ϣ���������˵�ġ�һ�ε�����ָ���ǳ�һ���߶�״�ĵ���������������һ��ļ��ε����������ε�������һ����ôҲҪ�ֱ����Щ�����ṩ������  
��֪���е� F��1 <= F <= 150���ε�����λ�ã��������Ǻ�������ƽ�У����Ҷ˵����������������0 <= X,Y <= 100������ĳ���Ҫ�������ӵ�Դ��ÿ�ε�������ĵ��ߵ���С�ܳ��ȣ����е�Դ��������ꡣ  
��Դ��������������ũ��Լ����ũ���е��κ�һ��λ�ã�����һ����������  
## INPUT FORMAT  
��һ�а��� F ���������������� ����� F ��ÿ�а������� X��Y �ԣ���ʾ��ε����������˵㡣  
(ps:�������е����ǵ��������� 68 97 68 97����ò������Ŀ������������ע�� //from Error)��·�˼ף�ò�����������ˣ����ùܣ���������  
## OUTPUT FORMAT  
ֻ��һ�У����������������ÿ������1λС�����ٶ���ĵ��Ե���������ȷ�ض�С�������������롣  
���������ǣ���Դ�������� X ֵ�� ��Դ�������� Y ֵ���� ��Ҫ�ĵ��ߵ��ܳ��ȣ�Ҫ��С����  
## SAMPLE INPUT (file fence3.in)  
```  
3  
0 0 0 1  
2 0 2 1  
0 3 2 3  
```  
## SAMPLE OUTPUT (file fence3.out)  
```  
1.0 1.6 3.7  
```  
  
## Description  
Farmer John has decided to construct electric fences. He has fenced his fields into a number of bizarre shapes and now must find the optimal place to locate the electrical supply to each of the fences.  
A single wire must run from some point on each and every fence to the source of electricity. Wires can run through other fences or across other wires. Wires can run at any angle. Wires can run from any point on a fence (i.e., the ends or anywhere in between) to the electrical supply.  
Given the locations of all F (1 <= F <= 150) fences (fences are always parallel to a grid axis and run from one integer gridpoint to another, 0 <= X,Y <= 100), your program must calculate both the total length of wire required to connect every fence to the central source of electricity and also the optimal location for the electrical source.  
The optimal location for the electrical source might be anywhere in Farmer John's field, not necessarily on a grid point.  
## INPUT FORMAT  
The first line contains F, the number of fences.  
F subsequent lines each contain two X,Y pairs each of which denotes the endpoints of a fence.  
## SAMPLE INPUT (file fence3.in)  
```  
3  
0 0 0 1  
2 0 2 1  
0 3 2 3  
```  
## OUTPUT FORMAT  
On a single line, print three space-separated floating point numbers, each with a single decimal place. Presume that your computer's output library will round the number correctly.  
The three numbers are:  
the X value of the optimal location for the electricity,  
the Y value for the optimal location for the electricity, and  
the total (minimum) length of the wire required.  
## SAMPLE OUTPUT (file fence3.out)  
```  
1.0 1.6 3.7  
```  