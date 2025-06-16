<p>You are familiar with greeting cards, right?</p>
<p>On the occasion of EID, Mahir along with his cousins, decided to sell special greeting cards for wishing EID. As per decision, they setted up their small stall. And they started selling. Initially they have <strong>N</strong> Eid cards. There is a serial number of each EID card. The serial number of 1<sup>st</sup> Card is 1, 2<sup>nd&nbsp;</sup>card is 2 and so on. The serial numbers of the EID Cards are written on it.</p>
<p>&nbsp;</p>
<p>Mahir came up with a great pricing idea. As they are looking to make much profit, the price of the EID cards are not fixed. They will fix according to their idea. So let¡¯s describe it.</p>
<p>&nbsp;</p>
<p>Firstly, they will consider two things, the serial number of the card they are selling and the number of cards left before selling current card. And the price of this card will be product of this two.</p>
<p>&nbsp;</p>
<p>Let¡¯s make it straight forward:</p>
<ul>
<li>Consider, they are selling <strong>i<sup>th</sup></strong>&nbsp;card. So the serial number is <strong>i.</strong></li>
<li>And so there will be actually <strong><em>n-i+1</em></strong> cards left before selling this card.</li>
<li>So the price of the card will be <strong>i * (n-i+1).</strong></li>
</ul>
<p>It is guranteed that they will sell all the cards. Your task is to calculate the total income after selling all the cards.</p>
<h3>Input</h3>
<p>The first line of the input contains an integer <strong>T&nbsp;</strong>(<strong><em>1   ¡Ü   T   ¡Ü </em></strong><strong><em> </em></strong><strong><em>1,000)</em></strong>.&nbsp;Each of the following <strong>T</strong> lines will have an integer<strong><em>&nbsp;</em><em>N (</em></strong><strong><em>1   ¡Ü   N   ¡Ü </em></strong><strong><em> 1,000,000,000)</em></strong>&nbsp;.</p>
<h3>Output</h3>
<p>For each case, output a single line consisting of the total income of Mahir modulo <strong><em>1,000,000,007</em></strong>.</p>
<h3>Example</h3>
<h3>Input:</h3>
<p><span style="white-space: normal;">2<br>5<br>10</span></p>
<h3>Output:</h3>
<p><span style="white-space: normal;">35<br>220 </span></p>