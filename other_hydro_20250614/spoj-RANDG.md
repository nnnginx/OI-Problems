<p style="margin-bottom: 0in; text-align: center"><span style="text-decoration: underline;"><strong><span style="font-size: small;"><span style="font-family: ">Red &amp; Green</span></span></strong></span><span style="text-decoration: underline;"><strong><span style="font-size: small;"><span style="font-family: ">&nbsp;</span></span></strong></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in"><span style="font-size: small;"><span style="font-family: ">&nbsp;</span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="font-size: small;"><span style="font-family: ">You have several squares arranged in a single row. Each square is currently painted red or green. You can choose any of the squares and paint it over with either color. The goal is that, after painting, every red square is further to the left than any of the green squares. We want you to do it repainting the minimum possible number of squares.</span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="font-size: small;"><span style="font-family: ">Squares are numbered from left to right. You will be given the initial arrangement as a String, such that character i is 'R' if square i is red or 'G' if square i is green. Print the minimum number of repaints needed to achieve the goal.</span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal">&nbsp;</p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="text-decoration: underline;"><span style="font-size: small;"><span style="font-family: ">Input</span></span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="font-size: small;"><span style="font-family: ">There will be several test cases. Each test case will contain a string of not more than 50 characters on a separate line. Input is terminated by EOF.</span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="text-decoration: underline;"><span style="font-size: small;"><span style="font-family: ">Output</span></span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="font-size: small;"><span style="font-family: ">For each test case, print the output on a separate line.</span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal">&nbsp;</p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="text-decoration: underline;"><span style="font-size: small;"><span style="font-family: ">Constraints</span></span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="font-size: small;"><span style="font-family: ">-Input will contain between 1 and 50 characters, inclusive.</span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="font-size: small;"><span style="font-family: ">-Each character of input will be either 'R' or 'G'.</span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal">&nbsp;</p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="text-decoration: underline;"><span style="font-size: small;"><span style="font-family: ">Sample Input</span></span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="font-size: small;"><span style="font-family: ">RGRGR</span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="font-size: small;"><span style="font-family: ">RRRGGGGG</span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="font-size: small;"><span style="font-family: ">GGGGRRR</span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="font-size: small;"><span style="font-family: ">RGRGRGRGRGRGRGRGR</span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="text-decoration: underline;"><span style="font-size: small;"><span style="font-family: ">Sample Output</span></span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="font-size: small;"><span style="font-family: ">2</span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="font-size: small;"><span style="font-family: ">0</span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="font-size: small;"><span style="font-family: ">3</span></span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="font-size: small;"><span style="font-family: ">8</span></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="font-family: "><br></span></p>
<p style="margin-bottom: 0in; font-weight: normal"><span style="font-size: small;"><span style="font-family: ">Solution &amp; Dataset : Bidhan Roy&nbsp;</span></span></p>