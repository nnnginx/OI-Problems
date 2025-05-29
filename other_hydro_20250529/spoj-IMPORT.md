<p>

With the introduction of the new ThrustoZoom gigadimensional drive, it
has become possible for HyperCommodities, the import/export
conglomerate from New Jersey, to begin trading with even the most
remote galaxies in the universe.  HyperCommodities wants to import
goods from some of the galaxies in the Plural Z sector.  Planets
within these galaxies export valuable products and raw materials like
vacuuseal, transparent aluminum, digraphite, and quantum steel.
Preliminary reports have revealed the following facts: </p><p>

</p><ul>

<li> Each galaxy contains at least one and at most 26 planets.  Each
planet within a galaxy is identified by a unique letter from A to Z. <p>

</p></li><li> Each planet specializes in the production and export of one good.
Different planets within the same galaxy export different goods. <p>

</p></li><li> Some pairs of planets are connected by hyperspace shipping lines.
If planets A and B are connected, they can trade goods freely.  If
planet C is connected to B but not to A, then A and C can still trade
goods with each other through B, but B keeps 5% of the shipment as a
shipping fee.  (Thus A only receives 95% of what C shipped, and C
receives only 95% of what A shipped.) In general, any two planets can
trade goods as long as they are connected by some set of shipping
lines, but each intermediate planet along the shipping route keeps 5%
of what it shipped (which is not necessarily equal to 5% of the
original shipment). <p>

</p></li><li> At least one planet in each galaxy is willing to open a
ThrustoZoom shipping line to Earth.  A ThrustoZoom line is the same as
any other shipping line within the galaxy, as far as business is
concerned.  For example, if planet K opens a ThrustoZoom line to
Earth, then the Earth can trade goods freely with K, or it can trade
goods with any planet connected to K, subject to the usual shipping
fees. <p>

</p></li></ul>
     
HyperCommodities has assigned a relative value (a positive real number
less than 10) to each planet's chief export.  The higher the number,
the more valuable the product.  More valuable products can be resold
with a higher profit margin in domestic markets.  The problem is to
determine which planet has the most valuable export when shipping fees
are taken into account. <p>

The input consists of one or more galaxy descriptions.  Each galaxy
description begins with a line containing an integer <i>N</i> which
specifies the number of planets in the galaxy.  The next <i>N</i> lines
contain descriptions of each planet, which consist of: </p><p>

</p><ol>
<li> The letter used to represent the planet. <p>
</p></li><li> A space. <p>
</p></li><li> The relative value of the planet's export, in the form <i>d.dd</i>. <p>
</p></li><li> A space. <p>
</p></li><li> A string containing letters and/or the character `*'; a letter
indicates a shipping line to that planet, and a `*' indicates a
willingness to open a ThrustoZoom shipping line to Earth. <p>
</p></li></ol>

For each galaxy description, output a single line which reads "Import
from P" where P is the letter of the planet with the most valuable
export, once shipping fees have been taken into account.  (If more
than one planet have the same most valuable export value then output
the plant which is alphabetically first). <p>

A sample input file is shown here: </p><p>

</p><pre>1
F 0.81 *
5
E 0.01 *A
D 0.01 A*
C 0.01 *A
A 1.00 EDCB
B 0.01 A*
10
S 2.23 Q*
A 9.76 C
K 5.88 MI
E 7.54 GC
M 5.01 OK
G 7.43 IE
I 6.09 KG
C 8.42 EA
O 4.55 QM
Q 3.21 SO
</pre>

<p> The following output file should be produced from the above sample input:

</p><pre>Import from F
Import from A
Import from A
</pre>