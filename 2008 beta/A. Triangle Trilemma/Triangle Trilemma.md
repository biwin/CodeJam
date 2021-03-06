Triangle Trilemma
=================

You're interested in writing a program to classify triangles. Triangles can be classified according to their internal angles. If one of the internal angles is exactly 90 degrees, then that triangle is known as a "right" triangle. If one of the internal angles is greater than 90 degrees, that triangle is known as an "obtuse" triangle. Otherwise, all the internal angles are less than 90 degrees and the triangle is known as an "acute" triangle.

Triangles can also be classified according to the relative lengths of their sides. In a "scalene" triangle, all three sides have different lengths. In an "isosceles" triangle, two of the sides are of equal length. (If all three sides have the same length, the triangle is known as an "equilateral" triangle, but you can ignore this case since there will be no equilateral triangles in the input data.)

Your program must determine, for each set of three points, whether or not those points form a triangle. If the three points are not distinct, or the three points are collinear, then those points do not form a valid triangle. (Another way is to calculate the area of the triangle; valid triangles must have non-zero area.) Otherwise, your program will classify the triangle as one of "acute", "obtuse", or "right", and one of "isosceles" or "scalene".

###Input


The first line of input gives the number of cases, N. N test cases follow. Each case is a line formatted as

	x1 y1 x2 y2 x3 y3

###Output


For each test case, output one line containing "Case #x: " followed by one of these strings:

    isosceles acute triangle
    isosceles obtuse triangle
    isosceles right triangle
    scalene acute triangle
    scalene obtuse triangle
    scalene right triangle
    not a triangle

###Limits


1 ≤ N ≤ 100,
x1, y1, x2, y2, x3, y3 will be integers.

###Small dataset

0 ≤ x1, y1, x2, y2, x3, y3 ≤ 9

Large dataset

-1000 ≤ x1, y1, x2, y2, x3, y3 ≤ 1000

###Sample

Input

	8
	0 0 0 4 1 2
	1 1 1 4 3 2
	2 2 2 4 4 3
	3 3 3 4 5 3
	4 4 4 5 5 6
	5 5 5 6 6 5
	6 6 6 7 6 8
	7 7 7 7 7 7

Output

	Case #1: isosceles obtuse triangle
	Case #2: scalene acute triangle
	Case #3: isosceles acute triangle
	Case #4: scalene right triangle
	Case #5: scalene obtuse triangle
	Case #6: isosceles right triangle
	Case #7: not a triangle
	Case #8: not a triangle