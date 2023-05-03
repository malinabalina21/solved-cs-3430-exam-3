Download Link: https://assignmentchef.com/product/solved-cs-3430-exam-3
<br>
You have a directory of binary images. Your task is to implement an image search engine that converts the images into feature vectors and then finds the top <em>n </em>matches closest to a given input image. Would you use Jaccard similarity to find the closest images? You must answer this question as YES or NO (but not both!) and use 2-5 sentences to explain your answer. In other words, if your answer is YES, justify it briefly. If your answer is NO, justify it and give an alternative similarity metric you would use.

Type and save your solution in a multiline comment under the section Problem 1.1 in cs3430_s19_exam_03.py. <strong>Problem 1.2: (0.3 point; no coding)</strong>

Figure 1: Edge detection: original image (left); gradient edge detection (middle); Canny edge detection (right).

Consider the images in Figure 1. The left image in this figure is an original image with a horizontal line. The middle image shows the edges (white pixels) detected by the gradient edge detection algorithm discussed in lectures 19, 20 and implemented in assignment 10. The right image shows the edges detected by Canny. Explain (no more than 2-5 sentences) why Canny does not detect any edges in the original image while the gradient edge detection algorithm does.

Type and save your solution in a multiline comment under the section Problem 1.2 in cs3430_s19_exam_03.py.

<h2>Problem 1.3: (0.2 point; no coding)</h2>

Consider the gradient edge detection algorithm discussed in lectures 19, 20 and implemented in assignment 10. Briefly (2-5 sentences) describe how one can make this algorithm run faster.

Type and save your solution in a multiline comment under the section Problem 1.3 in cs3430_s19_exam_03.py.

<h2>Problem 1.4: (0.2 point; no coding)</h2>

Consider the Hough Transform line detection algorithm discussed in lectures 21, 22 and implemented in assignment 11. Briefly (2-5 sentences) describe how one can make this algorithm run faster.

Type and save your solution in a multiline comment under the section Problem 1.4 in cs3430_s19_exam_03.py.

<h2>Problem 1.5: (0.5 point; no coding)</h2>

Your task is to write an algorithm to distinguish different textures. Briefly (2-5 sentences) state which CVIP techniques covered in this class you would use to implement it and why.

Type and save your solution in a multiline comment under the section Problem 1.5 in cs3430_s19_exam_03.py.

<h2>Problem 1.6: (0.5 point; no coding)</h2>

Your task to to write an algorithm that finds all instances of an object in a larger image (e.g., all tennis balls in a tennis court photo). You’re thinking of using color histograms. Briefly (2-5 sentences) explain when your approach will work and when it will not.

<h2>Problem 1.7: (1 point; coding)</h2>

Figure 2: Line detection: original image (left); image with lines drawn.

Write the function detect_lines(impath1, impath2, magn_thresh=20, spl=20) that reads an image saved in impath1, uses the Hough Transform algorithm to detect lines in it at the gradient magnitude threshold magn_thresh and the support level threshold spl, and saves in impath2 the image with all detected lines drawn. You may use your implementations of gradient edge detection and Hough Transform from assignments 10 and 11. You may not use OpenCV for edge detection or Hough Transform. You may use OpenCV to draw lines in the resulting image with whatever color you want so long as they are clearly seen. Figure 2 shows an original image and the same image with the lines drawn blue and saved as cross_ln.png with the following call. The exam’s zip contains a couple of small images you can use for quick tests.

&gt;&gt;&gt; detect_lines(’cross.png’, ’cross_ln.png’, magn_thresh=20, spl=100)

Save your implementation of the function detect_lines() in cs3430_s19_exam_03.py.

<h1>Problem 2 (3 points)</h1>

<h2>Problem 2.1 (0.5 point; no coding)</h2>

A fertilizer company makes three types of fertilizers: 20-8-8 for lawns, 4-8-4 for gardens, and 4-4-2 for general purposes. The numbers in each brand (i.e., x-y-z) refer to the weight percentage of nitrate, phosphate, and potash, respectively. The company has 6,000 pounds of nitrate, 10,000 pounds of phosphate, and 4,000 pounds of potash to use. The profit is $3 per 100 pounds of lawn fertilizer, $8 per 100 pounds of garden fertilizer, and $6 per 100 pounds of general-purpose fertilizer. Formulate an LP problem for the numbers of pounds of each fertilizer that should be produced to maximize the company’s profit by clearly defining the objective function and the constraints. You do not have to solve this problem, just formulate it.

Type and save your solution in a multiline comment under the section Problem 2.1 in cs3430_s19_exam_03.py

<h2>Problem 2.2 (0.5 point; no coding)</h2>

Suppose that <em>F </em>is the non-empty feasible set for an LP problem and <em>f </em>is the objective function. Let <em>F </em>be bounded. Which one of the following statements is true?

<ol>

 <li><em>f </em>takes arbitrarily large negative values on <em>F</em>;</li>

 <li>If <em>f </em>is maximized/minimized, it achieves its maximum/minimum value at a corner point;</li>

 <li><em>f </em>takes arbitrarily large positive values on <em>F</em>;</li>

 <li><em>f </em>achieves its maximum/minimum value on the complement of <em>F</em>.</li>

</ol>

Type and save exactly one number as your solution in a multiline comment under the section Problem 2.2 in cs3430_s19_exam_03.py

<h2>Problem 2.3 (0.5 point; no coding)</h2>

Suppose that <em>F </em>is the non-empty feasible set for an LP problem and <em>f </em>is the objective function. Let <em>F </em>be unbounded. Suppose that <em>f </em>is to be maximized. Which one of the following statements is true?

<ol>

 <li><em>f </em>achieves its maximum/minimum value on the complement of <em>F</em>.</li>

 <li><em>f </em>takes arbitrarily large positive values on <em>F</em>;</li>

 <li><em>f </em>takes arbitrarily large negative values on <em>F</em>;</li>

 <li><em>f </em>attains its maximum at a corner point or <em>f </em>takes arbitrarily large positive values on <em>F</em>;</li>

 <li><em>f </em>attains its maximum at a corner point or <em>f </em>takes arbitrarily large negative values on <em>F</em>;</li>

</ol>

Type and save exactly one number as your choice in a multiline comment under the section Problem 2.3 in cs3430_s19_exam_03.py

<h2>Problem 2.4 (0.5 point; no coding)</h2>

Suppose that <em>F </em>is the non-empty feasible set for an LP problem and <em>f </em>is the objective function. Let <em>F </em>be unbounded. Suppose that <em>f </em>is to be minimized. Which one of the following statements is true?

<ol>

 <li><em>f </em>takes arbitrarily negative values on <em>F</em>;</li>

 <li><em>f </em>attains its minimum at a corner point or <em>f </em>takes arbitrarily large positive values on <em>F</em>;</li>

 <li><em>f </em>takes arbitrarily positive values on <em>F</em>;</li>

 <li><em>f </em>attains its minimum at a corner point or <em>f </em>takes arbitrarily large negative values on <em>F</em>;</li>

 <li><em>f </em>achieves its maximum/minimum value on the complement of <em>F</em>.</li>

</ol>

Type and save exactly one number as your choice in a multiline comment under the section Problem 2.4 in cs3430_s19_exam_03.py

<h2>Problem 2.5 (1 point; coding)</h2>

Use your implementations of maximize_obj_fun() and line_intersection() from assignment 12 to solve the following LP problem. Maximize <em>f</em>(<em>x,y</em>) = <em>x </em>+ <em>y </em>satisfying the following constraints:

<ul>

 <li><em>x </em>≥ 0;</li>

 <li><em>y </em>≥ 0;</li>

 <li><em>x </em>+ 2<em>y </em>≥ 6;</li>

 <li><em>x </em>− <em>y </em>≥ −4;</li>

 <li>2<em>x </em>+ <em>y </em>≤ 8.</li>

</ul>

Save your solution in the function problem_2_5() in cs3430_s19_exam_03.py. This function returns a 3-tuple (<em>x,y,z</em>), where <em>x </em>and <em>y </em>are the coordinates of the corner point where the objective function attains its maximum value of <em>z</em>.

<h1>Problem 3 (3 points)</h1>

Use numpy functions to solve the following problems.

<h2>Problem 3.1 (0.5 point; coding)</h2>

Solve the following linear system and save your solution in the function problem_3_1() in cs3430_s19_exam_03.py. The function problem_3_1() returns the 1D numpy array x that solves this linear system.

<em>x </em>+ <em>y </em>+ 2<em>z </em>= 9 2<em>x </em>+ 4<em>y </em>− 3<em>z </em>= 1

3<em>x </em>+ 6<em>y </em>− 5<em>z </em>= 0

<h2>Problem 3.2 (1 point; coding)</h2>

Solve the linear system in problem 3.1 using Cramer’s rule and save your solution in the function problem_3_2() in cs3430_s19_exam_03.py. This function returns the 1D numpy vector x that solves this linear system.

<h2>Problem 3.3 (1.5 points; coding)</h2>

A <em>proper </em>factor of a whole number <em>n </em>is a whole number <em>d </em>that divides <em>n </em>with no remainder and is strictly less than <em>n</em>. For example, the proper factors of 8 are 1, 2, and 4. Two integers <em>x </em>and <em>y </em>are called <em>satyamitra </em>numbers if the sum of the proper factors of <em>x </em>is equal to <em>y </em>and the sum of the proper factors of <em>y </em>is equal to <em>x</em>. For example, 220 and 284 are satyamitra numbers.

Implement the function satyamitra_numbers_in_range(lower, upper) that computes all pairs of satyamitra numbers in the range from lower to upper where both lower and upper are positive integers and lower ≤ upper. More specifically, a call to this function returns a list of pairs (i.e., 2-tuples) [(<em>x</em><sub>1</sub><em>,x</em><sub>2</sub>)<em>,</em>(<em>x</em><sub>3</sub><em>,x</em><sub>4</sub>)<em>,…,</em>(<em>x<sub>k</sub></em><sub>−1</sub><em>,x<sub>k</sub></em>)], where, in each pair (<em>x<sub>i</sub>,x<sub>j</sub></em>), <em>x<sub>i </sub></em>and <em>x<sub>j </sub></em>are satyamitra numbers such that lower ≤ <em>x<sub>i </sub></em>≤ upper and lower ≤ <em>x<sub>j </sub></em>≤ upper. Here is a sample call.

&gt;&gt;&gt; satyamitra_numbers_in_range(0, 2000)

[(220, 284), (1184, 1210)]

Write the function satyamitra_matrix(sn_list) that takes a list of satyamitra number pairs that contains <em>n </em>numbers, where <em>n </em>is a perfect square (recall that a perfect square is an integer that is the product of two equal integers, e.g., 4 = 2 · 2, 9 = 3 · 3, 16 = 4 · 4, etc.) and creates an <em>n </em>× <em>n </em>numpy matrix out of these pairs. For example, if sn_list = [(<em>x</em><sub>1</sub><em>,x</em><sub>2</sub>)<em>,</em>(<em>x</em><sub>3</sub><em>,x</em><sub>4</sub>)], then satyamitra_matrix(sn_list) creates this matrix

.

If sn_list = [(<em>x</em><sub>1</sub><em>,x</em><sub>2</sub>)<em>,</em>(<em>x</em><sub>3</sub><em>,x</em><sub>4</sub>)<em>,…,</em>(<em>x</em><sub>8</sub><em>,x</em><sub>9</sub>)], then satyamitra_matrix(sn_list) creates this matrix

.

If sn_list = [(<em>x</em><sub>1</sub><em>,x</em><sub>2</sub>)<em>,</em>(<em>x</em><sub>3</sub><em>,x</em><sub>4</sub>)<em>,</em>(<em>x</em><sub>5</sub><em>,x</em><sub>6</sub>)<em>,…,</em>(<em>x</em><sub>15</sub><em>,x</em><sub>16</sub>)], the matrix looks like

<table width="0">

 <tbody>

  <tr>

   <td width="40"> <em>x</em><sub>1</sub> <em>x</em><sub>5</sub> <em>x</em><sub>9 </sub><em>x</em>13</td>

   <td width="31"><em>x</em><sub>2 </sub><em>x</em><sub>6 </sub><em>x</em>10 <em>x</em>14</td>

   <td width="31"><em>x</em><sub>3 </sub><em>x</em><sub>7 </sub><em>x</em>11 <em>x</em>15</td>

   <td width="34"><em>x</em><sub>4</sub> <em>x</em><sub>8</sub>. <em>x</em>12 <em>x</em>16</td>

  </tr>

 </tbody>

</table>

Here is a concrete example.

&gt;&gt;&gt; satyamitra_matrix(satyamitra_numbers_in_range(0, 2000)) array([[ 220, 284],

[1184, 1210]])

Use these functions to write the boolean function is_satyamitra_matrix_singular() that determines if the matrix composed of the satyamitra numbers in the range [1, 20000] (from 1 to twenty thousand) is singular. Save your implementations of satyamitra_numbers_in_range(), satyamitra_matrix(), and is_satyamitra_matrix_singular() in cs3430_s19_exam_03.py.

<h1>Problem 4 (3 points)</h1>

<h2>Problem 4.1 (0.5 point; no coding)</h2>

When is the profit of a firm maximized?

<ol>

 <li>When marginal revenue is strictly smaller than marginal cost;</li>

 <li>When marginal revenue is strictly greater than marginal cost;</li>

 <li>When marginal revenue equals marginal cost;</li>

 <li>When marginal revenue is zero;</li>

 <li>When marginal cost is zero.</li>

</ol>

Type and save exactly one number as your solution in a multiline comment under the section Problem 4.1 in cs3430_s19_exam_03.py

<h2>Problem 4.2 (1.5 points; coding)</h2>

Solve <em>y</em><sup>0 </sup>= 5<em>y</em>, <em>y</em>(0) = 3 and write the function problem_4_2() that plots and displays the graph of your solution where the range of <em>x </em>is limited to [-2, 2] and the range of <em>y </em>is limited to [0, 10].

<h2>Problem 4.3 (0.5 point; no coding)</h2>

Suppose that the demand for a given product at a given price is elastic. What happens to the change in revenue with respect to the change in price?

<ol>

 <li>When the revenue increases, the price decreases and when the revenue decreases, the price increases;</li>

 <li>When the revenue increases or decreases, the price remains the same;</li>

 <li>When revenue increases or decreases, the price changes in the same direction;</li>

</ol>

Type and save your solution in a multiline comment under the section Problem 4.3 in cs3430_s19_exam_03.py

<h2>Problem 4.4 (0.5 point; no coding)</h2>

Suppose that the demand for a given product at a given price is inelastic. What happens to the change in revenue with respect to the change in price?

<ol>

 <li>When the revenue increases, the price decreases and when the revenue decreases, the price increases;</li>

 <li>When the revenue increases or decreases, the price remains the same;</li>

 <li>When revenue increases or decreases, the price changes in the same direction;</li>

</ol>

Type and save your solution in a multiline comment under the section Problem 4.4 in cs3430_s19_exam_03.py

<h1>Problem 5: (3 points)</h1>

<h2>Problem 5.1 (1 point; coding)</h2>

Use the Newton-Raphson algorithm to approximate a solution to <em>e</em><sup>10−<em>x </em></sup>= 20−<em>x</em>. Save your implementation in the function problem_5_1(). This function returns a float.

<h2>Problem 5.2 (2 points; coding)</h2>

√

Write the function pell_sqrt(n) that uses Pell equations to compute <em>n</em>, where 1 ≤ <em>n </em>≤ 30 and <em>n </em>is not a perfect square. Pells do not approximate perfect squares well. An integer <em>n </em>is a perfect square if there exists another integer <em>k </em>such that <em>k</em><sup>2 </sup>= <em>n</em>. For example, 1 is a perfect square, because 1<sup>2 </sup>= 1; 4 is a perfect square, because 4 = 2<sup>2</sup>; 9 is a perfect square, because 9 = 3<sup>2</sup>, etc.

You can use the function test_pell_sqrt(lwr, uppr) defined in cs3430_s19_exam_03.py to test your implementation of pell_sqrt in the interval [lwr, uppr], where lwr and uppr are positive integers such that lwr ≤ uppr.

def test_pell_sqrt(lwr, uppr):

for i in range(lwr, uppr+1):

try:

print(’pell_sqrt(’ + str(i) + ’)=’ + str(pell_sqrt(i)) + ’; ’ + 

’math.sqrt(’ + str(i) + ’)=’ + str(math.sqrt(i))) except Exception, e:

print(str(i) + ’ –&gt; ’ + str(e))

Let’s use Pells to approximate square roots of numbers in the range [1<em>,</em>10].

&gt;&gt;&gt; test_pell_sqrt(1, 10) pell_sqrt(1)=1 is a perfect square; math.sqrt(1)=1.0 pell_sqrt(2)=1.41666666667; math.sqrt(2)=1.41421356237 pell_sqrt(3)=1.73111395647; math.sqrt(3)=1.73205080757 pell_sqrt(4)=4 is a perfect square; math.sqrt(4)=2.0 pell_sqrt(5)=2.23607038123; math.sqrt(5)=2.2360679775 pell_sqrt(6)=2.44948974279; math.sqrt(6)=2.44948974278 pell_sqrt(7)=2.64575127772; math.sqrt(7)=2.64575131106 pell_sqrt(8)=2.82842712474; math.sqrt(8)=2.82842712475 pell_sqrt(9)=9 is a perfect square; math.sqrt(9)=3.0 pell_sqrt(10)=3.16227766017; math.sqrt(10)=3.16227766017

Let’s use Pells to approximate square roots of numbers in the range [11<em>,</em>20].

&gt;&gt;&gt; test_pell_sqrt(11, 20) pell_sqrt(11)=3.31662479036; math.sqrt(11)=3.31662479036 pell_sqrt(12)=3.46410161514; math.sqrt(12)=3.46410161514 pell_sqrt(13)=3.60555127546; math.sqrt(13)=3.60555127546 pell_sqrt(14)=3.74165738677; math.sqrt(14)=3.74165738677 pell_sqrt(15)=3.87298334621; math.sqrt(15)=3.87298334621 pell_sqrt(16)=16 is a perfect square; math.sqrt(16)=4.0 pell_sqrt(17)=4.12310562562; math.sqrt(17)=4.12310562562 pell_sqrt(18)=4.24264068712; math.sqrt(18)=4.24264068712 pell_sqrt(19)=4.35889894354; math.sqrt(19)=4.35889894354 pell_sqrt(20)=4.472135955; math.sqrt(20)=4.472135955

Let’s use Pells to approximate square roots of numbers in the range [21<em>,</em>30].

&gt;&gt;&gt; test_pell_sqrt(21, 30) pell_sqrt(21)=4.58257569496; math.sqrt(21)=4.58257569496 pell_sqrt(22)=4.69041575982; math.sqrt(22)=4.69041575982 pell_sqrt(23)=4.79583152331; math.sqrt(23)=4.79583152331 pell_sqrt(24)=4.89897948557; math.sqrt(24)=4.89897948557 pell_sqrt(25)=25 is a perfect square; math.sqrt(25)=5.0 pell_sqrt(26)=5.09901951359; math.sqrt(26)=5.09901951359 pell_sqrt(27)=5.19615242271; math.sqrt(27)=5.19615242271 pell_sqrt(28)=5.29150262213; math.sqrt(28)=5.29150262213 pell_sqrt(29)=5.38516480713; math.sqrt(29)=5.38516480713 pell_sqrt(30)=5.47722557505; math.sqrt(30)=5.47722557505 Save your implementation of pell_sqrt(n) in cs3430_s19_exam_03.py.