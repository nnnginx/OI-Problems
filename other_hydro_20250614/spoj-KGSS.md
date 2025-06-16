<div align="left">
You are given a sequence A[1], A[2], ..., A[N] ( 0 ¡Ü A[i] ¡Ü 10^8 , 2 ¡Ü N ¡Ü 10^5 ). There are two types of operations and they are defined as follows:<p></p>
<b>Update:</b>
<p>
This will be indicated in the input by a 'U' followed by space and then two integers i and x.</p><p>
<b>U i x</b>, 1 ¡Ü i ¡Ü N, and x, 0 ¡Ü x ¡Ü 10^8.</p><p>
This operation sets the value of A[i] to x.</p>
<b>Query:</b>
<p>
This will be indicated in the input by a 'Q' followed by a single space and then two integers i and j.</p><p>
<b>Q x y</b>, 1 ¡Ü x &lt; y ¡Ü N. </p><p>
You must find i and j such that x ¡Ü i, j ¡Ü y and i != j, such that the sum A[i]+A[j] is maximized. Print the sum A[i]+A[j].
</p>
<h3 align="center">Input</h3>
<p>The first line of input consists of an integer <b>N</b> representing the length of the sequence. Next
line consists of N space separated integers A[i]. Next line contains an integer <b>Q</b>, Q ¡Ü 10^5, representing the number of operations. Next Q lines contain the operations.

</p><h3 align="center">Output</h3>
<p>Output the maximum sum mentioned above, in a separate line, for each Query.

</p><h3 align="center">Example</h3>

<pre><b>Input:</b>
5
1 2 3 4 5
6
Q 2 4
Q 2 5
U 1 6
Q 1 5
U 1 7
Q 1 5

<b>Output:</b>
7
9
11
12

</pre>
<div align="center">
<b>Warning: large Input/Output data, be careful with certain languages</b>
</div>
</div>

<div class="text-center">
	<a href="/submit/KGSS/" class="btn btn-primary btn-lg"><i class="fa fa-send"></i> Submit solution!</a>
</div>
			<!-- google_ad_section_end -->
			
			<div id="ccontent">
			<!-- google_ad_section_start -->
			
<hr style="clear:both;">
<a href="#" onclick="toggleComments(); return false;"><span id="comments_sh">hide</span> comments</a><br>

<a id="comments"></a>
<table id="comments_table" width="100%">
		<tbody><tr>
		<td colspan="2">
		<ul class="pagination" style="">
			<li class="disabled"><span>&lt;</span></li>
		<li class="disabled"><span>Previous</span></li>
						<li class="active"><span>1</span></li> 
							<li><a href="/problems/KGSS/cstart=10" class="pager_link">2</a></li> 
							<li><a href="/problems/KGSS/cstart=20" class="pager_link">3</a></li> 
							<li><a href="/problems/KGSS/cstart=30" class="pager_link">4</a></li> 
							<li><a href="/problems/KGSS/cstart=40" class="pager_link">5</a></li> 
							<li><a href="/problems/KGSS/cstart=50" class="pager_link">6</a></li> 
							<li><a href="/problems/KGSS/cstart=60" class="pager_link">7</a></li> 
							<li><a href="/problems/KGSS/cstart=70" class="pager_link">8</a></li> 
							<li><a href="/problems/KGSS/cstart=80" class="pager_link">9</a></li> 
							<li><a href="/problems/KGSS/cstart=90" class="pager_link">10</a></li> 
							<li><a href="/problems/KGSS/cstart=100" class="pager_link">11</a></li> 
						<li><a href="/problems/KGSS/cstart=10" class="pager_link">Next</a></li>
		<li><a href="/problems/KGSS/cstart=100" class="pager_link">&gt;</a></li>
	</ul>
		</td>
	</tr>
	<tr>
		<td colspan="2">
				</td>
	</tr>
	
	<script language="JavaScript">
	<!--
	$(document).ready(function(){
        $('.pager_link').bind('click', function(me){
                var href=$(me.currentTarget).attr('href');
		$('#ccontent').animate({opacity: 0.5},1);
                $.ajax({
                        type: "GET",
                        url: href+",ajax=1",
                        contentType: "application/x-www-form-urlencoded;charset=ISO-8859-2",
                        success: function(data){
                                $('#ccontent').html(data);
				$('#ccontent').animate({opacity: 1.0},1);
                        },
                        error: function(err){
                                alert('error');
                        }
                });
                return false;
        });
	});
	-->
	</script>
	



			
	<tr>
		<td width="50" style="vertical-align:top;">
			<img src="file://d78nocSb.png">
		</td>
		<td class="comm comm_odd">
			<a href="/users/mortal_beast">mortal_beast</a>: 
								<span style="font-size: 10px; color: #666;">2021-06-06 15:17:15</span>
		<br>
				<p>Good for begineers</p>
						</td>
	</tr>
				
	<tr>
		<td width="50" style="vertical-align:top;">
			<img src="file://HmZCM7gf.png">
		</td>
		<td class="comm comm_even">
			<a href="/users/rimuru_404">rimuru_404</a>: 
								<span style="font-size: 10px; color: #666;">2021-06-05 05:38:54</span>
		<br>
				<p>After some silly mistakes AC. Nice problem for segment tree beginners </p>
						</td>
	</tr>
				
	<tr>
		<td width="50" style="vertical-align:top;">
			<img src="file://pMzZ5gR1.png">
		</td>
		<td class="comm comm_odd">
			<a href="/users/mukund007">mukund007</a>: 
								<span style="font-size: 10px; color: #666;">2021-05-30 08:43:03</span>
		<br>
				<p>Fenwick Tree go go</p>
						</td>
	</tr>
				
	<tr>
		<td width="50" style="vertical-align:top;">
			<img src="file://6UrsLanD.png">
		</td>
		<td class="comm comm_even">
			<a href="/users/saurabh_kl">saurabh_kl</a>: 
								<span style="font-size: 10px; color: #666;">2021-02-11 21:05:39</span>
		<br>
				<p>Accepting Java solution, I don't know it gives TLE with Scanner or not but FastReader is okay</p>
				<b>Last edit: 2021-02-11 21:06:32</b>
						</td>
	</tr>
				
	<tr>
		<td width="50" style="vertical-align:top;">
			<img src="file://hIgvOrGo.png">
		</td>
		<td class="comm comm_odd">
			<a href="/users/kanisht09">kanisht09</a>: 
								<span style="font-size: 10px; color: #666;">2021-01-22 21:47:48</span>
		<br>
				<p>Solved it using segment trees 2 different ways</p>
						</td>
	</tr>
				
	<tr>
		<td width="50" style="vertical-align:top;">
			<img src="file://jhbNMT1m.png">
		</td>
		<td class="comm comm_even">
			<a href="/users/saurav7192">saurav7192</a>: 
								<span style="font-size: 10px; color: #666;">2020-08-06 10:56:08</span>
		<br>
				<p>Aced finally..............................</p>
				<b>Last edit: 2020-08-06 12:30:50</b>
						</td>
	</tr>
				
	<tr>
		<td width="50" style="vertical-align:top;">
			<img src="file://6JNI9oeO.png">
		</td>
		<td class="comm comm_odd">
			<a href="/users/skj_helloworld">skj_helloworld</a>: 
								<span style="font-size: 10px; color: #666;">2020-08-04 12:34:34</span>
		<br>
				<p>accepted in one go</p>
						</td>
	</tr>
				
	<tr>
		<td width="50" style="vertical-align:top;">
			<img src="file://9EZJX07Y.png">
		</td>
		<td class="comm comm_even">
			<a href="/users/chefpr7">chefpr7</a>: 
								<span style="font-size: 10px; color: #666;">2020-07-02 09:09:33</span>
		<br>
				<p>AC in One Go!! Nice practice problem for newbies!</p>
						</td>
	</tr>
				
	<tr>
		<td width="50" style="vertical-align:top;">
			<img src="file://FqPk2abE.png">
		</td>
		<td class="comm comm_odd">
			<a href="/users/wargang">wargang</a>: 
								<span style="font-size: 10px; color: #666;">2020-07-01 13:25:12</span>
		<br>
				<p>very nice problem!!
<br></p>
						</td>
	</tr>
				
	<tr>
		<td width="50" style="vertical-align:top;">
			<img src="file://DV32nsJ2.png">
		</td>
		<td class="comm comm_even">
			<a href="/users/sarthak_19">sarthak_19</a>: 
								<span style="font-size: 10px; color: #666;">2020-06-29 06:21:49</span>
		<br>
				<p>AC in one GO!!!!!!!!
<br>Good for Beginners</p>
						</td>
	</tr>
			
</tbody></table>


<script language="javascript" type="text/javascript">
<!--
function getCookieVal (offset) {
        var endstr = document.cookie.indexOf (";", offset);
        if (endstr == -1) { 
                endstr = document.cookie.length; 
        }
        return unescape(document.cookie.substring(offset, endstr));
}

function GetCookie (name) {
  var arg = name + "=";
  var alen = arg.length;
  var clen = document.cookie.length;
  var i = 0;
  while (i < clen) {
    var j = i + alen;
    if (document.cookie.substring(i, j) == arg) {
      return getCookieVal (j);
      }
    i = document.cookie.indexOf(" ", i) + 1;
    if (i == 0) break; 
    }
  return null;
}

function toggleComments() {
        var a = document.getElementById('comments_table');
        var d = a.style.display;
        if( d == "" || d == "block" ){
                d = "none";
                document.getElementById('comments_sh').innerHTML = 'show';
        } else {
                d = "block";
                document.getElementById('comments_sh').innerHTML = 'hide';
        }
        a.style.display = d;
        document.cookie="comments_table="+d+"; path=/;";
}

if( GetCookie('comments_table') == 'none' ){
        document.getElementById('comments_sh').innerHTML = 'show';
        document.getElementById('comments_table').style.display = 'hide';
}

-->
</script>


			<!-- google_ad_section_end -->
			</div>
			<table width="100%">
                <tbody><tr>
                <td colspan="2" height="20px"></td>
        </tr>
        <form method="post" action="/comment/KGSS/add/"></form>
        <tr> <td style="" colspan="2">Leave a Comment</td> </tr>
        <tr>
                <td valign="top"></td>
                <td><textarea name="content" rows="3" class="form-control"></textarea></td>
        </tr>
        <tr>
                <td colspan="2" style=""><br>
                        <input type="submit" value="Publish" class="btn btn-default">
                        <input type="hidden" name="pcode" value="KGSS">
                </td>
        </tr>
<tr>
<td colspan="2" style="padding-left:5px; color: #999;">
<br>
Notes:
<br>1. Don't post any source code here.
<br>2. Please be careful, leave short comments only. Don't spam here.
<br>3. For more discussion (hints, ideas, solutions) please visit our <a href="/forum">forum</a>.
<br>4. Authors of the problems are allowed to delete the post and use html code here (e.g. to provide some useful links).
</td>
</tr>
        
        </tbody></table>
<br>