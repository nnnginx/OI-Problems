## ��Ŀ����
BBCode��Markdown�����ֳ��õĸ�ʽ���ԡ���ν��ʽ����ָ��������ĳЩ��վ��������������ʱ������ʹ�����������۽������Σ�ʹ���ֿ�������ɫ������ȸ�����ʽ��


## ��Ŀ����
#### PDF����Ŀ: http://pan.baidu.com/s/1i3mxk4t ��ȡ����hayc


BBCode���﷨������ʾ��

```cpp
[h1]Hello World![/h1]
[h2][i]This is a BBCode[/i][/h2]
[b][i]I love[/i] Olympic [i]Informatics[/i][/b]
```

���磬�ڱ�ǩ[h1]�У���[h1]��[/h1]֮���������������һ�����⣬������֮�������Ҫ����һ���������ʽ��Ⱦ��

��ע��BBCodeҪ���ǩ�Ŀ��ձ�����������Ƕ������Ҳ����˵�������е����Ӷ��ǲ��Ϸ���BBCode��


```cpp
[h1]Hello World! //��ǩδ�պ�
[h1]Hello World![/h2] //������ǩ��ƥ��
[h1][i]Hello World![/h1][/i] //Ƕ�״������
```

���⣬������Ҫ��һ���ǣ�BBCode��һ������ı�ǩ[quote][/quote]�������е��������ֶ���Ӧ������ΪBBCode���룬��Ӧ�ö������Markdown�������ԭ�������


���ڽ���Markdown�����﷨������ʾ��

```cpp
# Hello World! #
## *This is a Markdown* ##
__*I love* Olympic *Informatics*__
```

���������ǽ�������һ��BBCodeת����Markdown�����Բ��Ϸ������뱨��


��Ŀ�����л���ֵ�����BBCode�ı�ǩ�����ӦMarkdown��Ӧ��ϵ���£���֤�����ֳ���֮��Ķ�Ӧ��



 ![](https://cdn.luogu.com.cn/upload/pic/1493.png) 

����[quote]��ǩ�ĸ���˵����


![](https://cdn.luogu.com.cn/upload/pic/1494.png)


## �����ʽ
����ת����BBCode��


```input1
[h1]Hello World![/h1]
[h2]How are [i]you[/i]?[/h2]
```

```output1
# Hello World! #
## How are *you*? ##
```

```input2
[h1]Introducing Swift.[/h1][quote]
import SpriteKit
let object = SKSpriteNode(imageNamed: ��[L2/Ascention]��
[/quote]
```

```output2
# Introducing Swift. #
> import SpriteKit
> let object = SKSpriteNode(imageNamed: ��[L2/Ascention]��
```

```input3
[h1]I knew you were
trouble when you walked in[/h1]
[url=http://www.example.com]By Taylor Swift[/url]
```

```output3
# I knew you were
trouble when you walked in #
[By Taylor Swift](http://www.example.com)
```

```input4
[h1]Thanks for [i]inviting[/h1] me.[/i]
```

```output4
Match Error
```

```input5
[h2]Your gift is awesome!
```

```output5
Unclosed Mark
```

```input6
[quote][/quote][/quote]
```

```output6
Match Error
(�Ը����ݵĽ���: ƥ�䵽��һ���رձ�ǩ�󼴲���Ϊ������������Ǵ����)
```

```input7
[quote][quote][/quote]
```

```output7
> [quote]
```

## ��ʾ
Ϊ��֤����˳���������У���ע������Ҫ��

����ԭ��������Ļ��У���������ɾ��

���ڵ�һ���������ǣ� ����[quote]��ǩ�����µ�һ��ʱ��Markdown��������һ�С�����[quote]��ǩ�еĴ����ͷβ������ȥ����������ֿհ׵�quote��

��ע���ϱ��еĿո�

���ڲ��Ϸ���BBCode���룬��ĳ�����뱨������ƥ�����ı�ǩ���Match Error������δ�պϵı�ǩ���Unclosed Mark����ο��������������ͬʱ���ֵ�ʱ�򣨼�ͬʱ��ƥ������δ�պϵı�ǩʱ��������ƥ����������Match Error������quote��ǩ�������ԣ�Ϊ��֤���������壬���ݱ�֤quote��ǩ������ִ���(���ڳ�����[i][h1]Text[/i]���������������Match Error��������[i][h1]Text[/h1]���������������Unclosed Mark����)

����������ƣ����������Unclosed Mark��ʱ����close�м��п���Ϊ�����ַ������������ᱻ�̼�¼��

��֤���������ַ��������ڳ�quote��ǩ�����Ķ����е������У�[,],/,\*,\_,#,>������ַ�п��ܻ����/�ַ���

��֤���벻����ֱ�ǩ�����������������[h1]Text[/h

���������������ط�ʹ�ù�Markdown��BBCode��ͬѧ�����еĸ�ʽ�����ϸ��BBCode��Markdown��ʽ�����𱻾����Ի�


