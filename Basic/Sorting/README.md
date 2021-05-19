# Sorting Problems:

## Problem 1: Distribute An Array of Numbers around a given pivot

    Given an Array of integers and pivot integer return an array
    that ditributes the array around that pivot in a sorted order.

    Example:

    In many cases, multiple pivots will be equally good. Further, 
    if one uses a three-way subdivision where all items equal to 
    the pivot get grouped in the middle,the optimal choice of pivot 
    would depend upon more than just the number of elements above 
    and below the pivot, but also their value distribution. 
    For example, given [1,2,2,2,3,4,5,6,7] the median value is 3, 
    but pivoting around 3 would require one pivoting operation on 
    the left and two on the right, while pivoting around 4 would 
    result in only one additional operation being needed on each 
    side.
