<p>Byteasar has had a new palace built. It consists of N&nbsp;chambers and N-1&nbsp;corridors connecting them. Each corridor connects exactly two chambers. The rooms are numbered from 1&nbsp;to N. There is only a single entrance to the palace, which leads to chamber no. 1. For each chamber there is exactly one route leading to it from the entrance, without turning back on the way. In other words, the chambers and the corridors form a&nbsp;<em>tree</em>&nbsp;- a connected acyclic graph.</p>
<p>The fire marshal who is to approve the building demands placing fire extinguishers inside. The following are his exact requirements:</p>
<ul>
<li>The fire extinguishers should be placed in (some) chambers, and one chamber may store any number of extinguishers.</li>
<li>Each chamber has to be assigned one fire extinguisher, though it may be stored in another chamber.</li>
<li>Each fire extinguisher can be assigned to at most S&nbsp;different chambers.</li>
<li>For each room its assigned extinguisher is within the range of K&nbsp;corridors.</li>
</ul>
<p>Byteasar has a week spot for lavish palaces, so it is no surprise he has very little money now, right after completion of another splendid palace. Therefore he is interested in the minimum number of fire extinguishers sufficient for satisfying fire marshal's demands.</p>
<p>&nbsp;</p>
<h2>Input</h2>
<p>The first line of the standard input contains three integers N, S&nbsp;and K&nbsp;separated by single spaces, 1 &lt;= N &lt;= 100000, 1 &lt;= S &lt;= N, 1 &lt;= K &lt;= 20. Each of the following N-1&nbsp;lines holds two integers separated by a single space. Line no. i+1&nbsp;contains the numbers X<sub>i</sub> Y<sub>i</sub>&nbsp;denoting the corridor connecting chambers no. X<sub>i</sub>&nbsp;and Y<sub>i</sub>.</p>
<h2>Output</h2>
<p>The first and only line of the standard output is to hold one integer - the minimum number of fire extinguishers that have to be installed in palace.</p>
<h2>Example</h2>
<p>For the input data:</p>
<pre>12 3 1
1 12
3 8
7 8
8 9
2 12
10 12
9 12
4 8
5 8
8 11
6 8
</pre>
<p>the correct result is:</p>
<pre>4</pre>

<p>
</p><div align="center"><img style="width: 50%; height: 50%" title="Image" src="../../content/francky:stc01" alt="Image">
 <p></p>
</div>

<div class="text-center">
	<a href="/submit/STC01/" class="btn btn-primary btn-lg"><i class="fa fa-send"></i> Submit solution!</a>
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
			<img src="file://1rNWaoCz.png">
		</td>
		<td class="comm comm_odd">
			<a href="/users/krist7599555">krist7599555</a>: 
								<span style="font-size: 10px; color: #666;">2017-05-18 15:20:25</span>
		<br>
				<p>picture
<br>http://main.edu.pl/en/archive/oi/16/gas
<br>=(Francky)=&gt; Thanks. Added in body, no copyright infringement intended. To be removed if need.</p>
				<b>Last edit: 2017-05-18 16:28:15</b>
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
        <form method="post" action="/comment/STC01/add/"></form>
        <tr> <td style="" colspan="2">Leave a Comment</td> </tr>
        <tr>
                <td valign="top"></td>
                <td><textarea name="content" rows="3" class="form-control"></textarea></td>
        </tr>
        <tr>
                <td colspan="2" style=""><br>
                        <input type="submit" value="Publish" class="btn btn-default">
                        <input type="hidden" name="pcode" value="STC01">
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