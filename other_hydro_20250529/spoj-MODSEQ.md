<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">Nevest has a sequence <strong>A</strong> with <strong>N</strong> distinct elements. She wants to have a sequence <strong>S</strong> with length <strong>M</strong> and all of the conditions below must be fulfilled:</p>
<ul style="font-family: 'Ubuntu', sans-serif; font-size: 14px; padding-inline-start: 35px;">
<li style="margin: 2px; padding: 1px;">For all subarrays in <strong>S</strong> of length <strong>K</strong>, the sum of each number in the subarray must be divisible by <strong>K</strong>.</li>
<li style="margin: 2px; padding: 1px;">For&nbsp;<strong>1 ¡Ü i &lt; j ¡Ü M</strong>, <strong>S<sub>i</sub> ¡Ù S<sub>j</sub></strong> must hold.</li>
<li style="margin: 2px; padding: 1px;"><strong>A</strong> must be a subsequence of <strong>S</strong>.</li>
<li style="margin: 2px; padding: 1px;">For&nbsp;<strong>1 ¡Ü i ¡Ü M</strong>, constrain <strong>1 ¡Ü S<sub>i</sub> ¡Ü  5 ¡Á 10<sup>5</sup></strong> must be fulfilled.</li>
<li style="margin: 2px; padding: 1px;">The length of sequence <strong>S</strong>&nbsp;mustn't exceed <strong>5 ¡Á 10<sup>5</sup></strong>.</li>
</ul>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">Nevest is not very good at problem-solving so she asked you instead. Help Nevest by giving her any valid sequence or print "-1" if no valid sequence exist (without quotation marks).</p>
<p style="font-family: helvetica; font-size: 14px;"><strong>Please note that you don't have to minimize M.</strong></p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Input Format</strong></p>
<p style="font-family: Menlo,Monaco,Consolas,Courier New,monospace; border: 2px solid #ccc; border-radius: 5px; padding: 10px; font-size: 13px;">N K<br> A<sub>1</sub> A<sub>2</sub> ... A<sub>N</sub></p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Output Format</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">If there's a valid answer, print <strong>M</strong> in the first line followed by a line containing sequence <strong>S</strong> with <strong>M</strong> numbers. If there's no valid sequence <strong>S</strong> print "-1" (without quotation marks).</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Sample Input 1</strong></p>
<p style="font-family: Menlo,Monaco,Consolas,Courier New,monospace; border: 2px solid #ccc; border-radius: 5px; padding: 10px; font-size: 13px;">5 3<br> 1 3 2 5 4</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Sample Output 1</strong></p>
<p style="font-family: Menlo,Monaco,Consolas,Courier New,monospace; border: 2px solid #ccc; border-radius: 5px; padding: 10px; font-size: 13px;">7<br> 1 3 2 7 9 5 4</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Sample Input 2</strong></p>
<p style="font-family: Menlo,Monaco,Consolas,Courier New,monospace; border: 2px solid #ccc; border-radius: 5px; padding: 10px; font-size: 13px;">4 2<br> 1 3 5 7</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Sample Output 2</strong></p>
<p style="font-family: Menlo,Monaco,Consolas,Courier New,monospace; border: 2px solid #ccc; border-radius: 5px; padding: 10px; font-size: 13px;">4<br> 1 3 5 7</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Constraints</strong></p>
<ul style="font-family: 'Ubuntu', sans-serif; font-size: 14px; padding-inline-start: 25px;">
<li style="margin: 2px; padding: 1px;">1 ¡Ü K ¡Ü N ¡Ü 500</li>
<li style="margin: 2px; padding: 1px;">1 ¡Ü A<sub>i</sub> ¡Ü 500</li>
<li style="margin: 2px; padding: 1px;">A<sub>i</sub> ¡Ù A<sub>j</sub>, for 1 ¡Ü i &lt; j ¡Ü N</li>
</ul>