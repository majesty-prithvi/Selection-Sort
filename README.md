# Selection-Sort<br>
Selection sort is a simple and efficient sorting algorithm that works by repeatedly selecting the smallest (or largest) element from the unsorted portion of the list and moving it to the sorted portion of the list. The algorithm repeatedly selects the smallest (or largest) element from the unsorted portion of the list and swaps it with the first element of the unsorted portion. This process is repeated for the remaining unsorted portion of the list until the entire list is sorted. One variation of selection sort is called “Bidirectional selection sort” which goes through the list of elements by alternating between the smallest and largest element, this way the algorithm can be faster in some cases.<br>
<br>
![image](https://user-images.githubusercontent.com/125802204/234185331-b287fd84-43aa-483c-847a-c764f8257f83.png)
<br>
<b>The algorithm maintains two subarrays in a given array.</b>

The subarray which already sorted.<br> 
The remaining subarray was unsorted.<br>
In every iteration of the selection sort, the minimum element (considering ascending order) from the unsorted subarray is picked and moved to the beginning of the sorted subarray. <br>

After every iteration sorted subarray size increase by one and the unsorted subarray size decrease by one.<br>
After the N (size of the array) iteration, we will get a sorted array.<br>
<br>
# Steps to solve the problem are:<br>

1.Initialize minimum value(min_idx) to location 0.<br>
2.Traverse the array to find the minimum element in the array.<br>
3.While traversing if any element smaller than min_idx is found then swap both values.<br>
4.Then, increment min_idx to point to the next element.<br>
5.Repeat until the array is sorted.<br>
<br>
<b><ins> Output </b></ins>
<br>
<img width="922" alt="Selection sort" src="https://user-images.githubusercontent.com/125802204/234187200-a76f8e32-93fd-4f5d-8c23-1cd537cfe3b1.png">
<br>
<b>Time Complexity:</b> The time complexity of Selection Sort is O(N2) as there are two nested loops:<br>

One loop to select an element of Array one by one = O(N)<br>
Another loop to compare that element with every other Array element = O(N)<br>
Therefore overall complexity = O(N) * O(N) = O(N*N) = O(N2)<br>

<b>Auxiliary Space: </b>O(1) as the only extra memory used is for temporary variables while swapping two values in Array. The selection sort never makes more than O(N) swaps and can be useful when the memory write is a costly operation. <br>
