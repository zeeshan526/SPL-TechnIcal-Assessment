# Search Problems:

## Problem 1: Given An Array and a target number Find all the Pairs the sum of which is equal to that target number.

    Find all the pairs in an array the sum of which is equal to
    the provided target number.


def findPairs(arr, n, sum):
 
    count = 0  # Initialize result
 
    # Consider all possible pairs
    # and check their sums
    for i in range(0, n):
        for j in range(i + 1, n):
            if arr[i] + arr[j] == sum:
                count += 1
 
    return count
 
# Driver function
arr = [1, 5, 7, -1, 5]
n = len(arr)
sum = 6
print("Count of pairs is",
      getPairsCount(arr, n, sum))
