The Price Is Wrong
==================

You're playing a game in which you try to guess the correct retail price of various products for sale. After guessing the price of each product in a list, you are shown the same list of products sorted by their actual prices, from least to most expensive. (No two products cost the same amount.) Based on this ordering, you are given a single chance to change one or more of your guesses.

Your program should output the smallest set of products such that, if you change your prices for those products, the ordering of your guesses will be consistent with the correct ordering of the product list. The products in the returned set should be listed in alphabetical order. If there are multiple smallest sets, output the set which occurs first lexicographically.

For example, assume these are your initial guesses:

    code = $20
    jam = $15
    foo = $40
    bar = $30
    google = $60

If the correct ordering is code jam foo bar google, then you would need to change two of your prices in order to match the correct ordering. You might change one guess to read jam = $30 and another guess to read bar = $50, which would match the correct ordering and produce the output set bar jam. However, the output set bar code comes before bar jam lexicographically, and you can match the correct ordering by changing your guesses for these items as well.

###Input

The first line of input gives the number of cases, N. N test cases follow. Each case consists of two lines. The first line contains the list of products, space separated, sorted from least to most expensive. Each product's name will consist of only lowercase letters and underscores. There will be no duplicate products in the list. The second line contains your initial guesses for each product in the list, respectively. All guesses will be integers between 1 and 100, inclusive. The number of guesses will be equal to the number of products, and no two guesses will be the same. The guesses will be space separated. (Note that although the initial guesses all happen to be integers, you are allowed to change your guesses to any amounts, not just integers.)

###Output

For each test case, output one line containing "Case #x: " followed by the set of products for which you must change your prices. The products should be in alphabetical order and space separated. The constraints guarantee that you will need to change the price of at least one product for each test case.

###Limits

1 ≤ N ≤ 100.

###Small dataset

2 ≤ number of products in list ≤ 8

###Large dataset

2 ≤ number of products in list ≤ 64

Sample

Input

	1
	code jam foo bar google
	20 15 40 30 60

OutPut

	Case #1: bar code