<p>Dr. Whooves has been holed up in his laboratory, analyzing radio transmissions.  Specifically, he has been listening to a very odd transmission - it is just somepony reading a bunch of numbers!  There are several of these stations, and Dr. Whooves wants to know what they are trying to hide.  He is going to try to decrypt the messsages, and after a lot of study, he has discovered a special number N for each transmission, which will let him discover the true message.
	
	He knows that numbers correspond to letters in exactly the following way: a = 1, b = 2, c = 3, ..., z = 26.
	So for a message, there are many possible decodings, just based off of that.  This is where the special number comes in.  If Dr. Whooves sorts all the possible decodings lexicographically, then the secret message is the Nth lexicographic decoding.
	For a given input, output the Nth lexicographic decoding.
	
	However, Dr. Whooves realized that he can't type very quickly, so you'll have to make the program yourself.

</p><h3>Input Format</h3>
<p>An integer T, followed by T lines of the form
	S N
	where S is a string of digits, and N is an integer for which you are to report the Nth lexicographic possibility.
	You are guaranteed that S can be parsed in at least 1 way, and that N is a valid number.  That is, if there are only 5 ways to 
	parse S, then N will be between 1 and 5.
	
	It is further guaranteed that the total number of ways to parse S will fit into a 64 bit signed integer, and that the length of S will
	be less than or equal to 100.

</p><h3>Output Format</h3>
<p>On T separate lines, output the N_i'th lexicographic valid string.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
1111 4
1111 5

<b>Output:</b>
kaa
kk
</pre>