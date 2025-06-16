## ��Ŀ����


Abstract Communication Mastership (ACM) is a software company that develops a unique social network called tWinter.

Each tWinter user has a handle that starts with a commercial at $(��@')$ character. Users of tWinter social network publish short messages to the network.

If a user's message contains another user's handle (preceded by a space or at the beginning of the message, and followed by a space or at the end of the message) then it is called a mention.

A sequence of messages is called a conversation if each message in the sequence (except the first one) contains a mention of the author of the previous message in the sequence.

You are hired to find the longest conversation in the given chronological log of messages.



## �����ʽ


The first line of the input file contains an integer $n (1 \le n \le 50 000)$ -- the number of messages in the chronological log.

Each of the next $n$ lines contains a message preceded by its author's handle, a colon $(��:')$ character, and a space.

Each message is at most $139$ characters long. Each handle is at most $20$ characters long and does not contain colons or spaces.

The input file contains only characters with ASCII codes between $32$ and $126$ , inclusive, and line breaks.



## �����ʽ


On the first line of the output file write the length of the longest conversation in the given log. On the second line write $1-based$ indices of the messages in that conversation in ascending order.

If there are multiple longest conversations, write any one of them.



## ��Ŀ����
Abstract Communication Mastership (ACM)��һ�������˾������һ����Ϊ$��tWinter��$�Ķ����罻���硣

ÿ��$��tWinter��$�û�����һ������������$��(��$��$������$��$��@��$��$���䡯$�� $��)��$��ͷ��

ÿ��$��tWinter��$�罻������û����������緢������Ϣ��

����û�����Ϣ������һ���û��ľ�������ǰ���ǿո��������Ϣ�Ŀ�ͷ���Һ���ո����Ϣĩβ�������Ϊ�ἰ��

�����Ϣ�����е�ÿ����Ϣ����һ����Ϣ���⣩���ἰ������ǰһ����Ϣ�����ߣ������Ϣ���г�Ϊ�Ự��

����Ҫ�ڸ�������Ϣʱ��˳����־�в�����ĶԻ���

## �����ʽ
�����ļ���$n+1$�У�

��һ�а���һ������$n(1��n��50000)$Ϊ��Ϣ��־����Ϣ������

������$n$��ÿ��һ����Ϣ��ǰ���������ߵľ�����������һ��ð�ţ�ð�ź�Ϊ��Ϣ���ġ�

ÿ����Ϣ�������Ϊ$139$���ַ���ÿ���ֱ�����(������ð�Ż�ո�)���Ϊ$20$���ַ���

�����ļ������� ASCII �������32��126������֮��ͻ��з���

## �����ʽ
����ļ���$2$�У�

��һ���ϣ�д�������־����Ի��ĳ��ȣ�

�ڵڶ���д�öԻ�����Ϣ����1�����������������С�

## ˵��/��ʾ
ʱ�����ƣ�2S��

�ռ����ƣ�128MB��

```input1
6
@Petr: Leaving for #NEERC tomorrow!
@Roman: This #NEERC is going to be awesome!
@Stone_in_forest: Nothing happened today.
@NEERCNews: @Petr Don't forget an umbrella :)
@Lydia: @NEERCNews cares about @Petr - so cute ^_^
@Lydia: @Lydia @NEERCNews @Petr it won't be raining though!

```

```output1
3
1 4 5

```

## ��ʾ
Time limit: 2 s, Memory limit: 128 MB. 



