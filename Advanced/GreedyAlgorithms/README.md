# Greedy Algorithms:

## Problem 1: Find Minimum Absolute Difference of Adjacent Elements In An Array.

    Given an array of elements find the minimum absolute difference
    between adjacent elements in an array.

def findAbsMin(arr,n):
    # sort the given array
    arr.sort()
    # initialize sum
    sum = 0
         
    # min absolute difference for
    # the 1st array element
    sum += abs(arr[0] - arr[1]);
         
    # min absolute difference for
    # the last array element
    sum += abs(arr[n - 1] - arr[n - 2]);
         
    # find min absolute difference for
    # rest of the array elements and
    # add them to sum
    for i in range(1, n - 1):
        sum += min(abs(arr[i] - arr[i - 1]),
                  abs(arr[i] - arr[i + 1]))
             
    # required sum
    return sum;
