<p><span style="font-size: small;">(For Vietnamese version, see below.)</span></p>
<p>&nbsp;</p>
<p><span style="font-size: small;">Farmer John has N cows that need to be milked (1 &lt;= N &lt;= 10,000), each of which takes only one unit of time to milk.</span></p>
<p><span style="font-size: small;">Being impatient animals, some cows will refuse to be milked if Farmer John waits too long to milk them. More specifically, cow i produces g_i gallons of milk (1 &lt;= g_i &lt;= 1000), but only if she is milked before a deadline at time d_i (1 &lt;= d_i &lt;= 10,000). Time starts at t=0, so at most x total cows can be milked prior to a deadline at time t=x.</span></p>
<p><span style="font-size: small;">Please help Farmer John determine the maximum amount of milk that he can obtain if he milks the cows optimally.</span></p>
<p><span style="font-size: small;"><strong>Input </strong>:</span></p>
<p><span style="font-size: small;">&nbsp;- Line 1: The value of N.</span></p>
<p><span style="font-size: small;">&nbsp;- Lines 2..1+N: Line i+1 contains the integers g_i and d_i.</span></p>
<p><span style="font-size: small;"><strong>Output </strong>: A single numbers denotes the maximum number of gallons of milk Farmer John can obtain.</span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"><strong>Sample</strong> :</span></p>
<p><span style="font-size: small;">&nbsp;<strong>Input:</strong></span></p>
<p><span style="font-size: small;">&nbsp;4</span></p>
<p><span style="font-size: small;">&nbsp;10 3</span></p>
<p><span style="font-size: small;">&nbsp;7 5</span></p>
<p><span style="font-size: small;">&nbsp;8 1</span></p>
<p><span style="font-size: small;">&nbsp;2 1</span></p>
<p><span style="font-size: small;">&nbsp;<strong>Output :</strong></span></p>
<p><span style="font-size: small;">&nbsp;25</span></p>
<p><span style="font-size: small;">Input details : There are 4 cows. The first produces 10 gallons of milk if milked by time 3, and so on.</span></p>
<p><span style="font-size: small;">Output details : Farmer John milks cow 3 first, giving up on cow 4 since she cannot be milked by her deadline due to the conflict with cow 3. Farmer John then milks cows 1 and 2.</span></p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><span style="font-size: small;">***</span></p>
<p>&nbsp;</p>
<p><span style="font-size: small;">Nông dân John có N con bò, để vắt sữa một con bò cần 1 đơn vị thời gian.</span></p>
<p><span style="font-size: small;">Vốn là loài vật lười, những con bò sẽ không chịu để vắt sữa nếu John bắt chúng chờ quá lâu. Cụ thể, con bò i cho g_i gallon sữa, nhưng chỉ khi nó được vắt sữa trước thời gian d_i. Thời gian bắt đầu ở T = 0, nên có tối đa X con bò có thể được vắt sữa trước thời hạn T = X.</span></p>
<p><span style="font-size: small;">Hãy giúp nông dân John tính lượng sữa tối đa mà ông có thể vắt được nếu như ông chọn được cách vắt hiệu quả nhất.</span></p>
<p><span style="font-size: small;"><strong>Input :</strong></span></p>
<p><span style="font-size: small;">&nbsp;- Dòng 1 : chứa số nguyên dương N.</span></p>
<p><span style="font-size: small;">&nbsp;- Dòng 2 -&gt; n + 1 : dòng thứ i + 1 chứa 2 số nguyên g_i và d_i.</span></p>
<p><span style="font-size: small;"><strong>Output :</strong></span></p>
<p><span style="font-size: small;">&nbsp;- Lượng sữa nhiều nhất mà John có thể vắt.</span></p>
<p><span style="font-size: small;"><strong>Giới hạn :</strong></span></p>
<p><span style="font-size: small;">&nbsp;-&nbsp;1 ≤ n&nbsp;≤ 10000</span></p>
<p><span style="font-size: small;">&nbsp;- 1&nbsp;≤ g_i&nbsp;≤ 1000</span></p>
<p><span style="font-size: small;">&nbsp;- 1&nbsp;≤ d_i&nbsp;≤ 10000</span></p>
<p><span style="font-size: small;"><strong>Ví dụ :</strong></span></p>
<p><span style="font-size: small;">Input :</span></p>
<p><span style="font-size: small;">&nbsp;4</span></p>
<p><span style="font-size: small;">&nbsp;10 3</span></p>
<p><span style="font-size: small;">&nbsp;7 5</span></p>
<p><span style="font-size: small;">&nbsp;8 1</span></p>
<p><span style="font-size: small;">&nbsp;2 1</span></p>
<p><span style="font-size: small;">Output :</span></p>
<p><span style="font-size: small;">&nbsp;25</span></p>
<p><span style="font-size: small;">Giải thích : John vắt sữa con bò 3, sau đó đến con 1 rồi con 2.</span></p>
<div><span style="font-size: small;"><br></span></div>