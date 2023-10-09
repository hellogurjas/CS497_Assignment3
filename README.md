# CS497_Assignment3

Numbers 1-5

Number 1)

Given an array nums of size n, return the majority element.

The majority element is the element that appears more than ⌊n / 2⌋ times. You may assume that the majority element always exists in the array.

Hash map allows us to store according to occurences. We iterate through, using a loop. We incremenet a value for each element. After the occurences, we count and iterate through the values.

We can achieve O(n) since we only iterate through the array once to count.

Number 2)

Given an integer array nums and an integer k, return the kth largest element in the array.

Note that it is the kth largest element in the sorted order, not the kth distinct element.

Can you solve it without sorting?

We start by initializing the left to the start and the right to the end. Then we partition and after we return the final position. Then we are able to make our comparison. The average case is linear.

Number 3)

Given an integer array nums, return the maximum difference between two successive elements in its sorted form. If the array contains less than two elements, return 0.

You must write an algorithm that runs in linear time and uses linear extra space.

We simply make a bucket. For both string min and max. We divide our answer by the average to get our value. Then we are able to see the max and min of different buckets, and call accordingly. Since this time is determined by the length of the array, we achieve a time of O(n).

Number 4)

Given a string s, remove duplicate letters so that every letter appears once and only once. You must make sure your result is the smallest in lexicographical order among all possible results.

We pay attention to the stack, and the bool array. This allows us to mark if a value is there or not. Length of the bool array is 26. We simply mark true based on if the counts are greater or less, and keep track of

Number 5)

Given an integer array nums and an integer k, return the length of the shortest non-empty subarray of nums with a sum of at least k. If there is no such subarray, return -1.

Simple prefix sum calculation. We deque to increase, and make a comparison each time; as long as we keep track of the sum of the array, we are able to return the shortest non-empty subarray of nums. We iterate through each index to push, and at most we popped an index, which gives us O(n).

A subarray is a contiguous part of an array.
