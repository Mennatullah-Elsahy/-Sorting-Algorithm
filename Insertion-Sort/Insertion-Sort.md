# Characteristics of Insertion Sort:
* This algorithm is one of the simplest algorithm with simple implementation
* Basically, Insertion sort is efficient for small data values
* Insertion sort is adaptive in nature, i.e. it is appropriate for data sets which are already partially sorted.

# Working of Insertion Sort algorithm:
Consider an example:
arr= {12, 11, 13, 5, 6}
![image](https://user-images.githubusercontent.com/100795596/206428082-3d26704c-2d51-4dde-be24-c4b1f14a365f.png)

## First Pass:
* Initially, the first two elements of the array are compared in insertion sort.
![image](https://user-images.githubusercontent.com/100795596/206428252-15ddf761-2103-41c6-8041-170cc120e98e.png)

* Here, 12 is greater than 11 hence they are not in the ascending order and 12 is not at its correct position. Thus, swap 11 and 12.
* So, for now 11 is stored in a sorted sub-array.
![image](https://user-images.githubusercontent.com/100795596/206428793-3a7074c7-12cc-43fa-a4f5-7a633c3401e4.png)

## Second Pass:
* Now, move to the next two elements and compare them
![image](https://user-images.githubusercontent.com/100795596/206428993-272cd903-39fa-4a1b-ae5b-2344f03f7944.png)
* Here, 13 is greater than 12, thus both elements seems to be in ascending order, hence, no swapping will occur. 12 also stored in a sorted sub-array along with 11

## Third Pass:
* Now, two elements are present in the sorted sub-array which are 11 and 12
* Moving forward to the next two elements which are 13 and 5


