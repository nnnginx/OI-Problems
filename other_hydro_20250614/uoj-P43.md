<p>�ڽ��� Web ��˿���ʱ������Ҫ��һ������� router��ͨ����˵����˵Ĵ�������� action ��ɣ�router �����þ��ǽ������������� URL ��Ӧ����Ӧ�� action �ϡ�</p>
<p>���󵽴��� Web ������ʱ���Ѿ�����Ҫ���������Ͷ˿��ˣ����һ��������������ʽ��</p>
<p>��<samp>/{something_1}/{something_2}/.../{something_k}</samp>�� �� ��<samp>/{something_1}/{something_2}/.../{something_k}?{parameter_list}</samp>��</p>
<p>���� parameter_list �����Ϊ����<samp>{name_1}={value_1}&amp;{name_2}={value_2}&amp;...&amp;{name_n}={value_n}</samp>��������һ������е� parameter_list Ϊ�գ�</p>
<p>���� ��<samp>/user/list/show?gender=male&amp;birthyear=1990</samp>�� ����һ���Ϸ����������а������������� gender �� birthyear����Ӧ�� value �ֱ��� male �� 1990��</p>
<p>router ������� path ��ɣ�ÿһ�� path ���Ӧ��һ�� action �ϡ�router ��ƥ�� URL �� path ʱֻ�� parameter_list ֮ǰ�Ĳ��֣�����֮ǰ�������ֻ�� ��<samp>/user/list/show</samp>�� �ⲿ�֡�parameter_list �ڵĲ����ᱻֱ���͵� action �С����һ�� path ���Ǿ���������ʽ��</p>
<p>��<samp>/{something_1}/{something_2}/.../{something_k}</samp>��</p>
<p>Ϊ��ʹ�� router ����ÿһ���е� something ���˿����þ�����ַ����⣬��������һ��������ʽȥƥ�䣬������ȡ���ⲿ�ֵ�������Ϊ�����͵� action ȥ����������£�something ������Ϊ��<samp>:{regexp_name}</samp>�������� regexp_name ��Ӧһ��������ʽ�����ں����������ı��ʽ������ router �е�һ�� path Ϊ ��<samp>/user/:handle/show</samp>�������С�<samp>:handle</samp>�� ��Ӧ��һ��������ʽ������������ƥ��������СдӢ����ĸ��ɵķǿմ�����ʱ���� ��<samp>/user/testuser/show</samp>�� ����ƥ����� path���������� action ����һ�� name Ϊ handle��value Ϊ testuser �Ĳ���������������Ϊ ��<samp>/user/testuser/show?avatar=true&amp;message=hello</samp>�� �Ļ���������ƥ��֮ǰ�� path���͵� action �Ĳ����ͻ���������handle��avatar��message����Ӧ�� value �ֱ�Ϊ testuser��true �� hello��</p>
<p>����ʹ�ô�������ʽ�� path ʱҲ�ܵ�һЩ���ơ�������˵������� router �������� path������ǰ�� $i$ �� something �ε�������ȫ��ͬ���� $i$ ��������Ժ�������ʽ���ʱ��Ҫ����������ͬ��������ʽ����Ȼ��� $i+1$ �� something �ε����ݲ�ͬ����������������</p>
<ol><li>һ�� path ��һ�ε���������ͨ�ַ�������һ�� path ��һ�ε����ݶ�Ӧ��������ʽ����ô���������ʽһ���޷�ƥ��ǰһ�� path �� $i+1$ �ε��ַ���������һ�� path �� ��<samp>/foo/:tmp/bar/pop</samp>������һ�� path �� ��<samp>/foo/:tmp/:exp/push</samp>������ô exp ��Ӧ��������ʽһ������ƥ�� bar��</li>
<li>���� path ��һ�ε����ݶ���������ʽ����ô������������ʽƥ����ַ���һ��û�н���������һ�� path �� ��<samp>/foo/:tmp/:aaa/push</samp>������һ�� path �� ��<samp>/foo/:tmp/:bbb/pop</samp>������ô������һ���ַ�����ͬʱ�� aaa ��Ӧ��������ʽ�� bbb ��Ӧ��������ʽƥ�䡣</li>
</ol><p>������������ʽ��Ϊ���������һЩ�������е�������ʽ���������ʵ��ʹ�õ������򻯡�������ʽ���ķ����� Atom��Quantifier��Term��Alternative �⼸������� Regexp ��ʾ������ʽ����ÿ�ָ������Ϊ��</p>
<ol><li>Regexp �����ɵ��� Alternative ��ɣ�������һ�� Alternative ��һ�� Regexp ��ɣ��м����ַ� ��<samp>|</samp>�� ���ӡ�����ǰһ���������������ʽƥ������ Alternative ��ƥ��Ķ��������ں�һ�������һ���ַ���Ҫ�ܱ���������ʽƥ�䣬Ҫô�ܱ� ��<samp>|</samp>�� ǰ��� Alternative ��ƥ�䣬Ҫô�ܱ� ��<samp>|</samp>�� ����� Regexp��ƥ�䡣</li>
<li>Alternative �ɵ��� Term ���� Term ������ɣ�����ƥ����Щ Term ��ƥ����ַ��������ӡ�����֮��һ���ַ���Ҫ����� Alternative ƥ�䣬����ַ����ܹ�������ɶΣ������� Alternative �� Term ����һ���ࣩ��ÿ�����α� Alternative ��ÿ�� Term ƥ�䡣</li>
<li>Term ��һ�� Atom ��һ�� Atom ����һ�� Quantifier ��ɡ�������˽⵽��Quantifier ��Ӧ�������ظ����������䡣�� Term �ɵ��� Atom ��ɣ��� Term ��ƥ��������� Atom ��ͬ����� Atom ����� Quantifier�������һ���ַ����ܻ���Ϊ���ɶΣ����ֵĶ����� Quantifier ָ���������ڣ���ʹ��ÿ�ζ��ܱ� Atom ƥ�䣬��ô����ַ������ܱ���� Term ƥ�䡣</li>
<li>Quantifier ����ʽΪ ��<samp>{lower_bound,upper_bound}</samp>�������� lower_bound �� upper_bound ����Ӧһ�������� $20$ �ķǸ����������� $\text{upper_bound} \geq \text{lower_bound}$��Quantifier ��Ӧ������Ϊ������ $[\text{lower_bound}, \text{upper_bound}]$��ע�� upper_bound ����Ϊ�գ���ʱ�м�Ķ��Ż����еģ���upper_bound Ϊ�ձ�ʾ�Ͻ�Ϊ�����<samp>{1,3}</samp>, <samp>{0,1}</samp>, <samp>{2,2}</samp>, <samp>{3,}</samp> ��Ϊ�Ϸ��� Quantifier���� <samp>{3,2}</samp>, <samp>{,1}</samp> �Ͳ��Ϸ���</li>
<li>Atom ��������ʽ����һ��Ϊ�����ַ��������ַ�Լ��ֻ����Ӣ���ַ���������д��Сд�������֣�������ʽ�µ� Atom ����ƥ������ݾ��Ǹ��ַ����ڶ�����ʽΪ�ַ����䣬������ʽΪ ��<samp>[lower-upper]</samp>�������� lower �� upper ��Ϊ�����ַ�������ҪôͬʱΪСдӢ����ĸ��ҪôͬʱΪ��д��ĸ��ҪôͬʱΪ���֣����� lower ��ASCII�벻С�� upper ��ASCII�룬��������µ� Atom ����ƥ������ݾ�����������ڵ��ַ������� lower �� upper������������ʽ�� ��<samp>(Regexp)</samp>������һ���Ϸ���������ʽ����һ�����ţ���������¸� Atom ��ƥ������ݺ������ڵ�������ʽ��ͬ��</li>
</ol><p>���������ķ�����<samp>[0-9]{1,3}</samp>�� Ϊ�Ϸ���������ʽ������ƥ�䳤��Ϊ $1 \sim 3$ ����������ɵ��ַ�������<samp>([a-z]|[0-9]){3,10}</samp>�� ҲΪ�Ϸ���������ʽ������ƥ�䳤��Ϊ $3 \sim 10$ ����СдӢ����ĸ��������ɵ��ַ����������ӵ�һ������Ϊ ��<samp>01[0-1]{0,}|10[0-1]{0,}</samp>��������ƥ������ <samp>01</samp> �� <samp>10</samp> ��ͷ�� <samp>01</samp> �ַ�����</p>
<h2>�����ʽ</h2>
<p>��һ��һ�������� $T$����ʾ���ݵ��������������θ���ÿ�����ݡ�</p>
<p>ÿ�����ݵĵ�һ�а���һ�������� $N$����ʾ router ���� $N$ �� path������ $2N$ �У�ÿ��������һ�� path����һ��Ϊ path ƥ��� URL����ʽΪ</p>
<p>��<samp>/{something_1}/{something_2}/.../{something_k}</samp>��</p>
<p>ÿ�� something ҪôΪ������ַ������ɴ�дӢ����ĸ��СдӢ����ĸ����������ҳ����� $[1,50]$ �ڣ���ҪôΪ ��<samp>:{regexp_name}</samp>�������� regexp_name �ɴ�д��СдӢ����ĸ����ҳ��Ȳ����� $30$�������������ʽ����֮��������и����������� path �ĵڶ���Ϊ��Ӧ�� action ���ƣ��ɴ�д��СдӢ����ĸ��ɣ������� $[1,30]$ �ڣ���</p>
<p>��������������ǰ�� path �г��ֵ�����������ʽ��ÿ������һ��������ʽ��ÿ���ڰ��������ǿ��ַ�������һ���ո��������ǰ����ַ�����ʾ regexp_name��������ַ�����ʾ��Ӧ������ʽ�����Ȳ����� $50$����ע��ͬһ�� regexp_name ������ǰ������� path �г��ֶ�Σ�һ�� path �г��ֶ�λ��ڲ�ͬ path �г��֣���������������Ƕ�Ӧ��������ʽ����ͬ�ģ�����������ֻ������һ�Ρ�����ͬʱ��֤��������� regexp_name ��������һ�� path �г��ֹ���</p>
<p>����һ�а���һ�������� $M$����ʾ�� $M$ �������˹��������� $M$ �У�ÿ������һ������� URL��URL Ϊ ��<samp>/{something_1}/{something_2}/.../{something_k}</samp>�� �� ��<samp>/{something_1}/{something_2}/.../{something_k}?{name_1}={value_1}&amp;{name_2}={value_2}&amp;...&amp;{name_n}={value_n}</samp>�� ����ʽ���������� something �� value ���ɴ�дӢ����ĸ��СдӢ����ĸ����������ҳ����� $[1,50]$ �ڣ����� name ���ɴ�д��СдӢ����ĸ����ҳ����� $[1,30]$ �ڡ�</p>
<h2>�����ʽ</h2>
<p>����ÿ�����ݣ��ȵ���һ����� ��<samp>Case #{case_no}:</samp>�����������ţ������� case_no ��ʾ��ǰ�ǵڼ������ݣ��� $1$ ��ʼ��ţ���</p>
<p>ÿ��������ζ�Ӧÿ���������û�� path �ܹ�ƥ�������� URL����� ��<samp>404 Not Found</samp>����</p>
<p>����� path �ܹ�ƥ���������� ��<samp>Request matches action "{action_name}" with parameters {parameter_list}</samp>�������� action_name Ϊƥ�� path ��Ӧ action �����ƣ�parameter_list Ϊ���еĲ�����</p>
<ul><li>���� parameter_list ��һ���ֵ�ķ�ʽ������������������������ǵ� name Ϊ avatar��message �� page����Ӧ�� value �ֱ�Ϊ true��hello �� 2����ô����� parameter_list Ϊ ��<samp>{"avatar":"true","message":"hello","page":"2"}</samp>�������в������� name ���ֵ������У���</li>
<li>ע��һ�������У�ӵ����ͬ name �Ĳ������ܳ��ֶ�Σ���������� URL Ϊ ��<samp>/user/me/show?name=you&amp;name=he</samp>����ƥ��� path Ϊ ��<samp>/user/:name/show</samp>������ʱ�� parameter_list Ϊ ��<samp>{"name":["me","you","he"]}</samp>�������������水�ղ��������� URL �г��ֵĴ��������</li>
<li>��������������ο������������ܹ���֤һ�����󲻻ᱻ��� path ƥ�䡣</li>
</ul>

<pre><code class="language-input1">3
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
/foo/777/az/bc?bar=xyz&amp;bar=zzz
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
</code></pre>


<pre><code class="language-output1">Case #1:
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
</code></pre>

<h2>������Լ��</h2>
<p>���� 30% �����ݣ�path �в������������ʽ��</p>
<p>���� 100% �����ݣ�$N, M \leq 20000$��$T \leq 5$�������ļ���С������ $10\texttt{MB}$����ͬ���Ƶ�������ʽ����� $50$ ����</p>
<p><strong>ע������������������ݡ�</strong></p>
<p><strong>ʱ������</strong>��$20\texttt{s}$</p>
<p><strong>�ռ�����</strong>��$256\texttt{MB}$</p>
<h2>��Դ</h2>
<p>�й����Ҷ��廪��ѵ2014~2015 Day 3 - By ��־��</p>
<h2>����</h2>
<p><a href="./20483/file/attachment.zip">������������</a></p>
