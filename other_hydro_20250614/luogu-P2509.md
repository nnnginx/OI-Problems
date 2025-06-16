## ��Ŀ����
��һ���򵥵Ľű����ԣ�ֻ�и�ֵ��䡢�������ͷ���������֡������������ǵ�����д��ĸ���ұ������� $32$ λ������������

�����Ե�ÿ�������뵥��ռһ�С������в������У���ÿ�е�������ĩ���޿ո�ÿ�еĲ�ͬ token ֮���õ����ո�����������Ե� BNF ���£�

```cpp
<line> :: <head> | <assignment> | <if> | ELSE | END IF | <return>
<head> :: PARAM <paramlist> | PARAM
<assignment> :: <variable> = <rvalue>
<if> :: IF <variable> <relation> <value> THEN
<return> :: RETURN <value>
<paramlist> :: <variable> | <variable> <paramlist>
<rvalue> :: <value> | <value> <operator> <value>
<value> :: <variable> | <integer>
<operator> :: + | - | * | /
<relation> :: < | = | >
<variable> :: A | B | ... | Z
<integer> :: ����ǰ�� 0 �� 32 λ����������
```
����ĵ�һ����һ�� `<head>` ��䣬�����˺����Ĳ����������һ��һ���� `<return>` ��䡣`<head>` ��䲻���ڳ��˵�һ��֮��������κεط����֣��� `<return>` �������ڳ����ж�γ��֡��кŴ� $1$ ��ʼ��š�
ÿ�� `IF` ���һ����һ�����׵� `END IF` ��䣬����һ����ѡ�� `ELSE` ��䣨ע��û�� `ELSE IF` ��䣩��`IF` ������Ƕ�ף������ǱȽ�һ��������һ������������һ��������

��Ӧ�÷���һ�������ĳ��򣬲�������ྯ����Ϣ����ʽ�������������

- ��һ�ྯ�棺�޷�����Ĵ����С����ܸ��� `IF` ���Ĳ������ʽ���滹�Ǽ٣�����ÿ�� `IF` ���Ĳ������ʽ���Ǽȿ���Ϊ��Ҳ����Ϊ�٣��������� `IF` �����Ӱ�죩��

- �ڶ��ྯ�棺����δ��ʼ���ı�����������õ���ĳ��������ֵ������������Ȳ��ڵ�һ��ָ���Ĳ����б��Ҳû���ڴ�֮ǰ�ɸ�ֵ��丳ֵ���������������޷������ô��Ӧ�ø������ྯ�档

ע�⣬��� `ELSE` �� `END IF` ���ǿ�ִ����䣬��˲�Ӧ���յ��κξ�����Ϣ��


## �����ʽ
������ $50$ �У�����Ҫ����ĳ��򡣱�֤�ó���Ϸ���


## �����ʽ
���水���кŴ�С�����������ͬһ�����ж������δ��ʼ���ı�����������ĸ˳���С�������С����û���κξ�����Ϣ��������Ӧ��Ϊ�ա�

```input1
PARAM A B
IF A > 5 THEN
C = B * A
END IF
D = B - C
Z = Y + X
E = T
F = E + E
V = G + G
RETURN F
```

```output1
Line 5: variable C might not have been
initialized
Line 6: variable X might not have been
initialized
Line 6: variable Y might not have been
initialized
Line 7: variable T might not have been
initialized
Line 9: variable G might not have been
initialized
```

```input2
PARAM G
RETURN G
B = K
RETURN C
```

```output2
Line 3: unreachable code
Line 4: unreachable code
```

```input3
PARAM T C
B = T
A = 4
IF A < 4 THEN
IF B > 3 THEN
Q = 100 + F
ELSE
IF C = -1111111111 THEN
Q = T - A
IF Q = 0 THEN
V = V - 1
END IF
ELSE
RETURN I
E = A
END IF
END IF
ELSE
Q = 1
END IF
RETURN Q
```

```output3
Line 6: variable F might not have been
initialized
Line 11: variable V might not have
been initialized
Line 14: variable I might not have
been initialized
Line 15: unreachable code
```

