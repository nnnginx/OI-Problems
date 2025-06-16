


## ��Ŀ����
The king of Byteotia, Byteasar, is returning to his country after a victorious battle. In Byteotia, there are n towns connected with only n-1 roads. It is known that every town can be reached from every other town by a unique route, consisting of one or more (direct) roads. (In other words, the road network forms a tree).
The king has just entered the capital. Therein a triumphal arch, i.e., a gate a victorious king rides through, has been erected. Byteasar, delighted by a warm welcome by his subjects, has planned a triumphal procession to visit all the towns of Byteotia, starting with the capital he is currently in.
The other towns are not ready to greet their king just yet - the constructions of the triumphal arches in those towns did not even begin! But Byteasar's trusted advisor is seeing to the issue. He desires to hire a number of construction crews. Every crew can construct a single arch each day, in any town. Unfortunately, no one knows the order in which the king will visit the towns. The only thing that is clear is that every day the king will travel from the city he is currently in to a neighboring one. The king may visit any town an arbitrary number of times (but as he is not vain, one arch in each town will suffice).
Byteasar's advisor has to pay each crew the same flat fee, regardless of how many arches this crew builds. Thus, while he needs to ensure that every town has an arch when it is visited by the king, he wants to hire as few crews as possible. Help him out by writing a program that will determine the minimum number of crews that allow a timely delivery of the arches.
Foreseeable�������ص����ý���ʦ�á��ĸ���������Ϸ
�á��ĸ��׻���һ���С������š�����Ϸ��
������һ��n���ڵ��������ʾһ������ 
1�ŵ����������ҵ��׶� �����Ϸ��������
һ���� һ����Ұ����Ӳ���ҵĹ�����
��һ�����ݽ��������ŵĽ���ʦ һ��ʼֻ���׶�
�п����� ����ÿ�λ�ӵ�ǰ���ڳ����ƶ���һ����
�ڵĳ��� �ڹ���ÿ���ƶ�ǰ������ʦ����ѡ�����
�����ⲻ����k�����н���������� ���������һ��
ʱ�̣��������ڵĳ���û�п����� ��ô�������������
���ݽ���ʦ����Ҿ����� ������еĳ��ж��������˿���
�Ŷ�����һֱû���ߵ��п����ŵĳ��У���ô����ʦ��ʤ����
Foreseeable���Ὠ�������������ݹ��� ���á��ĸ�����
�����ݡ�����ʦ�����������ǽ���ʦ����Ҫ���ݣ�  ���׷���k
�Ĵ�С�ǳ�Ӱ����Ϸ��Ȥ�ȡ��� ���k̫����ô����ʦ������
�����ж�ǰ�������г��н��������ţ���ô������û��ʤ����ϣ����
������Foreseeable���������� ���k̫С����ôForeseeable
���п��ܻᷢ���Լ���ʣ�޼��������ߵ�һ��û�п����ŵĵط�  
�á��ĸ���������ŰForeseeable�Ŀ�� ������Ҫ����ȷ
����С��k��ʹ���������Ϸ�У��������ʦ�㹻������
��������ʦ��ʤ  
Input ��һ��һ������n ������n-1�У�ÿ����������u,v����ʾu,v���� Output һ��һ��������ʾ��С��k 
Sample Input 
7 1 2 1 3 2 5 2 6 7 2 4 1
Sample Output
3 
Hint 1<=n<=300000 
�������ͣ���foreseeable��һ���ж�ǰ������2,3,4���н���
�����ţ�Ȼ�����������foreseeable�ߵ��ĸ����У�
��5,6,7���ÿ����ž��ܱ�֤�õ�ʤ����  

```
## �����ʽ
 **The first line of the standard input contains a single integer n (1<=N<=300000) , the number of towns in Byteotia. The towns are numbered from 1 to n, where the number 1 corresponds to the capital.
The road network is described in n-1 lines that then follow. Each of those lines contains two integers,a,b(1<=a,b<=N) , separated by a single space, indicating that towns a and b are directly connected with a two way road.
** 
## �����ʽ
 **The first and only line of the standard output is to hold a single integer, the minimum number of crews that Byteasar's advisor needs to hire.
** 

```input1
7
1 2
1 3
2 5
2 6
7 2
4 1
 
```

```output1
3
Explanation of the example: On the first day, triumphal arches need to be erected in towns 2, 3, 4. On the second day, they should be erected in towns 5, 6, 7.

```
## ��ʾ
û��д����ʾ
## ��Ŀ��Դ
��лWcmg�ṩ����
								
							
						
					
				
				
				
			
		
	
