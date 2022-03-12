# Leetcode-Two-Sum-Problems-Solution-with-Approach
This is very interesting problem from leetcode practice, in this repo i am going to share my approach to this problem with implementation.
Approach:
1. We have given an unsorted array and we have to find the indices whose values sum is equals to the given target.
2. So obiviously we come up with naive approach i.e iterate through all the pairs and compare the sum of the pairs with given target. But this is an expensive approach, i.e O(N^2).
3. Again after thinking we might decide to use two pointer approach, but as we are aware, that two pointer approach is based on binary search technique which needs array to be sorted.
but if we sort the array then indices will change so our output never will be as expected.
4. But you don't worry, i have implemented same approach(Two pointer) but with the use of different container i.e nothing but the pairs in STL.
5. We will use vetors of pairs to implement two pointer approach.
6. we will store pairs of array element and its indices during traversing he array. 
7. Then sort the vector of pairs ascendingly, this will help to unchange the indices of array elements, it will sort the vector of pairs with its genuine indices.
8. And finally we will use two pointer approach on the sorted vectors of pairs.
9. std::sort() uses Introsort having NLogN time so we can expect the total time complexity to NlogN.
