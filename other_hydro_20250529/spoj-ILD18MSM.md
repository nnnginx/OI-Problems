<p style="font-size: 16px; border: 0px; font-family: OpenSans; font-stretch: inherit; line-height: 1.5em; margin: 12px 0px 1em; outline: 0px; padding: 0px; vertical-align: baseline; word-wrap: break-word; word-break: break-word; caret-color: #39424e; color: #39424e;">We have two strings A and B which are permutations of the same set of characters. We need to change these strings to obtain two identical strings by performing the following operations:</p>
<p style="font-size: 16px; border: 0px; font-family: OpenSans; font-stretch: inherit; line-height: 1.5em; margin: 12px 0px 1em; outline: 0px; padding: 0px; vertical-align: baseline; word-wrap: break-word; word-break: break-word; caret-color: #39424e; color: #39424e;">1) swap two consecutive characters of a string</p>
<p style="font-size: 16px; border: 0px; font-family: OpenSans; font-stretch: inherit; line-height: 1.5em; margin: 12px 0px 1em; outline: 0px; padding: 0px; vertical-align: baseline; word-wrap: break-word; word-break: break-word; caret-color: #39424e; color: #39424e;">2) swap the first and the last characters of a string</p>
<p style="font-size: 16px; border: 0px; font-family: OpenSans; font-stretch: inherit; line-height: 1.5em; margin: 12px 0px 1em; outline: 0px; padding: 0px; vertical-align: baseline; word-wrap: break-word; word-break: break-word; caret-color: #39424e; color: #39424e;">The operation can be performed on either string. Return the minimum number of moves that we need in order to obtain two equal strings?</p>
<div style="font-size: 16px; border: 0px; font-family: OpenSans; font-stretch: inherit; line-height: inherit; margin: 0px 0px 10px; outline: 0px; padding: 0px; vertical-align: baseline; word-wrap: break-word; word-break: break-word; caret-color: #39424e; color: #39424e;">
<p style="border: 0px; font-style: inherit; font-variant-caps: inherit; font-stretch: inherit; line-height: 1.5em; margin: 0px 0px 1em; outline: 0px; padding: 0px; vertical-align: baseline; word-wrap: break-word; word-break: break-word;"><strong>Constraints</strong></p>
</div>
<div style="font-size: 16px; border: 0px; font-family: OpenSans; font-stretch: inherit; line-height: inherit; margin: 0px 0px 10px; outline: 0px; padding: 0px; vertical-align: baseline; word-wrap: break-word; word-break: break-word; caret-color: #39424e; color: #39424e;">
<div style="border: 0px; font-style: inherit; font-variant-caps: inherit; font-stretch: inherit; line-height: inherit; margin: 0px; outline: 0px; padding: 0px; vertical-align: baseline; word-wrap: break-word; word-break: break-word;">
<p style="border: 0px; font-style: inherit; font-variant-caps: inherit; font-stretch: inherit; line-height: 1.5em; margin: 12px 0px 1em; outline: 0px; padding: 0px; vertical-align: baseline; word-wrap: break-word; word-break: break-word;">1 &lt; length(A) = length(B) ¡Ü 2,000</p>
<p style="border: 0px; font-style: inherit; font-variant-caps: inherit; font-stretch: inherit; line-height: 1.5em; margin: 12px 0px 1em; outline: 0px; padding: 0px; vertical-align: baseline; word-wrap: break-word; word-break: break-word;">All the input characters are between 'a' and 'z'</p>
<p style="border: 0px; font-style: inherit; font-variant-caps: inherit; font-stretch: inherit; line-height: 1.5em; margin: 12px 0px 1em; outline: 0px; padding: 0px; vertical-align: baseline; word-wrap: break-word; word-break: break-word;">The count of each distinct character in A is identical to the count of the same character in B.</p>
</div>
</div>
<h3>Input</h3>
<p>First line: String A.</p>
<p>Second line: String B.</p>
<h3>Output</h3>
<p>Minimum number of moves.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
aab</pre>
<pre>baa

<strong>Output:</strong>
1</pre>