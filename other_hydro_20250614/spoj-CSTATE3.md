<p><strong>Note: This is a harder version of CSTATE1 and CSTATE2 - a solution to this problem will (except I/O format) pass there.</strong></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">V Slovakistane sa rozhodli osadníci usporiadať národný šachový turnaj.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Za prvé miesto sa dá získať diplom, a tak všetci hrajú ako o život.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Keďže sa však nehrá na čas, vyskytol sa problém -- hráči nechceli priznať prehru.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Stále len tvrdili, že určite nemajú mat, však určite sa z tej situácie dá nejak dostať, keby len mali ešte chvíľku na rozmýšlanie... A možno ešte jednu...</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Na budúci rok sa bude TMŠ v Slovakistane organizovať zas, ale je potrebné tento problém dovtedy nejako vyriešiť.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">## Úloha</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Pre daný popis šachovnice rozlíšte, či má niektorý z hráčov šach alebo mat.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Pritom berte do úvahy len obyčajné pohyby figúrok (komplikované ťahy ako</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">*rošáda*, *en passant*, *pohyb pešiakom o dva políčka vpred* a</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">*povýšenie pešiaka* sa v Slovakistane neakceptujú).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">## Formát vstupu</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">V prvom riadku je číslo $1 \leq t \leq 1000$, udávajúce počet šachovníc na vstupe.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Nasleduje $t$ popisov šachovníc.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Každý popis šachovnice pozostáva z ôsmich riadkov, každý obsahujúci</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">osem znakov (teda šachovnica má klasické rozmery $8 \times 8$).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Tieto znaky sú `.KQRBHP`, reprezentujúce v tomto poradí voľné</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">políčko, kráľa, kráľovnú, vežu, strelca, koňa, a pešiaka.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Bielemu hráčovi patrí horná strana šachovnice (skôr na vstupe) a jeho</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">figúrky sú označené malými písmenami. Teda bieli pešiaci sa pohybujú</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">smerom dole.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Čiernemu hráčovi patrí dolná strana šachovnice a jeho figúrky sú</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">označené veľkými písmenami. Jeho pešiaci sa pohybujú smerom hore.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Za každým popisom šachovnice je jeden prázdny riadok.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Počet ani poloha figúrok nijak nemusia byť dosiahnuteľné v</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">klasickej hre šachu, avšak môžete predpokladať, že na každej</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">šachovnici sa nachádza práve jeden biely kráľ (`k`) a práve jeden</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">čierny kráľ (`K`).&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Navyše, figúrky sa vo vstupoch budú vyskytovať nasledovne:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">| Číslo sady | Nové figúrky <span style="white-space: pre;"> </span>|</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">| :--------: |------------------|</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">|<span style="white-space: pre;"> </span> &nbsp;$1$<span style="white-space: pre;"> </span> | Kráľ, kôň<span style="white-space: pre;"> </span>|</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">| <span style="white-space: pre;"> </span> &nbsp;$2$<span style="white-space: pre;"> </span> | Veža<span style="white-space: pre;"> </span>|</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">|<span style="white-space: pre;"> </span> &nbsp;$3$<span style="white-space: pre;"> </span> | Strelec, kráľovná|</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">|<span style="white-space: pre;"> </span> &nbsp;$4$<span style="white-space: pre;"> </span> | Pešiak<span style="white-space: pre;"> </span>|</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">## Formát výstupu</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Pre každú šachovnicu vypíšte jeden riadok s jednou z nasledovných hlášok:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">+ &nbsp; "Neutralna situacia.", ak žiaden z kráľov nie je ohrozený nepriateľskou figúrkou.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">+ &nbsp; "Nemozna situacia.", ak sú obaja králi ohrození nepriateľskou figúrkou.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">+ &nbsp; "{farba} hrac ma sach.", kde {farba} je "Biely", resp. "Cierny", ak</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">je kráľ tohto hráča v ohrození, ale existuje platný ťah niektorou</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">z jeho figúrok taký, po ktorom už v ohrození nebude.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">+ &nbsp; "{farba} hrac ma mat.", kde {farba} je "Biely", resp. "Cierny", ak je</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">kráľ tohto hráča v ohrození, a neexistuje platný ťah niektorou z jeho</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">figúrok taký, po ktorom už v ohrození nebude.</div>
<p>&nbsp;</p>
<p>A thousand years ago the inhabitants of Slovakistan decided to organize a national chess tournament.</p>
<p>Since the first place prize was 1 point on SPOJ, everyone played as if their life was at stake.</p>
<p>However, since time was not measured in this chess tournament (unlike at most chess tournaments in the rest of the world), a problem occured - players took way too long to admit defeat.</p>
<p>They always just kept thinking and thinking, trying to find some move which would prevent their king from being taken. Just one more moment... And perhaps one more...</p>
<p>Luckily, a skilled programmer lent them a hand and got rid of this nuisance!</p>
<p>The next year, they organized a chess tournament once more. However, since word got out of how awesome it was, contestants from all over the world joined. Slovakistan could not embarras itself - that year's tournament had to be more awesome, way more dramatic, and - most importantly - a whole lot bigger. Hence, during that year's tournament the contestants did not only play on the classic 8-by-8 chessboards, but rather on n-by-n boards.</p>
<p>That gave rise to a new problem though - the programs of skilled programmers which helped them the previous year were not capable of deciding the state of chessboards of such size!</p>
<p>Once again, the inhabitants of Slovakistan needed help.&nbsp;</p>
<p>That is the origin story of the now most popular tournament in the entire universe. These days all the galactic empires have a ceasefire in the intergalactic wars to all take part in the Intergalactic Chess Tournament. For its thousandth aniversary, the Slovakistan Milky Way Empire is preparing a truly spectacular show - the chesspieces this year will be represented by planets, and the chessboard will be an entire galaxy!</p>
<p>As in the legendary tale from a thousand years ago, they are facing the same problem: the programs written to decide the state of a chessboard can not handle the size of the chessboard, even when run on the most modern quantum computers. To tackle this problem, they have constructed a time machine to come to this legendary time - and look for a skilled programer who could help them with this task!</p>
<p>For a given description of a chessboard, decide its state - which player's king is under threat, and whether it is a check or a checkmate. Additionally, if it's a check, to help build up suspense, the contestants would like to know the number of valid moves the checked player has after which his king is no longer threatened.</p>
<p>For the purposes of this problem only take into account basic moves of every chesspiece; complicated moves such as Castling, En passant, moving a pawn 2 squares or Promotion are not accepted in the known universe.</p>
<h3>Input</h3>
<p>The first line of the input contains the integer <strong>1 ≤ t ≤ 20000</strong>&nbsp;- the number of chessboards. <strong>t</strong> descriptions of a chessboard follow.</p>
<p>The first line of each description contains two integers <strong>8 ≤ n ≤ 10<sup>18</sup><sup>&nbsp;</sup>, 2 ≤ p ≤ 2*10<sup>5</sup>&nbsp;</strong>- the length of side of the chessboard and the number of pieces currently on it.</p>
<p><strong>p</strong> lines follow, each in the form '<strong>x y c</strong>' , where <strong>1 ≤ x,y ≤ n </strong>indicate the coordinates of the chesspiece; the upper-left square has coordinates <strong>(1,1) </strong>while the bottom-right square is at <strong>(n,n)</strong>.</p>
<p><strong>c</strong>&nbsp;represents the type of the chesspiece - this character is from the set <strong>{KQRBHPkqrbhp}</strong>, representing in this order the king, queen, rook, bishop, knight (horse), and pawn.</p>
<p>The pieces belonging to the White player are marked by lowercase characters; the upper side of the chessboard (lower <strong>y </strong>coordinates) belongs to him, hence white pawns move in the positive <strong>y</strong>&nbsp;direction.</p>
<p>The pieces belonging to the Black player are marked by uppercase characters; the lower side of the chessboard (greater <strong>y </strong>coordinates) belongs to him, hence black pawns move in the negative <strong>y </strong>direction.</p>
<p>A blank line follows after every chessboard description.</p>
<p>The number or placement of the pieces may by all means be impossible to reach in a standard game of intergalactic chess, however you may assume that on every chessboard there is exactly one white king ('<strong>k</strong>') and one black king ('<strong>K</strong>'). No two pieces are on the same coordinates.</p>
<p>Input files are 'reasonable' - that is, if a file contains a large amount of testcases, they are reasonably small. Specifically, the sum of <strong>p</strong>&nbsp;within an input file does not exceed <strong>10<sup>6</sup></strong>.</p>
<h3>Output</h3>
<p>For each chessboard output one line with one of the following messages:</p>
<ul>
<li>"<strong>Safe</strong>", if neither players' kings are being threatened</li>
<li>"<strong>Impossible</strong>", if both players' kings are being threatened</li>
<li>"<strong>{colour}</strong> <strong>Check - m Plausible Moves</strong>", where <strong>{colour}</strong> is either "<strong>Black</strong>" or "<strong>White</strong>", if the respective player's king is being threatened, and there exists <strong>m</strong> valid moves by his pieces after which his king is no longer threatened</li>
<li>"<strong>{colour} Checkmate</strong>", where {colour} is either "<strong>Black</strong>" or "<strong>White</strong>",&nbsp;&nbsp;if the respective player's king is being threatened, and there exists no valid move by any of his pieces after which his king is no longer threatened</li>
</ul>
<h4>Additional note</h4>
<p>There are 16 input files "0" through "15". File 0 is the example given below. Files 1 through 7 contain testdata from CSTATE2.</p>
<p>After submission you can view extra information about the result of each file by clicking the result text ("accepted","wrong answer",...), such as the result of each file and the time/memory used, but no message is present like in CSTATE1 - if you are stuck, consider submitting there for a hint at what is off in your solution.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
7
8 4
5 1 k
4 3 H
4 5 h
5 7 K

8 4
5 2 h
3 3 k
6 4 H
4 5 K

8 6
1 1 k
4 1 H
4 2 H
2 3 H
3 3 H
7 6 K

8 7
1 1 k
4 1 H
4 2 H
2 3 H
3 3 H
7 6 K
2 7 r

8 9
1 1 K
7 1 R
8 1 r
1 2 R
3 2 h
8 2 r
1 5 r
2 5 r
6 6 k

8 6
1 1 k
8 2 R
4 4 B
2 5 R
7 6 K
3 7 q

8 9
3 2 P
4 2 P
5 2 P
3 3 P
4 3 k
5 3 P
4 4 P
5 4 p
4 5 K

</pre>
<pre><strong>Output:</strong>
Impossible
Safe
White Checkmate
White Check - 1 Plausible Moves
Black Checkmate
White Check - 1 Plausible Moves
Black Check - 5 Plausible Moves</pre>
<p>If you have any questions, problems or suggestions, do let me know :)</p>