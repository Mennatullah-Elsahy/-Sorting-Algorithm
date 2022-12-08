# Working of Merge Sort algorithm:
Think of it as a recursive algorithm continuously splits the array in half until it cannot be further divided. This means that if the array becomes empty or has only one element left, the dividing will stop, i.e. it is the base case to stop the recursion. If the array has multiple elements, split the array into halves and recursively invoke the merge sort on each of the halves. Finally, when both halves are sorted, the merge operation is applied. Merge operation is the process of taking two smaller sorted arrays and combining them to eventually make a larger one.

# Illustration:
To know the functioning of merge sort, lets consider an array:
arr= {38, 27, 43, 3, 9, 82, 10}

* At first, check if the left index of array is less than the right index, if yes then calculate its mid point.

![image](https://user-images.githubusercontent.com/100795596/206437380-cbf721c1-cd84-4660-8cfc-377b0764b359.png)

* Now, as we already know that merge sort first divides the whole array iteratively into equal halves, unless the atomic values are achieved. 
* Here, we see that an array of 7 items is divided into two arrays of size 4 and 3 respectively.

![image](https://user-images.githubusercontent.com/100795596/206437474-27716fc4-1b16-4abf-baec-f7cf8a4da4dc.png)

* Now, again find that is left index is less than the right index for both arrays, if found yes, then again calculate mid points for both the arrays.

![image](https://user-images.githubusercontent.com/100795596/206437561-9f753ae4-6fa8-400d-bdcd-b32e8d90d068.png)

* Now, further divide these two arrays into further halves, until the atomic units of the array is reached and further division is not possible.

![image](https://user-images.githubusercontent.com/100795596/206437616-7bad2a3b-f2f8-4304-be50-2ea532d6ac53.png)

* After dividing the array into smallest units, start merging the elements again based on comparison of size of elements.
* Firstly, compare the element for each list and then combine them into another list in a sorted manner.

![image](https://user-images.githubusercontent.com/100795596/206437740-80e2f370-a595-40ee-ada5-f60f5b85ea37.png)

* After the final merging, the list looks like this:

![image](https://user-images.githubusercontent.com/100795596/206437849-050b05a8-fabc-4721-8269-077f134c8b2e.png)



#### The following diagram shows the complete merge sort process for an example array {38, 27, 43, 3, 9, 82, 10}. 

#### If we take a closer look at the diagram, we can see that the array is recursively divided into two halves till the size becomes 1. Once the size becomes 1, the merge processes come into action and start merging arrays back till the complete array is merged.

![image](https://user-images.githubusercontent.com/100795596/206438481-a7e935b7-c7bd-4503-b818-8613e66679e5.png)



