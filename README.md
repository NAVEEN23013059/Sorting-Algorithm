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
```py 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: NAVEEN.S
RegisterNumber: 23013059
'''
def selection_sort(arr):
    # write your code here using selection sort
    n=len(arr)
    for i in range(n):
        min=i
        for j in range(i+1,n):
           if arr[j]<arr[min]:
               min=j
        arr[i],arr[min]=arr[min],arr[i]
    
list_of_nums = eval(input())
# use the selection sort function
# print the sorted list
selection_sort(list_of_nums)
print(list_of_nums)





```
ii)	#Insertion Sort
```py
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: NAVEEN.S
RegisterNumber: 23013059
'''
def selection_sort(arr):
    # Write your code here selection sort
    n=len(arr)
    for i in range(1,n):
        key=arr[i]
        j=i-1
        while j>=0 and key<arr[j]:
            arr[j+1]=arr[j]
            j-=1
        arr[j+1]=key
list_of_nums = eval(input())
# use the insertion sort function to get the sorted list
# print the sorted list
selection_sort(list_of_nums)
print(list_of_nums)






```

## Output:
![output](![Alt text](image.png))
![output](![Alt text](image-1.png))


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
