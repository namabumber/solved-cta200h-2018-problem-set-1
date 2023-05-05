Download Link: https://assignmentchef.com/product/solved-cta200h-2018-problem-set-1
<br>






Please submit your responses electronically by github. Instructions included at the bottom of this assignment. Make sure the instructors will be able to run your code. Also include any figures you make as part of the activity.

For this assignment you may work in pairs and submit your work as a pair. In this case please make sure to discuss as much as possible and to share the coding work equitably.

<ol>

 <li>(Dan Green.) Write a script that finds and replaces a given word in all the .txt files in the working directory, with the following properties:

  <ul>

   <li>The script <em>name </em>is called with “<em>name find replace</em>” where <em>find </em>and <em>replace </em>are words the user chooses when running the program. b A new directory named <em>replace </em>is created within the working directory.</li>

  </ul></li>

</ol>

c A copy of the .txt files with <em>find </em>is put in the <em>replace </em>directory, but with all occurrences of ’find’ replaced by ’replace.’ If a file does not contain <em>find</em>, it is ignored.

<ol start="2">

 <li>(Adapted from Newman.) The binomial coefficient is given by</li>

</ol>

(1)

for <em>k </em>≥ 1 and 1 for

<ul>

 <li>Write your own routine to generate the binomial coefficients for a given<em>n </em>and <em>k</em>. Make sure the result is an integer (not a float) and gives the (correct) value 1 for <em>k </em>= 0. (Hint; you can do a cancellation to make it more tractable.)</li>

 <li>Use your routine to write out the first 20 lines of Pascal’s triangle. Thisgives the coefficients for expanding binomials of the form (<em>x </em>+ <em>y</em>)<em><sup>n</sup></em>.</li>

 <li>Consider a biased (e.g., bent) coin with probability <em>p </em>of coming up heads, and probability 1 − <em>p </em>of coming up tails. The probability of obtaining heads <em>k </em>times when flipping the coin <em>n </em>times is given by</li>

</ul>

<em>.                                                     </em>(2)

Consider an experiment in which you flip the coin <em>n </em>times and hope to obtain at least <em>k </em>values of heads. For values of <em>p</em>, <em>n</em>, and <em>k </em>of your choice, use your routine to calculate the probability of obtaining heads at least <em>k </em>times in <em>n </em>flips. (Example application: a baseball player with batting average <em>p </em>= 0<em>.</em>250 has <em>n </em>= 4 attempts to obtain a hit, or at-bats, during a given game. What is the chance that s/he will obtain at least one hit during the game, assuming that all at-bats are statistically the same and uncorrelated?)

<ul>

 <li>Simulate the experiment <em>N </em>times for <em>N </em>∈ {10<em>,</em>100<em>,</em>1000}, or a similar range of your choice. For each value of <em>N</em>, which fraction of experiments were successful? Consider showing the results in a plot.</li>

</ul>

<ol start="3">

 <li>(Adapted from Newman.) The Bessel function of the first kind of order <em>m </em>is given by</li>

</ol>

<em>.                                    </em>(3)

<ul>

 <li>Write a routine to calculate this integral directly, using the methodof integration of your choice, using only the library sine and cosine functions (you may use the library Bessel functions to check the results of your integral). Plot the results for a few values of <em>m</em>.</li>

 <li>Suppose that light passing through a circular telescope aperture of ra-dius <em>a </em>is focussed on the telescope’s focal plane. If the source is effectively a point on the sky, then the pattern of intensity seen in the focal plane at a distance <em>q </em>from the optical axis is given by</li>

</ul>

(4)

where <em>I</em><sub>0 </sub>is the intensity at the center, and <em>x </em>= <sup>2</sup><em><sub>λR</sub><sup>πaq</sup></em>. Here <em>λ </em>is the wavelength of the light and <em>R </em>is the distance from the aperture to the focal plane. This is known as the “point spread function” in optical astronomy, the “beam” in radio astronomy, and the “Airy disk” in general. (The geometrical ratio <em>R/</em>(2<em>a</em>) is known as the “f-number” of the telescope and typically has values of several.) For a given set of parameters, make an image of the two-dimensional point spread function, using a monochrome color scheme. Indicate the <em>x </em>and <em>y </em>axes with real distance units. (It might be hard to see the detail away from the main beam; if so, try increasing the contrast of your image in order to see the features on the edge.)

<ul>

 <li>Download a high-resolution astronomical (or other) image of your choice.If this image were viewed through a telescope with a finite aperture, each pixel’s value would get smeared out to neighboring pixels, degrading the image. This is known as <em>convolution</em>. To simulate how this image would look when viewed through a telescope, use a canned convolution routine (e.g., scipy.ndimage.filters.convolve(), scipy.signal.convolve2d()) to convolve the image by your point-spread function. Don’t worry about being quantitative in this sub-section; rather play around to see what happens to your image when you convolve it.</li>

</ul>

<ol start="4">

 <li>(George) <em>Scene: </em>Its 3pm and your supervisor has just handed you their old Fortran77 code that they swear “solved this problem in the 80s” and “is really smartly written and easy to follow”. After the meeting you take one look at the code and realize it doesn’t. And it’s not.</li>

</ol>

But, you said you’d have results by the group meeting the following day, so lets see if we can understand what it is doing, fix it up, and get some results! Also, this code has somehow already been converted into python 3. who knows

The code can be found in the form of a jupyter notebook in problemset1/question6/question6.ipynb . Go through the examples near the top, and fix up the code in the final cell.

<ol start="5">

 <li>For each point in the complex plane <em>c </em>= <em>x </em>+ <em>iy</em>, with −2 <em>&lt; x &lt; </em>2 and −2 <em>&lt; y &lt; </em>2, set <em>z</em><sub>0 </sub>= 0 and iterate the equation <em>z<sub>i</sub></em><sub>+1 </sub>= <em>z<sub>i</sub></em><sup>2 </sup>+ <em>c</em>. Note what happens to the <em>z<sub>i</sub></em>’s: some points will remain bounded in absolute value |<em>z</em>|<sup>2 </sup>= ℜ(<em>z</em>)<sup>2 </sup>+ ℑ(<em>z</em>)<sup>2</sup>, while others will run off to infinity. Make an image in which your points <em>c </em>that diverge are given one color and those that stay bounded are given another. (Once you have done this, you can try coloring the points that diverge using a colorscale that indicates the iteration number at which the given point diverged.) Try zooming in on a portion of the image and trying again.</li>

 <li>Write your own program simulating a space battle. It should have 3 typesof spaceships: standard spaceships, warships, and speeders. Each ship has lasers, shields and hull strength (and most importantly, a name!). Warships additionally have high powered missiles which they fire 30% of the time, while speeders have a 50% chance to dodge incoming shots. When a spaceship is shot by another ship, it first depletes its shields equal to the strength of the shot. When it runs out of shields, it takes hull damage at 50% of the shot strength. Once the hull is breached, the ship is destroyed!</li>

</ol>

Your program should include a class Ship that defines the standard spaceship, and two classes which inherit from Ship called Warship and Speeder. The classes should store the ship’s shield strength, hull strength, laser power and name. There should be, at a minimum, methods to deal with when a ship shoots, is shot at, whether the ship is destroyed or not, and printing a diagnostic summary of the ship’s status.

Your program should instantiate 3 regular ships, 1 warship and 1 speeder.

The spaceships should shoot randomly at each other until only one remains (targets cannot be themselves nor ships that are already destroyed). Print a log of the battle as it progresses, and declare a final victor.

<ul>

 <li></li>

</ul>