## ��Ŀ����
Farmer John ӵ��һ�����������ļ��徭Ӫ��ũ�������е���ţ�ĸ�Դͬ��Ҳ���������ũ����׷��������ͨ���������ϵļ�¼��Farmer John ���������ڵ���Ⱥ��ţ����֮����ʲô��ϵ���������� 

## �����ʽ
����ĵ�һ�а��� $N$��$1\le N\le 100$����֮������ͷ��ţ�����֡�ÿͷ��ţ�����ֶ��������� $10$ ����д��ĸ��`A-Z`����ɵ��ַ�����Farmer John ��������������������ͷ��ţ֮��Ĺ�ϵ��

�������� $N$ �У�ÿ�а�����ͷ��ţ������ $X$ �� $Y$����ʾ $X$ �� $Y$ ��ĸ�ס� 

## �����ʽ
�������һ�У���ʾ�����һ��ָ������ͷ��ţ֮��Ĺ�ϵ���������������������У�������ͷ��ţ��Ϊ BESSIE �� ELSIE���������ǿ��ܳ��ֵĲ�ͬ����Ĺ�ϵ��

- ���BESSIE��ELSIE��ĸ����ͬһͷ��ţ����� `SIBLINGS`��
- BESSIE ������ ELSIE ��ֱϵ�����Ҳ����˵ ELSIE ��BESSIE ��ĸ�ף�`mother`��������ĸ��`grand-mother`������������ĸ��`great-grand-mother`����������������ĸ��`great-great-grand-mother`�����ȵȡ������������������ `ELSIE is the (relation) of BESSIE`������ `(relation)` ���ʵ��Ĺ�ϵ������ `great-great-grand-mother`��
- ��� ELSIE ���� BESSIE ��ĳ�����Ȼ���ã������� BESSIE ��ĳ�����ȵĺ��ӣ���ô ELSIE ���� BESSIE ����ĸ��`aunt`����������ע��Ӣ��ԭ��������������󣬹���������������������� ELSIE �� BESSIE ������ĸ�ĺ��ӣ���� `ELSIE is the aunt of BESSIE`����� ELSIE �� BESSIE ����������ĸ�ĺ��ӣ���� `ELSIE is the great-aunt of BESSIE`����� ELSIE �� BESSIE ��������������ĸ�ĺ��ӣ���� `ELSIE is the great-great-aunt of BESSIE`���Դ����ơ�
- ��� BESSIE �� ELSIE ���κ����������ݹ�ϵ��Ҳ����˵�������й�ͬ�����ȣ������Ǿ��Ǳ���ã���� `COUSINS`��
- ��� BESSIE �� ELSIE ��û�й�ͬ�����ȣ������κ�һͷҲ������һͷ��ֱϵ�������� `NOT RELATED`��

��ͼ������������ϵ����ֻ�迼����Щ��ϵ���۲쵽��һЩ���ǡ���Ů��`niece`��������õ�Ů�����Ĺ�ϵ�ǲ���Ҫ�ģ������������ BESSIE �� ELSIE ����Ů����ô ELSIE ���� BESSIE ����ĸ��

![](https://cdn.luogu.com.cn/upload/image_hosting/xvfjp4u5.png)

```input1
7 AA BB
MOTHER AA
GGMOTHER BB
MOTHER SISTER
GMOTHER MOTHER
GMOTHER AUNT
AUNT COUSIN
GGMOTHER GMOTHER
```

```output1
BB is the great-aunt of AA
```

