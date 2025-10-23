# CMPS 2200 Reciation 5
## Answers

**Name:** Hoang Dieu Linh Nguyen


Place all written answers from `recitation-05.md` here for easier grading.







- **1b.**
When comparing the running times, the fixed-pivot Quicksort performs well on random lists but becomes very slow on already sorted lists, because choosing the first element as the pivot leads to highly unbalanced partitions (worst case O(n^2)).
The randomized version performs more consistently because random pivot selection avoids the worst case with high probability, maintaining an expected O(n log n) runtime.
Selection sort performs consistently worse for large n because its O(n^2) time complexity dominates.
Therefore, input type strongly affects deterministic Quicksort but not randomized Quicksort, matching the theoretical asymptotic behavior.



- **1c.**
Comparing Quicksort with Python’s built-in Timsort, Timsort is significantly faster for all input sizes, especially for partially sorted lists.
Timsort combines merge sort and insertion sort, using adaptive techniques to detect existing order and minimize comparisons.
In contrast, both Quicksort implementations always perform recursive partitioning regardless of order, causing extra overhead.
Hence, Timsort outperforms Quicksort both in theory (due to better adaptation) and in practice, as reflected in the timing table.
