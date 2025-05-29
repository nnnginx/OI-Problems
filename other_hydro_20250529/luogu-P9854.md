## ��Ŀ����
The Body Mass Index (BMI) is one of the calculations used by doctors to assess an adult��s health. The doctor measures the patient��s height (in metres) and weight (in kilograms), then calculates the BMI using the formula:

$$\text{BMI} = \dfrac{\text{weight}}{\text{height} \times \text{height}}$$

Write a program which prompts for the patient��s height and weight, calculates the BMI, and displays the corresponding message from the table below.

| BMI Category | Message |
| :----------: | :----------: |
| More than $25$ | Overweight |
| Between $18.5$ and $25.0$ (inclusive)  | Normal weight |
| Less than $18.5$ | Underweight |

## �����ʽ
On the first line, enter your weight, and on the second line, enter your height (in meters).

## �����ʽ
Output the information corresponding to the BMI value obtained.

## ��Ŀ����
�������������� $weight(1.0 \leq weight \leq 100.0)$ �� $height(1.0 \leq height \leq 2.0)$�������æ�ж��� BMI ֵ����Ӧ����Ϣ��

| BMI ��Χ | ��Ӧ��Ϣ |
| :----------: | :----------: |
| ���� $25$ | Overweight |
| ���� $18.5$ �� $25.0$ ֮��  | Normal weight |
| С�� $18.5$ | Underweight |

BMI ���㹫ʽ��

$$\text{BMI} = \dfrac{\text{weight}}{\text{height} \times \text{height}}$$

```input1
69
1.73
```

```output1
Normal weight
```

```input2
84.5
1.8
```

```output2
Overweight
```

## ��ʾ
**Explanation for Output in Sample Input 1**:

The BMI is $69 \div (1.73 \times 1.73)$, which is approximately $23.0545$. According to the table, this is a "Normal weight".

**Explanation for Output in Sample Input 2**:

The BMI is $84.5 \div (1.8 \times 1.8)$, which is approximately $26.0802$. According to the table, this is "Overweight".

