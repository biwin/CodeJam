Random Route
============

Where do you want to go today, and how do you want to get there? You decide to choose the answer to both questions at random.

You will be given a list of roads. Each road connects one city to another city (all roads are one-way), and each road takes a certain amount of time to drive. You will also be given a starting city. Consider all cities that you're able to drive to, not including your starting city, and choose one of them at random with uniform probability to be your destination. Now consider every fastest route from your starting city to your destination city, and choose one of these routes at random with uniform probability. This will be the route on which you end up driving.

For each road in the input, your program must output the probability that you will end up driving on that road, given the behavior outlined above.

###Input

The first line of input gives the number of cases, N. N test cases follow. Each case begins with a line formatted as

	num_roads starting_city

This will be followed by num_roads lines, each formatted as

	city1 city2 time

Each line represents a one-way road that starts at city1 and ends at city2, and takes time hours to drive. All cities will be formatted as strings consisting of only lowercase letters and underscores. For each road, city1 will not be equal to city2, and time will be an integer between 1 and 100000, inclusive. The starting city is guaranteed to appear as city1 on at least one road; therefore, there will always be at least one possible destination (and at least one shortest route to that destination).

###Output

For each test case, output one line containing "Case #x: " followed by the probability that you will drive on each road, in the same order that the roads were listed in the input. Probabilities should be space separated and formatted so there are exactly seven digits after the decimal point. Each probability must be within a distance of 1e-6 from the correct answer to be judged as correct.

###Limits

1 ≤ N ≤ 100.

###Small dataset

2 ≤ num_roads ≤ 25.

###Large dataset

2 ≤ num_roads ≤ 50.

Sample
------


Input


	1
	5 san_francisco
	san_francisco los_angeles 6
	los_angeles san_diego 2
	san_francisco san_diego 8
	los_angeles san_diego 2
	san_francisco los_angeles 6

Output

	Case #1: 0.4500000 0.2000000 0.1000000 0.2000000 0.4500000