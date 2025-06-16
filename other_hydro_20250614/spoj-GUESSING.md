<p>Here is the rule of the game:
	The computer generates a number from 000000 to 999999, 
	and you should guess the number.<br>
	</p><p>Everytime, the computer will tell you the count of all i from 0..5 that guess[i]==target[i] (A).
	And the count of all (i,j) from (0..5,0..5) that guess[i]==target[j]&amp;&amp;i!=j (B).<br>
	</p><p>If you find a bug, please contact me. <br>

<noscript>please enable the javascript support. </noscript>
<script language="javascript">
function gogogo() {
	if(!(/^[0-9]{6}$/.test(Text1.value))) {
		alert("Format ERROR!!");
	} else {
		self.location = "/problems/GUESSING/179058" + Text1.value;
	}
}
</script>
</p><h3>
<p><input type="text" id="Text1" size="6" maxlength="6" value="000000">
</p><p><input type="submit" id="Submit1" size="6" value="submit" onclick="gogogo()">

</p></h3>