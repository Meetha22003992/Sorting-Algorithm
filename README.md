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
def selection_sort(num):
    for i in range(len(num)):
        lowest_value_index=i
        for j in range(i+1,len(num)):
            if num[j]<num[lowest_value_index]:
                lowest_value_index=j
        num[i],num[lowest_value_index]=num[lowest_value_index],num[i]
list_of_num=eval(input())
selection_sort(list_of_num)
print(list_of_num)
```
ii)	#Insertion Sort
```
def insertion_sort(num):
    for i in range(1,len(num)):
        item_to_insert=num[i]
        j=i-1
        while j>=0 and num[j]>item_to_insert:
            num[j+1]=num[j]
            j-=1
        num[j+1]=item_to_insert
list_of_num = eval(input())
# use the insertion sort function to get the sorted list
insertion_sort(list_of_num)
print(list_of_num)
# print the sorted list
```

## Output:
![image](https://github.com/Meetha22003992/Sorting-Algorithm/assets/119401038/865531ab-2939-45bb-a1c2-8222a33ea4db)

![image](https://github.com/Meetha22003992/Sorting-Algorithm/assets/119401038/e99d48c6-c379-4c1c-bbf0-37168c500a91)
## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
