<p><span style="font-family: verdana, geneva;">Chances are that you have probably already heard of the travelling salesman problem. If you have, then you are&nbsp;</span><span style="font-family: verdana, geneva;">aware that it is an NP-hard problem because it lacks an efficient solution. Well, this task is an uncommon version&nbsp;</span><span style="font-family: verdana, geneva;">of the famous problem! Its uncommonness derives from the fact that this version is, actually, solvable efficiently.&nbsp;</span></p>
<p><span style="font-family: verdana, geneva;"><br></span></p>
<p><span style="font-family: verdana, geneva;">The travelling salesman is on a mission to visit N cities, each exactly once. The cities are represented by numbers&nbsp;</span><span style="font-family: verdana, geneva;">1, 2, ..., N. What we know is the direct flight duration between each pair of cities. The salesman, being the efficient&nbsp;</span><span style="font-family: verdana, geneva;">man that he is, wants to modify the city visiting sequence so that the total flight duration is the minimum&nbsp;</span><span style="font-family: verdana, geneva;">possible.&nbsp;</span></p>
<p><span style="font-family: verdana, geneva;">Alas, all is not so simple. In addition, the salesman has a peculiar condition regarding the sequence. For each city&nbsp;</span><span style="font-family: verdana, geneva;">labeled K must apply: either all cities with labels smaller than K have been visited before the city labeled K or they&nbsp;</span><span style="font-family: verdana, geneva;">will all be visited after the city labeled K. In other words, the situation when one of such cities is visited before, and&nbsp;</span><span style="font-family: verdana, geneva;">the other after is not allowed.&nbsp;</span></p>
<p><span style="font-family: verdana, geneva;">Assist the poor fellow in his ambitious mission and calculate the minimum total flight duration needed in order to&nbsp;</span><span style="font-family: verdana, geneva;">travel to all the cities, starting from whichever and ending in whichever city, visiting every city exactly once, so that&nbsp;</span><span style="font-family: verdana, geneva;">his peculiar request is fulfilled.&nbsp;</span></p>
<p><span style="font-family: verdana, geneva;"><br></span></p>
<h3><span style="font-family: verdana, geneva;">Input</span></h3>
<p><span style="font-family: verdana, geneva;">The first line of input contains the positive integer N (2 ¡Ü N ¡Ü 1500), the number of cities. </span><span style="font-family: verdana, geneva;">Each of the following N lines contains N positive integers from the interval [0, 1000]. The number in B</span><sup>th</sup><span style="font-family: verdana, geneva;"> place in&nbsp;</span><span style="font-family: verdana, geneva;">the A</span><sup>th</sup><span style="font-family: verdana, geneva;"> row represents the flight duration between cities A and B; that number is equal to the A</span><sup>th</sup><span style="font-family: verdana, geneva;"> number in the&nbsp;</span><span style="font-family: verdana, geneva;">B</span><sup>th</sup><span style="font-family: verdana, geneva;"> row. When A = B, that number is 0. Otherwise, it is a positive value.</span></p>
<p><span style="font-family: verdana, geneva;"><br></span></p>
<h3><span style="font-family: verdana, geneva;">Output</span></h3>
<p><span style="font-family: verdana, geneva;">The first and only line of output must contain the required minimum total flight duration.&nbsp;</span></p>
<p><span style="font-family: verdana, geneva;"><br></span></p>
<h3><span style="font-family: verdana, geneva;">Example</span></h3>
<pre><span style="font-family: verdana, geneva;"><strong>Input:</strong>
3 
0 5 2 
5 0 4 
2 4 0 

<strong>Output:</strong>
7<span style="white-space: normal;">
</span></span></pre>
<pre><span style="font-family: verdana, geneva;"><br></span></pre>
<pre><strong><span style="font-family: verdana, geneva;"><strong>Input:</strong></span></strong></pre>
<pre><div id="_mcePaste" style="position: absolute; left: -10000px; top: 463px; width: 1px; height: 1px; overflow: hidden;">4&nbsp;</div></pre>
<pre><span style="font-family: verdana, geneva;">4 
0 15 7 8 
15 0 16 9 
7 16 0 12 
8 9 12 0</span></pre>
<div><strong><span style="font-family: verdana, geneva;"> </span>
<pre style="font-weight: normal;"><strong><span style="font-family: verdana, geneva;"><strong>Output:</strong></span></strong></pre>
<pre style="font-weight: bold;">31</pre>
<pre style="font-weight: bold;"><strong><span style="font-family: verdana, geneva;"><br></span></strong></pre>

<p><b>
Clarification of the first example:<br>
the optimal sequence is 2, 1, 3 or 3, 1, 2. The sequence 1, 3, 2 is even more favorable, but it does not fulfill the salesman's condition.
</b></p>

<p><b>
Clarification of the second example:<br>
the sequence is either 3, 1, 2, 4 or 4, 2, 1, 3.
</b></p>

</strong></div><strong>

<div class="text-center">
	<a href="/submit/PUTNIK/" class="btn btn-primary btn-lg"><i class="fa fa-send"></i> Submit solution!</a>
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
			<img src="file://9HtRx1wz.png">
		</td>
		<td class="comm comm_odd">
			<a href="/users/zukow">:D</a>: 
								<span style="font-size: 10px; color: #666;">2013-11-16 19:21:28</span>
		<br>
				<p>I made small correction to first paragraph. NP-hard problems ARE solvable, just inefficiently.</p>
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
        <form method="post" action="/comment/PUTNIK/add/"></form>
        <tr> <td style="" colspan="2">Leave a Comment</td> </tr>
        <tr>
                <td valign="top"></td>
                <td><textarea name="content" rows="3" class="form-control"></textarea></td>
        </tr>
        <tr>
                <td colspan="2" style=""><br>
                        <input type="submit" value="Publish" class="btn btn-default">
                        <input type="hidden" name="pcode" value="PUTNIK">
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
		</strong>