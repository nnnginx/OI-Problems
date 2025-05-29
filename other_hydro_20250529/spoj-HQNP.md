<p>HQ9+ is an esoteric programming language specialized for certain tasks. For example, printing “Hello,world!” or writing a quine (a program that prints itself) couldn’t be any simpler. Unfortunately, HQ9+&nbsp;doesn’t do very well in most other situations. This is why we have created our own variant of the language,HQ0-9+−INCOMPUTABLE?!.A HQ0-9+−INCOMPUTABLE?! program is a sequence of commands, written on one line without&nbsp;any whitespace (except for the trailing newline). The program can store data in two memory areas: the&nbsp;buffer, a string of characters, and the accumulator, an integer variable. Initially, the buffer is empty&nbsp;and the accumulator is set to 0. The value of the buffer after executing all the commands becomes the&nbsp;program’s output.</p>
<div>
<div style="text-align: -webkit-auto;">
<div>
<div>&nbsp; &nbsp;</div>
<div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; HQ0-9+−INCOMPUTABLE?! supports the following commands:</div>
</div>
<table id="TBL-1" class="tabular" style="font-size: medium; background-color: #fafad2; border-collapse: collapse; margin-left: auto; margin-right: auto; border-left-style: solid; border-left-color: black; border-left-width: 0.4pt; border-right-style: solid; border-right-color: black; border-right-width: 0.4pt;" border="0" cellspacing="0" cellpadding="0" rules="groups">
<colgroup id="TBL-1-1g"><col id="TBL-1-1"></colgroup><colgroup id="TBL-1-2g"><col id="TBL-1-2"></colgroup> 
<tbody>
<tr id="TBL-1-1-" style="vertical-align: baseline;">
<th id="TBL-1-1-1" class="td11" style="background-color: #191970; color: #fafad2; padding-top: 2px; padding-bottom: 2px; white-space: nowrap; padding-left: 5px; padding-right: 5px; text-align: right; margin: 0px;">command</th><th id="TBL-1-1-2" class="td11" style="background-color: #191970; color: #fafad2; padding-top: 2px; padding-bottom: 2px; white-space: nowrap; padding-left: 5px; padding-right: 5px; text-align: left; margin: 0px;">description</th>
</tr>
<tr id="TBL-1-2-" style="vertical-align: baseline;">
<td id="TBL-1-2-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">h</span>,&nbsp;<span class="cmtt-10" style="font-family: monospace;">H</span></td>
<td id="TBL-1-2-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">appends&nbsp;<span class="cmtt-10" style="font-family: monospace;">helloworld&nbsp;</span>to the buffer</p>
</td>
</tr>
<tr id="TBL-1-3-" style="vertical-align: baseline;">
<td id="TBL-1-3-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">q</span>,&nbsp;<span class="cmtt-10" style="font-family: monospace;">Q</span></td>
<td id="TBL-1-3-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">appends the program source code to the buffer (not including the trailing newline)</p>
</td>
</tr>
<tr id="TBL-1-4-" style="vertical-align: baseline;">
<td id="TBL-1-4-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">0-9</span></td>
<td id="TBL-1-4-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">replaces the buffer with&nbsp;<span class="cmmi-10" style="font-style: italic;">n&nbsp;</span>copies of its old value – for example, ‘<span class="cmtt-10" style="font-family: monospace;">2</span>’ doubles the buffer</p>
</td>
</tr>
<tr id="TBL-1-5-" style="vertical-align: baseline;">
<td id="TBL-1-5-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">+</span></td>
<td id="TBL-1-5-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">increments the accumulator</p>
</td>
</tr>
<tr id="TBL-1-6-" style="vertical-align: baseline;">
<td id="TBL-1-6-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">-</span></td>
<td id="TBL-1-6-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">decrements the accumulator</p>
</td>
</tr>
<tr id="TBL-1-7-" style="vertical-align: baseline;">
<td id="TBL-1-7-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">i</span>,&nbsp;<span class="cmtt-10" style="font-family: monospace;">I</span></td>
<td id="TBL-1-7-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">increments the ASCII value of every character in the buffer</p>
</td>
</tr>
<tr id="TBL-1-8-" style="vertical-align: baseline;">
<td id="TBL-1-8-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">n</span>,&nbsp;<span class="cmtt-10" style="font-family: monospace;">N</span></td>
<td id="TBL-1-8-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">applies ROT13 to the letters and numbers in the buffer (for letters ROT13 preserves case; for digits we define ROT13(<span class="cmmi-10" style="font-style: italic;">d</span>) = (<span class="cmmi-10" style="font-style: italic;">d&nbsp;</span>+ 13) mod 10)</p>
</td>
</tr>
<tr id="TBL-1-9-" style="vertical-align: baseline;">
<td id="TBL-1-9-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">c</span>,&nbsp;<span class="cmtt-10" style="font-family: monospace;">C</span></td>
<td id="TBL-1-9-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">swaps the case of every letter in the buffer; doesn’t change other characters</p>
</td>
</tr>
<tr id="TBL-1-10-" style="vertical-align: baseline;">
<td id="TBL-1-10-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">o</span>,&nbsp;<span class="cmtt-10" style="font-family: monospace;">O</span></td>
<td id="TBL-1-10-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">removes all characters from the buffer such that their index, counted from the end, is a prime or a power of two (or both); the last character has index 1 (which is a power of 2)</p>
</td>
</tr>
<tr id="TBL-1-11-" style="vertical-align: baseline;">
<td id="TBL-1-11-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">m</span>,&nbsp;<span class="cmtt-10" style="font-family: monospace;">M</span></td>
<td id="TBL-1-11-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">sets the accumulator to the current buffer length</p>
</td>
</tr>
<tr id="TBL-1-12-" style="vertical-align: baseline;">
<td id="TBL-1-12-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">p</span>,&nbsp;<span class="cmtt-10" style="font-family: monospace;">P</span></td>
<td id="TBL-1-12-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">removes all characters from the buffer such that their index is a prime or a power of two (or both); the first character has index 1 (which is a power of 2)</p>
</td>
</tr>
<tr id="TBL-1-13-" style="vertical-align: baseline;">
<td id="TBL-1-13-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">u</span>,&nbsp;<span class="cmtt-10" style="font-family: monospace;">U</span></td>
<td id="TBL-1-13-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">converts the buffer to uppercase</p>
</td>
</tr>
<tr id="TBL-1-14-" style="vertical-align: baseline;">
<td id="TBL-1-14-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">t</span>,&nbsp;<span class="cmtt-10" style="font-family: monospace;">T</span></td>
<td id="TBL-1-14-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">sorts the characters in the buffer by their ASCII values</p>
</td>
</tr>
<tr id="TBL-1-15-" style="vertical-align: baseline;">
<td id="TBL-1-15-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">a</span>,&nbsp;<span class="cmtt-10" style="font-family: monospace;">A</span></td>
<td id="TBL-1-15-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">replaces every character in the buffer with its ASCII value in decimal (1–3 digits)</p>
</td>
</tr>
<tr id="TBL-1-16-" style="vertical-align: baseline;">
<td id="TBL-1-16-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">b</span>,&nbsp;<span class="cmtt-10" style="font-family: monospace;">B</span></td>
<td id="TBL-1-16-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">replaces every character in the buffer with its ASCII value in binary (exactly eight ‘0’/‘1’ characters)</p>
</td>
</tr>
<tr id="TBL-1-17-" style="vertical-align: baseline;">
<td id="TBL-1-17-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">l</span>,&nbsp;<span class="cmtt-10" style="font-family: monospace;">L</span></td>
<td id="TBL-1-17-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">converts the buffer to lowercase</p>
</td>
</tr>
<tr id="TBL-1-18-" style="vertical-align: baseline;">
<td id="TBL-1-18-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">e</span>,&nbsp;<span class="cmtt-10" style="font-family: monospace;">E</span></td>
<td id="TBL-1-18-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">translates every character in the buffer to l33t using the following table:&nbsp;<br><span class="cmtt-10" style="font-family: monospace;">ABCDEFGHIJKLMNOPQRSTUVWXYZ abcdefghijklmnopqrstuvwxyz 0123456789</span>&nbsp;<br><span class="cmtt-10" style="font-family: monospace;">48(03=6#|JXLM~09Q257UVW%Y2 a6&lt;d3f9hijk1m^0p9r57uvw*y2 O!ZEA$G/B9</span></p>
</td>
</tr>
<tr id="TBL-1-19-" style="vertical-align: baseline;">
<td id="TBL-1-19-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">?</span></td>
<td id="TBL-1-19-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">removes 47 characters from the end of the buffer (or everything if it is too short)</p>
</td>
</tr>
<tr id="TBL-1-20-" style="vertical-align: baseline;">
<td id="TBL-1-20-1" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; white-space: nowrap; text-align: right; border-color: #dadab2;"><span class="cmtt-10" style="font-family: monospace;">!</span></td>
<td id="TBL-1-20-2" class="td11" style="padding-left: 5pt; padding-right: 5pt; border-top-style: solid; border-right-style: none; border-bottom-style: solid; border-left-style: none; border-top-width: 1px; border-right-width: 0px; border-bottom-width: 1px; border-left-width: 0px; text-align: left; border-color: #dadab2;">
<p class="noindent" style="text-align: justify; margin-top: 0em; margin-bottom: 0em; margin-left: 0px; text-indent: 0em;">removes 47 characters from the beginning of the buffer (or everything if it is too short)</p>
</td>
</tr>
</tbody>
</table>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">command &nbsp;description</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;appends helloworld to the buffer</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; h, H</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;appends the program source code to the buffer (not including the trailing newline)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; q, Q</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;replaces the buffer with n copies of its old value – for example, ‘2’ doubles the buffer</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; 0-9</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;increments the accumulator</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp;+</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;decrements the accumulator</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp;-</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;increments the ASCII value of every character in the buffer</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; i, I</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;applies ROT13 to the letters and numbers in the buffer (for letters ROT13 preserves</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; n, N</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;case; for digits we define ROT13(d) = (d + 13) mod 10)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;swaps the case of every letter in the buffer; doesn’t change other characters</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; c, C</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;removes all characters from the buffer such that their index, counted from the end, is a</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; o, O</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;prime or a power of two (or both); the last character has index 1 (which is a power of 2)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;sets the accumulator to the current buffer length</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; m, M</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;removes all characters from the buffer such that their index is a prime or a power of two</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; p, P</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;(or both); the first character has index 1 (which is a power of 2)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;converts the buffer to uppercase</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; u, U</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;sorts the characters in the buffer by their ASCII values</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; t, T</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;replaces every character in the buffer with its ASCII value in decimal (1–3 digits)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; a, A</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;replaces every character in the buffer with its ASCII value in binary (exactly eight ‘0’/‘1’</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; b, B</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;characters)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;converts the buffer to lowercase</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; l, L</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;translates every character in the buffer to l33t using the following table:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; e, E</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;ABCDEFGHIJKLMNOPQRSTUVWXYZ abcdefghijklmnopqrstuvwxyz 0123456789</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;48(03=6#|JXLM~09Q257UVW%Y2 a6&lt;d3f9hijk1m^0p9r57uvw*y2 O!ZEA$G/B9</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;removes 47 characters from the end of the buffer (or everything if it is too short)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp;?</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;removes 47 characters from the beginning of the buffer (or everything if it is too short)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp; &nbsp; &nbsp; &nbsp;!</div>
</div>
</div>
<p>In this task you have to print the&nbsp;HQ0-9+−INCOMPUTABLE?! program that will give the number n as output.</p>
<p class="noindent"><strong><span class="cmssbx-10">Limits</span></strong></p>
<p>Any HQ0-9+−INCOMPUTABLE?! program( output for each case ) must be at most 10<span class="thinspace" style="margin-left: 0.3em;">&nbsp;</span>000 commands long. The accumulator is unbounded (it can store an arbitrarily large integer). After each command, the buffer must be at most 10<span class="thinspace" style="margin-left: 0.3em;">&nbsp;</span>000 characters long. To prevent code injection vulnerabilities, during the execution of your program( output for each case ) <span class="cmti-10">the buffer must never contain</span> <span class="cmti-10">non-alphanumeric characters</span>, i.e. characters other than <span class="cmtt-10">A-Z</span>, <span class="cmtt-10">a-z</span>, and <span class="cmtt-10">0-9</span>. If it happens, your solution will be judged as wrong.</p>
<p>&nbsp;</p>
<h3>&nbsp;&nbsp; Input</h3>
<p>First line has integer T i.e number of test cases. ( T &lt;= 100 ). Next T lines has a number n. ( 0 &lt;= n &lt;= 10^100 )</p>
<p>&nbsp;</p>
<h3>&nbsp;&nbsp; Output</h3>
<p>For each n, output the required HQ0-9+−INCOMPUTABLE?! program which will give n as output. If there are multiple solutions, output any one of them. Output of each test case must be in a single line.</p>
<h3>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</h3>
<h3>&nbsp;&nbsp; Example</h3>
<p><strong>Input:</strong></p>
<p>3</p>
<p>0</p>
<p>321</p>
<p>4124144</p>
<p><strong>Output:</strong></p>
<p>Find yourself :)</p>
<p>&nbsp;</p>
<p class="noindent"><strong>Following are some HQ0-9+−INCOMPUTABLE?! programs and their corresponding outputs:</strong></p>
<table id="TBL-2" class="tabular" border="0" cellspacing="0" cellpadding="0" rules="groups">
<tbody>
<tr id="TBL-2-2-" style="vertical-align: baseline;">
<td id="TBL-2-2-1" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">h5! </span></td>
<td id="TBL-2-2-2" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">&nbsp;rld </span></td>
</tr>
<tr id="TBL-2-3-" style="vertical-align: baseline;">
<td id="TBL-2-3-1" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">QCq </span></td>
<td id="TBL-2-3-2" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">&nbsp;qcQQCq</span></td>
</tr>
<tr id="TBL-2-4-" style="vertical-align: baseline;">
<td id="TBL-2-4-1" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">q23 </span></td>
<td id="TBL-2-4-2" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">&nbsp;q23q23q23q23q23q23 </span></td>
</tr>
<tr id="TBL-2-5-" style="vertical-align: baseline;">
<td id="TBL-2-5-1" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">h?h </span></td>
<td id="TBL-2-5-2" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">&nbsp;helloworld </span></td>
</tr>
<tr id="TBL-2-6-" style="vertical-align: baseline;">
<td id="TBL-2-6-1" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">H2O </span></td>
<td id="TBL-2-6-2" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">&nbsp;hlwolheo</span></td>
</tr>
<tr id="TBL-2-7-" style="vertical-align: baseline;">
<td id="TBL-2-7-1" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">h4op </span></td>
<td id="TBL-2-7-2" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">&nbsp;ollwldwlhe </span></td>
</tr>
<tr id="TBL-2-8-" style="vertical-align: baseline;">
<td id="TBL-2-8-1" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">hint </span></td>
<td id="TBL-2-8-2" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">&nbsp;ccfkrsvzzz </span></td>
</tr>
<tr id="TBL-2-9-" style="vertical-align: baseline;">
<td id="TBL-2-9-1" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">q18N </span></td>
<td id="TBL-2-9-2" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">&nbsp;d41Ad41Ad41Ad41Ad41Ad41Ad41Ad41A</span></td>
</tr>
<tr id="TBL-2-10-" style="vertical-align: baseline;">
<td id="TBL-2-10-1" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">3QAh </span></td>
<td id="TBL-2-10-2" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">&nbsp;518165104helloworld </span></td>
</tr>
<tr id="TBL-2-11-" style="vertical-align: baseline;">
<td id="TBL-2-11-1" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">Qb </span></td>
<td id="TBL-2-11-2" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">&nbsp;0101000101100010 </span></td>
</tr>
<tr id="TBL-2-12-" style="vertical-align: baseline;">
<td id="TBL-2-12-1" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">opaque </span></td>
<td id="TBL-2-12-2" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">&nbsp;094QU3 </span></td>
</tr>
<tr id="TBL-2-13-" style="vertical-align: baseline;">
<td id="TBL-2-13-1" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">h1Qt </span></td>
<td id="TBL-2-13-2" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">&nbsp;1Qdehhllloortw </span></td>
</tr>
<tr id="TBL-2-14-" style="vertical-align: baseline;">
<td id="TBL-2-14-1" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">H9999&nbsp; <br></span></td>
<td id="TBL-2-14-2" class="td11" style="white-space: nowrap; text-align: left;">&nbsp;(error: buffer size exceeded 10<span class="thinspace" style="margin-left: 0.3em;">&nbsp;</span>000)</td>
</tr>
<tr id="TBL-2-15-" style="vertical-align: baseline;">
<td id="TBL-2-15-1" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">quine </span></td>
<td id="TBL-2-15-2" class="td11" style="white-space: nowrap; text-align: left;">&nbsp;(error: buffer contains “<span class="obeylines-h"><span class="verb"><span class="cmtt-10">|</span></span></span>”)</td>
</tr>
<tr id="TBL-2-16-" style="vertical-align: baseline;">
<td id="TBL-2-16-1" class="td11" style="white-space: nowrap; text-align: left;"><span class="cmtt-10">LMAO </span></td>
<td id="TBL-2-16-2" class="td11" style="white-space: nowrap; text-align: left;">
<p>&nbsp;(empty output)</p>
<p>&nbsp;</p>
</td>
</tr>
</tbody>
</table>