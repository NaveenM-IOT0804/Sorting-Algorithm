# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: Naveen M
RegisterNumber: 22000748

def selection_sort(list_of_nums):
    n = len(list_of_nums)
    for i in range(n): 
        min_idx = i 
        for j in range(i+1, n): 
            if list_of_nums[min_idx] > list_of_nums[j]: 
                min_idx = j 
        list_of_nums[i], list_of_nums[min_idx] = list_of_nums[min_idx], list_of_nums[i] 
    return list_of_nums
list_of_nums = eval(input())
print(selection_sort(list_of_nums))

```
ii)	#Insertion Sort
```

''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: Naveen M
RegisterNumber: 22000748
'''

def insertion_sort(list): 
    for i in range(1, len(list)): 
        currentValue = list[i] 
        position = i 
  
        while position > 0 and list[position - 1] > currentValue: 
            list[position] = list[position - 1] 
            position = position - 1
  
        list[position] = currentValue 

list = eval(input())
insertion_sort(list)
print(list)




```

## Output:

Selection sort:

![ss1](https://user-images.githubusercontent.com/117974950/213972809-ea280fe2-ac43-4172-8079-1b68b0c49e9a.png)


Insertion sort:

![ss2](https://user-images.githubusercontent.com/117974950/213972851-80d02cc6-5dd3-4b81-a391-ba6cdf7e08be.png)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
