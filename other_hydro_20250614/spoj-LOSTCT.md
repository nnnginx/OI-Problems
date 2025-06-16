<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="#" onclick="change2En()">English</a></td>
<td width="50%"><a href="#" onclick="change2Vn()">Vietnamese</a></td>
</tr>
</tbody>
</table>
<div id="lang-vn" style="display:none">
<h2>Bí mật về thành phố biến mất</h2>
<p>Nhà khảo cổ nổi tiếng Blue Mary vừa tìm thấy di tích một   thành phố bị biến mất. Cô tìm thấy 12 tấm bia lớn ở trung tâm   thành phố, mà cô đặt tên là thành phố Đỉnh-Băng (Ice-Peak   City). Các tấm bia có nhiều kiến trúc khác nhau. Blue Mary đặt   tên các kiến trúc này là IPA (Ice-Peak Articles). Không may là   cô không thể tìm ra thành phố Đỉnh Băng nữa sau khi quay về   phòng thí nghiệm của mình.Điều duy nhất Blue Mary biết về thành phố Đỉnh Băng là   hình dạng kiến trúc của các tấm bia. Vốn thông minh, cô nhanh   chóng tìm ra cú pháp của IPA. Cú pháp có dạng như dưới   đây.</p>
<pre>&lt;IPA&gt;        ::=&lt;câu&gt;{&lt;câu&gt;}
&lt;câu&gt;        ::=&lt;ngữ danh từ&gt;{&lt;ngữ động từ&gt;&lt;ngữ danh từ&gt;}[&lt;ngữ động từ&gt;]
&lt;ngữ danh từ&gt;::=&lt;danh từ&gt;|[&lt;trạng từ&gt;]&lt;ngữ danh từ&gt;
&lt;ngữ động từ&gt;::=&lt;động từ&gt;|[&lt;trạng từ&gt;]&lt;ngữ động từ&gt;
&lt;từ&gt;         ::=&lt;động từ&gt;|&lt;danh từ&gt;|&lt;trạng từ&gt;
</pre>
<p>Trong đó</p>
<p>danh từ, động từ và trạng từ được cho trước bởi một từ   điển mà ta sẽ nêu sau.</p>
<p>| ký hiệu "hoặc"</p>
<p>&nbsp;</p>
<p>Các đối tượng trong dấu [] xuất hiện 0 hoặc 1 lần.</p>
<p>Các đối tượng trong dấu {} xuất hiện 0 hoặc nhiều   lần.</p>
<p>Blue Mary đã soạn một từ điển các từ trong IPA. Do các   ký tự trong IPA chỉ gồm 26 dạng khác nhau, ta sẽ dùng các   chữ cái latin in thường từ 'a' đến 'z' để biểu diễn.</p>
<p>Không có dấu câu ngăn cách giữa các từ hoặc câu, do đó   Blue Mary nhờ bạn viết chương trình phân tách chuỗi IPA cho   trước thành một số ít câu nhất, sau đó lại phân tách các câu   này ra thành ít từ nhất.Dữ liệu</p>
<p>Dòng đầu tiên chứa số từ trong từ điển, không vượt quá   1000.</p>
<p>Các dòng tiếp theo chứa các từ có dạng "X.Y", mỗi từ   trên một dòng, trong đó X là một trong các ký tự 'n', 'v', 'a',   cho biết từ tương ứng là danh từ, động từ hay trạng từ, và Y là   chuỗi gồm các chữ cái in thường thể hiện một từ, có độ dài   không quá 20.</p>
<p>Dòng tiếp theo chứa một chuỗi IPA đúng (chỉ gồm các   chữ cái latin in thường), kết thúc bởi dấu chấm (.). Độ dài của   chuỗi IPA sẽ không vượt quá 5KB.</p>
<h3>Kết quả</h3>
<p>Dòng đầu tiên chứa số câu ít nhất trong chuỗi IPA. Dòng   thứ hai chứa số từ ít nhất trong chuỗi IPA, sau khi chuỗi IPA   đã được phân tách thành ít câu nhất.</p>
<h3>Ví dụ</h3>
<pre><strong>Dữ liệu</strong>
11
n.table
n.baleine
a.silly
n.snoopy
n.sillysnoopy
v.is
v.isnot
n.kick
v.kick
a.big
v.cry
sillysnoopyisnotbigtablebaleinekicksnoopysillycry.

<strong>Kết quả</strong>
2
9
</pre>
</div>
<div id="lang-en">
<p>The famous archaeologist Blue Mary has found a site of a   lost city. She found 12 huge steles in the center of the city -   called Ice-Peak City by her, on which there were many designs.   Blue Mary named these designs Ice-Peak Articles(IPA for   short). Unfortunately, she can't find Ice-Peak city any more   after she returns to her lab.</p>
<p>The only thing Blue Mary knows about Ice-Peak city is   pictures of the designs on the steles. With her intelligence she   soon comes up with the syntax of IPA. Its BNF form is   below.</p>
<pre>&lt;IPA&gt;        ::=&lt;sentence&gt;{&lt;sentence&gt;}
&lt;sentence&gt;   ::=&lt;noun phrase&gt;{&lt;verb phrase&gt;&lt;noun phrase&gt;}[&lt;verb phrase&gt;]
&lt;noun phrase&gt;::=&lt;noun&gt;|[&lt;adverb&gt;]&lt;noun phrase&gt;
&lt;verb phrase&gt;::=&lt;verb&gt;|[&lt;adverb&gt;]&lt;verb phrase&gt;
&lt;words&gt;      ::=&lt;verb&gt;|&lt;noun&gt;|&lt;adverb&gt;
</pre>
<p>Where</p>
<p>nouns, verbs and adverbs are given by a dictionary which   we will discuss later.</p>
<p>| denotes or.</p>
<p>Things in [] will appear zero or one time.</p>
<p>Things in {} will appear zero or more times.</p>
<p>Blue Mary has compiled a dictionary of words in IPA.   Since characters appeared in IPA only contain 26 different   forms, we will use small latin letters 'a' to 'z' to represent.</p>
<p>There are no seperators between words or sentences, so   Blue Mary asks you to write a program which will split a   correct IPA into minimum number of sentences, and split these   sentences into minimum number of words.</p>
<h3>Input</h3>
<p>The first line contains the number of words in the   dictionary, no more than 1000.</p>
<p>Next lines contain the words in the form "X.Y", one per   line, where X is one of the characters 'n', 'v', 'a', denoting that   the corresponding word is noun, verb or adverb, and  Y is a   string of lowercase latin letters, whose length will be no nore   than 20.</p>
<p>The next line contains a correct IPA (contains only   lowercase latin letters), ends with a dot(.). The length of the   IPA will be no more than 5KB.</p>
<h3>Output</h3>
<p>The first line contains the minimum number of sentences in   IPA. The second line contains the minimum number of words   in IPA, when given IPA is split into minimum number of   sentences.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
11
n.table
n.baleine
a.silly
n.snoopy
n.sillysnoopy
v.is
v.isnot
n.kick
v.kick
a.big
v.cry
sillysnoopyisnotbigtablebaleinekicksnoopysillycry.

<strong>Output:</strong>
2
9
</pre>
</div>
<strong>Time limit has been changed to 200 ms in total for all tests.</strong>

<script> 
function change2En() {
	document.getElementById("lang-vn").style.display="none";
	document.getElementById("lang-en").style.display="block";
}
function change2Vn() {
	document.getElementById("lang-en").style.display="none";
	document.getElementById("lang-vn").style.display="block";
}
</script>