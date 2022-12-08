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
* Now, move to the next two elements and compare them.

![image](https://user-images.githubusercontent.com/100795596/206428993-272cd903-39fa-4a1b-ae5b-2344f03f7944.png)

* Here, 13 is greater than 12, thus both elements seems to be in ascending order, hence, no swapping will occur. 12 also stored in a sorted sub-array along with 11.

## Third Pass:
* Now, two elements are present in the sorted sub-array which are 11 and 12.
* Moving forward to the next two elements which are 13 and 5.

![image](https://user-images.githubusercontent.com/100795596/206431465-1927aa0a-e81f-4a80-b8ed-728e29ba94b9.png)

* Both 5 and 13 are not present at their correct place so swap them.

![image](https://user-images.githubusercontent.com/100795596/206431749-d2be6bdf-a163-421e-893c-662886df2948.png)

* After swapping, elements 12 and 5 are not sorted, thus swap again.

![image](https://user-images.githubusercontent.com/100795596/206431926-a458620e-de40-45b1-b51e-e9412685439c.png)

* Here, again 11 and 5 are not sorted, hence swap again.

![image](https://user-images.githubusercontent.com/100795596/206432081-1e0a7644-1113-41eb-b408-f622811e5fec.png)

* here, it is at its correct position.

## Fourth Pass:
* Now, the elements which are present in the sorted sub-array are 5, 11 and 12.
* Moving to the next two elements 13 and 6.

![image](https://user-images.githubusercontent.com/100795596/206432389-f5b4871b-06fe-4d2f-a0a2-ad3a691f201b.png)

* Clearly, they are not sorted, thus perform swap between both.

![image](https://user-images.githubusercontent.com/100795596/206432522-52297b3e-8624-4b38-94ba-d344452c1fc1.png)

* Now, 6 is smaller than 12, hence, swap again.

![image](https://user-images.githubusercontent.com/100795596/206432645-77fdb1b8-5877-4f2b-8896-77eee68dff79.png)

* Here, also swapping makes 11 and 6 unsorted hence, swap again.

![image](https://user-images.githubusercontent.com/100795596/206432743-8b46b6e7-afab-4ea1-99a4-a63ba61e382f.png)

* Finally, the array is completely sorted.

### Illustrations:

![image](https://user-images.githubusercontent.com/100795596/206433548-448f6a85-7f3b-489a-9af1-29e31da2e2ba.png)


### So to sort an array of size N in ascending order: 

* Iterate from arr[1] to arr[N] over the array. 
* Compare the current element (key) to its predecessor. 
* If the key element is smaller than its predecessor, compare it to the elements before. Move the greater elements one position up to make space for the swapped element.
