# Recursion Problems:

## Problem 1: Calculate Mean of An Array using Recursion.


def calMean(A, N):
 
    if (N == 1):
        return A[N - 1]
    else:
        return ((findMean(A, N - 1) *
                (N - 1) + A[N - 1]) / N)
 
# Driver Code
Mean = 0
A = [1, 2, 3, 4, 5]
N = len(A)
print(findMean(A, N))
