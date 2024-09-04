Praveen Anand
1002219407

Hands-On 2
Implement:

1. insertion sort

2. selection sort

3. bubble sort

 

In the discussion:

1. Post a link to your github repository(s) with the source code.

2. Argue selection sort correctness.

3. Benchmark the runtime of each algorithm. Your benchmarks should include information about your computer (ram, cpu etc.) and be run with various input sizes; from small (array of size 5,10,20) all the way up to large arrays (where your computer is struggling). I should at the very least see a plot of time vs input size n. Feel free to use benchmarking software.

 Answer:
 Argue selection sort correctness.
 
 Selection sort is a basic sorting algorithm that continually picks the minimum or maximum of an element and moves it to the beginning of the sorted segment. 

Argument for its correctness:
*Initialization:
    At the starting point of the procedure, the sorted section of the array is empty, while the unsorted portion has all of the entries. As a result, the invariant holds trivially at the beginning.

*Maintenance:
    On every iteration, the selection sort chooses the smallest element from the unsorted segment and replaces it with the initial element in the unsorted portion. The primary element from the unsorted segment is then included in the sorted portion. The size of the sorted section rises by one, while the unsorted portion reduces by one.  Thus, after each iteration, the array is sorted up to the current entry. 

*Termination:
    The algorithm terminates when the entire array is sorted. 

*Time complexity:
    The time complexity of selection sort is O(n^2), where n is the number of elements in the array. 
    To locate the minimal element, selection sort scans the remaining unsorted section linearly. Despite its simplicity, selection sort is less effective on massive data sets than more complicated sorting algorithms.

To summarize, selection sort is a valid sorting algorithm that maintains the invariant of having a sorted component at the start of the array and an unsorted piece at the very end. Its soundness may be questioned based on the startup, maintenance, and termination phases, and its time complexity is well-defined, if less effective than certain alternative sorting algorithms.


System Specifications:

CPU: 11th Gen Intel(R) Core(TM) i5-1135G7 @ 2.40GHz   2.42 GHz

RAM: 16 GB

OS: Windows 11 Home

Python version: 3.10
