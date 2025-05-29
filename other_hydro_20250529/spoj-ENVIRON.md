<p>One of the major challenges for environmental engineers in the future will be the overall scarcity of potable water. Not only vegetation and wildlife are fundamentally dependent upon adequate freshwater resources, but also humans. Several desalination processes were developed to make sea water drinkable.</p>
<p>Nonetheless, the water distribution is not uniform on planet, and so some regions are lacking water while others possess it on excess. The International Committee for Precious Consumables (ICPC) worked out an ambitious project fostering the uniform distribution of water on Earth (a perfect ball). The richest and poorest regions in terms of water resources were found to lie equidistantly distributed along a circle of maximum length around the Earth (i.e. the centre of the Earth is also the centre of this circle). So the idea came to construct gigantic pipelines that can transport water along this circle.</p>
<p>&nbsp;</p>
<p><img src="../../../content/imuteb:Environ1" alt="" width="207" height="187"><img src="../../../content/imuteb:Environ2" alt="" width="281" height="187"></p>
<p>&nbsp;</p>
<p>Each pipeline has two terminals, starting at a location with water abundance and ending in a region with water scarcity. As drilling the Earth on so long distances is not a reasonable option, all pipelines will be above Earth. Further are there dedicated ducts for the pipelines at different heights. That is, a pipeline grows vertically into the sky until one of the allowed heights is reached, makes a 90¡ã angle, and follows the duct at constant height until it is above the depletion region, where it forms another 90¡ã angle to descent vertically to ground.</p>
<p>As all pipelines¡¯ projection to ground must follow the same circle, the ICPC faces a serious problem. They must make sure that no pipelines cross each other in this 2D plane! Further they are concerned about the total length of the pipes, which they¡¯d like to minimize. Your task is to calculate the minimal total length of all the pipes, knowing that the allowed duct heights are non-zero integer multiples of the distance between two adjacent locations (measured along the circle on surface level), which for our purpose has a value of 1.</p>
<p>&nbsp;</p>
<p><strong>INPUT</strong></p>
<p>The input consists of several test-cases separated by an empty line. Each test-case starts with the number of locations <em>N (0&lt;=N&lt;=500)</em>, followed by a line containing <em>N </em>numbers (¡®0¡¯ or ¡®1¡¯) and describing the locations along the circle. A ¡®0¡¯ stands for a location with water depletion, a ¡®1¡¯ for a region with water abundance. You may safely assume that there are as many ¡®0¡¯ as ¡®1¡¯. Input terminates on a test-case <em>with N=0</em>, which must not be evaluated.</p>
<p>&nbsp;</p>
<p><strong>OUTPUT</strong></p>
<p>For each test-case, output the minimum total length (to a precision of 10<sup>-2</sup>) of the pipes so that each abundance region connects to exactly one depletion region.</p>
<p>&nbsp;</p>
<p><strong>SAMPLE INPUT</strong></p>
<p>4</p>
<p>1 0 0 1</p>
<p>&nbsp;</p>
<p>8</p>
<p>1 1 1 1 0 0 0 0</p>
<p>&nbsp;</p>
<p>0</p>
<p>&nbsp;</p>
<p><strong>SAMPLE OUTPUT</strong></p>
<p>&nbsp;</p>
<p>9.14</p>
<p>31.00</p>
<p>&nbsp;</p>
<p><img src="../../../content/imuteb:Environ3" alt="" width="158" height="130">&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; <img src="../../../content/imuteb:Environ4" alt="" width="156" height="127">&nbsp;&nbsp;&nbsp; <img src="../../../content/imuteb:Environ5" alt="" width="163" height="131"></p>
<p>Sample input 1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp; &nbsp; &nbsp;&nbsp; Sample input 2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; A larger test-case</p>