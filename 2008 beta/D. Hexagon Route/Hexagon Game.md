Hexagon
=======


You are playing a game on a hexagonal board of size S. The middle row is composed of S hexagons, and the top and bottom rows each have (S + 1) / 2 hexagons. (S will be odd.) The hexagons are numbered starting with 1 in the upper left, and increasing left-to-right and top-to-bottom. Here is a hexagonal board of size S=5:

The game starts with S checkers on the board. Multiple checkers might start in the same position. Each checker also has an associated integer value between 0 and 50, inclusive. A turn consists of choosing a checker and moving it to an adjacent position, which increments your score by the value of that checker. Checkers cannot move off the board. Each position can contain any number of checkers at the same time.

The game ends when all the checkers are lined up in a straight row, with exactly one checker per hexagon. There are three possible ending configurations on any board. For S=5, the game will end when checkers are in positions (1, 5, 10, 15, 19), or in positions (3, 6, 10, 14, 17), or in positions (8, 9, 10, 11, 12). Your program must output the smallest possible score of a finished game.

For example, assume the checkers start in positions (1, 2, 5, 15, 19). The checker in position 1 has a value of 1, the checkers in positions 2 and 5 have values of 3, and the checkers in positions 15 and 19 have values of 0. You could move the checker from position 1 into position 5 and then position 10. Both of these moves add one point to your score. Then you could move the checker from position 2 into position 1, adding three points to your score. This game would end with a score of 5, which is the lowest possible score for this starting configuration.

###Input

The first line of input gives the number of cases, N. N test cases follow. Each case consists of two lines. The first line contains the starting positions of the checkers, space separated. The second line contains the values of each checker, respectively, space separated.

###Output

For each test case, output one line containing "Case #x: " followed by the minimum possible score of a finished game.

###Limits

1 ≤ N ≤ 100.

###Small dataset

3 ≤ S ≤ 15; S is odd.

###Large dataset

3 ≤ S ≤ 75; S is odd.

Sample
------

Input

	1
	1 2 5 15 19
	1 3 3 0 0


Output

	Case #1: 5