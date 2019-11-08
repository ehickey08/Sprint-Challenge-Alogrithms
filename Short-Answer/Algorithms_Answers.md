#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) This could be rewritten as JS for loop as follows for(a = 0; a < n^3; a += n^2). In order to reach n^3, if
    incrementing by n^2, it would take n loops. So this order would be O(n).


b) The for loop is a very clear O(n). The inner while loop is going to depend on what power of 2 n is. So if n = 32, then
  n = 2^5 which means 5 loops. Another way to put this is the number of loops will be equal to log base 2 n. Since I have
  not seen us discuss the base of log in regards to O, I will just treat it was a log n. Multiply the two loops and you get
  O (n log n).


c) The base case for this recursive funtion is bunnies = 0, which means the function has to be called n times since
    bunnies is decremented by 1 each time. This makes it O(n).

## Exercise II
This would require a strategy the implements the concept of binary search. It would have a runtime complexity of O(log n).0
The strategy is to start at the middle floor, drop an egg. If it breaks, you will move down. If not, you will move up.
The floor you move up or down to will be the middle of that section.
So for a 60 story building, you start at floor 30. If it breaks, go to floor 15. If it doesn't break there, go to floor
22. If it breaks there, go to floor 18. Once you find a floor where it breaks and the one immediately below it doesn't,
then you have found the floor where eggs start to break.
