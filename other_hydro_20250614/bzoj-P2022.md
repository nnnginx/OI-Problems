## ��Ŀ����

Gigel has a strange "balance" and he wants to poise it. Actually, the device is different from any other ordinary balance. It orders two arms of negligible weight and each arm's length is $15$. Some hooks are attached to these arms and Gigel wants to hang up some weights from his collection of G weights, knowing that these weights have distinct values in the range $1 \ldots 25$. Gigel may droop any weight of any hook but he is forced to use all the weights. Finally, Gigel managed to balance the device using the experience he gained at the National Olympiad in Informatics. Now he would like to know in how many ways the device can be balanced. Knowing the repartition of the hooks and the set of the weights write a program that calculates the number of possibilities to balance the device. It is guaranteed that will exist at least one solution for each test case at the evaluation.

����һ����ƽ���ɹҹ���λ�ã�����������ҵ���ƽ�ϣ����ж�����ʹ��ƽ��ƽ��ķ�����

## �����ʽ

The input has the following structure:

- the first line contains the number $c$ and the number $g$;
- the next line contains $c$ integer numbers (these numbers are also distinct and sorted in ascending order) in the range $[-15\ldots15]$ representing the repartition of the hooks; each number represents the position relative to the center of the balance on the $x$ axis (when no weights are attached the device is balanced and lined up to the $x$ axis; the absolute value of the distances represents the distance between the hook and the balance center and the sign of the numbers determines the arm of the balance to which the hook is attached: `-` for the left arm and `+` for the right arm);
- on the next line there are $g$ natural, distinct and sorted in ascending order numbers in the range $[1\ldots25]$ representing the weights'values.

## �����ʽ

The output contains the number $m$ representing the number of possibilities to poise the balance.

```input1
2 4
-2 3
3 4 5 8
```
```output1
2
```

## ����˵�� 1

��һ�ַŷ��� $(4,8)$ ����ߣ�$(3,5)$ ���ұߡ�

�ڶ��ַŷ��� $(3,4,5)$ ����ߣ�$8$ �������ұߡ�

## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ�$2 \leq c \leq 20$��$2 \leq g \leq 20$��