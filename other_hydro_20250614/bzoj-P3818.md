## ��Ŀ����

�ڽ��� Web ��˿���ʱ������Ҫ��һ������� router��ͨ����˵����˵Ĵ�������� action ��ɣ�router �����þ��ǽ������������� URL ��Ӧ����Ӧ�� action �ϡ�

���󵽴��� Web ������ʱ���Ѿ�����Ҫ���������Ͷ˿��ˣ����һ��������������ʽ��

`/{something_1}/{something_2}/.../{something_k}` �� `{something_1}/{something_2}/.../{something_k}?{parameter_list}`��

���� parameter_list �����Ϊ��`{name_1}={value_1}&{name_2}={value_2}&...&{name_n}={value_n}`������һ������е� parameter_list Ϊ�գ�

���� `/user/list/show?gender=male&birthyear=1990` ����һ���Ϸ����������а������������� gender �� birthyear����Ӧ�� value �ֱ��� male �� 1990��

router ������� path ��ɣ�ÿһ�� path ���Ӧ��һ�� action �ϡ�router ��ƥ�� URL �� path ʱֻ�� parameter_list ֮ǰ�Ĳ��֣�����֮ǰ�������ֻ�� `/user/list/show` �ⲿ�֡�parameter_list �ڵĲ����ᱻֱ���͵� action �С����һ�� path ���Ǿ���������ʽ��

`/{something_1}/{something_2}/.../{something_k}`��

Ϊ��ʹ�� router ����ÿһ���е� something ���˿����þ�����ַ����⣬��������һ��������ʽȥƥ�䣬������ȡ���ⲿ�ֵ�������Ϊ�����͵� action ȥ����������£�something ������Ϊ `:{regexp_name}`������ regexp_name ��Ӧһ��������ʽ�����ں����������ı��ʽ������ router �е�һ�� path Ϊ `/user/:handle/show`������ `:handle` ��Ӧ��һ��������ʽ������������ƥ��������СдӢ����ĸ��ɵķǿմ�����ʱ���� `/user/testuser/show` ����ƥ����� path���������� action ����һ�� name Ϊ handle��value Ϊ testuser �Ĳ���������������Ϊ `/user/testuser/show?avatar=true&message=hello` �Ļ���������ƥ��֮ǰ�� path���͵� action �Ĳ����ͻ���������handle��avatar��message����Ӧ�� value �ֱ�Ϊ testuser��true �� hello��

����ʹ�ô�������ʽ�� path ʱҲ�ܵ�һЩ���ơ�������˵������� router �������� path������ǰ�� $i$ �� something �ε�������ȫ��ͬ���� $i$ ��������Ժ�������ʽ���ʱ��Ҫ����������ͬ��������ʽ����Ȼ��� $i+1$ �� something �ε����ݲ�ͬ����������������

һ�� path ��һ�ε���������ͨ�ַ�������һ�� path ��һ�ε����ݶ�Ӧ��������ʽ����ô���������ʽһ���޷�ƥ��ǰһ�� path �� $i+1$ �ε��ַ���������һ�� path �� `/foo/:tmp/bar/pop`����һ�� path �� `/foo/:tmp/:exp/push`����ô exp ��Ӧ��������ʽһ������ƥ�� bar��

���� path ��һ�ε����ݶ���������ʽ����ô������������ʽƥ����ַ���һ��û�н���������һ�� path �� `/foo/:tmp/:aaa/push`����һ�� path �� `/foo/:tmp/:bbb/pop`����ô������һ���ַ�����ͬʱ�� aaa ��Ӧ��������ʽ�� bbb ��Ӧ��������ʽƥ�䡣

������������ʽ��Ϊ���������һЩ�������е�������ʽ���������ʵ��ʹ�õ������򻯡�������ʽ���ķ����� Atom��Quantifier��Term��Alternative �⼸������� Regexp ��ʾ������ʽ����ÿ�ָ������Ϊ��

Regexp �����ɵ��� Alternative ��ɣ�������һ�� Alternative ��һ�� Regexp ��ɣ��м����ַ� `|` ���ӡ�����ǰһ���������������ʽƥ������ Alternative ��ƥ��Ķ��������ں�һ�������һ���ַ���Ҫ�ܱ���������ʽƥ�䣬Ҫô�ܱ� `|` ǰ��� Alternative ��ƥ�䣬Ҫô�ܱ� `|` ����� Regexp ��ƥ�䡣

Alternative �ɵ��� Term ���� Term ������ɣ�����ƥ����Щ Term ��ƥ����ַ��������ӡ�����֮��һ���ַ���Ҫ����� Alternative ƥ�䣬����ַ����ܹ�������ɶΣ������� Alternative �� Term ����һ���ࣩ��ÿ�����α� Alternative ��ÿ�� Term ƥ�䡣

Term ��һ�� Atom ��һ�� Atom ����һ�� Quantifier ��ɡ�������˽⵽��Quantifier ��Ӧ�������ظ����������䡣�� Term �ɵ��� Atom ��ɣ��� Term ��ƥ��������� Atom ��ͬ����� Atom ����� Quantifier�������һ���ַ����ܻ���Ϊ���ɶΣ����ֵĶ����� Quantifier ָ���������ڣ���ʹ��ÿ�ζ��ܱ� Atom ƥ�䣬��ô����ַ������ܱ���� Term ƥ�䡣

Quantifier ����ʽΪ `{lower_bound,upper_bound}`������ lower_bound �� upper_bound ����Ӧһ�������� $20$ �ķǸ����������� `upper_bound��lower_bound`��Quantifier ��Ӧ������Ϊ������ `[lower_bound,upper_bound]`��ע�� upper_bound ����Ϊ�գ���ʱ�м�Ķ��Ż����еģ���upper_bound Ϊ�ձ�ʾ�Ͻ�Ϊ�����`{1,3},{0,1},{2,2},{3,}` ��Ϊ�Ϸ���Quantifier���� `{3,2},{,1}` �Ͳ��Ϸ���

Atom ��������ʽ����һ��Ϊ�����ַ��������ַ�Լ��ֻ����Ӣ���ַ���������д��Сд�������֣�������ʽ�µ� Atom ����ƥ������ݾ��Ǹ��ַ����ڶ�����ʽΪ�ַ����䣬������ʽΪ `[lower-upper]`������ lower �� upper ��Ϊ�����ַ�������ҪôͬʱΪСдӢ����ĸ��ҪôͬʱΪ��д��ĸ��ҪôͬʱΪ���֣����� lower �� ASCII �벻С�� upper �� ASCII �룬��������µ� Atom ����ƥ������ݾ�����������ڵ��ַ������� lower �� upper������������ʽ�� `(Regexp)`����һ���Ϸ���������ʽ����һ�����ţ���������¸� Atom ��ƥ������ݺ������ڵ�������ʽ��ͬ��

���������ķ���`[0-9]{1,3}` Ϊ�Ϸ���������ʽ������ƥ�䳤��Ϊ $1\sim 3$ ����������ɵ��ַ�����`([a-z]|[0-9]){3,10}` ҲΪ�Ϸ���������ʽ������ƥ�䳤��Ϊ $3\sim 10$ ����СдӢ����ĸ��������ɵ��ַ����������ӵ�һ������Ϊ `01[0-1]{0,}|10[0-1]{0,}`������ƥ������ `01` �� `10` ��ͷ�� 01 �ַ�����

## �����ʽ

��һ��һ�������� $T$����ʾ���ݵ��������������θ���ÿ�����ݡ�

ÿ�����ݵĵ�һ�а���һ�������� $n$����ʾ router ���� $n$ �� path������ $2n$ �У�ÿ��������һ�� path����һ��Ϊ path ƥ��� URL����ʽΪ `/{something_1}/{something_2}/.../{something_k}`��

ÿ�� something ҪôΪ������ַ������ɴ�дӢ����ĸ��СдӢ����ĸ����������ҳ����� $[1,50]$ �ڣ���ҪôΪ `:{regexp_name}`������ regexp_name �ɴ�д��СдӢ����ĸ����ҳ��Ȳ����� $30$�������������ʽ����֮��������и����������� path �ĵڶ���Ϊ��Ӧ�� action ���ƣ��ɴ�д��СдӢ����ĸ��ɣ������� $[1,30]$ �ڣ���

��������������ǰ�� path �г��ֵ�����������ʽ��ÿ������һ��������ʽ��ÿ���ڰ��������ǿ��ַ�������һ���ո��������ǰ����ַ�����ʾ regexp_name��������ַ�����ʾ��Ӧ������ʽ�����Ȳ����� $50$����ע��ͬһ�� regexp_name ������ǰ������� path �г��ֶ�Σ�һ�� path �г��ֶ�λ��ڲ�ͬ path �г��֣���������������Ƕ�Ӧ��������ʽ����ͬ�ģ�����������ֻ������һ�Ρ�����ͬʱ��֤��������� regexp_name ��������һ�� path �г��ֹ���

����һ�а���һ�������� $m$����ʾ�� $m$ �������˹��������� $m$ �У�ÿ������һ������� URL��URL Ϊ `/{something_1}/{something_2}/.../{something_k}` �� `/{something_1}/{something_2}/.../{something_k}?{name_1}={value_1}&{name_2}={value_2}&...&{name_n}={value_n}` ����ʽ���������� something �� value ���ɴ�дӢ����ĸ��СдӢ����ĸ����������ҳ����� $[1,50]$ �ڣ����� name ���ɴ�д��СдӢ����ĸ����ҳ����� $[1,30]$ �ڡ�

## �����ʽ

����ÿ�����ݣ��ȵ���һ����� `Case #{case_no}:`������ case_no ��ʾ��ǰ�ǵڼ������ݣ��� $1$ ��ʼ��ţ���

ÿ��������ζ�Ӧÿ���������û�� path �ܹ�ƥ�������� URL����� `404 Not Found`��

����� path �ܹ�ƥ���������� `Request matches action "{action_name}" with parameters {parameter_list}`������ action_name Ϊƥ�� path ��Ӧ action �����ƣ�parameter_list Ϊ���еĲ�����

���� parameter_list ��һ���ֵ�ķ�ʽ������������������������ǵ� name Ϊ avatar��message �� page����Ӧ�� value �ֱ�Ϊ true��hello �� 2����ô����� parameter_list Ϊ `{"avatar":"true","message":"hello","page":"2"}`�����в������� name ���ֵ������У���

ע��һ�������У�ӵ����ͬ name �Ĳ������ܳ��ֶ�Σ���������� URL Ϊ `/user/me/show?name=you&name=he`��ƥ��� path Ϊ `/user/:name/show`����ʱ�� parameter_list Ϊ `{"name":["me","you","he"]}`�����������水�ղ��������� URL �г��ֵĴ��������

��������������ο������������ܹ���֤һ�����󲻻ᱻ��� path ƥ�䡣

```input1
3
3
/user/:id/show
userShow
/message/list
messageList
/message/:id/show
messageShow
id [0-9]{2,4}
3
/message/list
/user/123/show?avatar=true
/message/5312/show?page=1
1
/foo/:id/:bar/:bar
fun
id [0-9]{2,4}
bar [a-z]{1,3}
1
/foo/777/az/bc?bar=xyz&bar=zzz
2
/user/:handle/show
userShow
/user/:id/show
userShow
id [0-9]{2,4}
handle ([a-z]|[A-Z])([a-z]|[A-Z]|[0-9]){4,10}
4
/user/259/show
/user/wjmzbmr/show?like=true
/user/0xxx/show
/user/WJMZBMR/show?love=true
```

```output1
Case #1:
Request matches action "messageList" with parameters {}
Request matches action "userShow" with parameters {"avatar":"true","id":"123"}
Request matches action "messageShow" with parameters {"id":"5312","page":"1"}
Case #2:
Request matches action "fun" with parameters {"bar":["az","bc","xyz","zzz"],"id":"777"}
Case #3:
Request matches action "userShow" with parameters {"id":"259"}
Request matches action "userShow" with parameters {"handle":"wjmzbmr","like":"true"}
404 Not Found
Request matches action "userShow" with parameters {"handle":"WJMZBMR","love":"true"}
```

## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ�$1\leq n,m\leq 2\times 10^4$��$1\leq T\leq 5$�������ļ���С������ $10$ MB����ͬ���Ƶ�������ʽ����� $50$ ����

## ��Դ

$2015$ ����Ҽ�ѵ�Ӳ��ԡ�

