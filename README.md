# Experiment-5
### Name : VASANTHAN,N
### Reg no. : 212224240180

## AIM:
Write a python program for Binary Search and inspect for failures. 

# ALGORITHM

1. Start the program.
2. Get the list from the user
3. Get the element to be searched
4. Compare the mid element with the key, if same return the index
5. If key is greater, search it in the right side, else search it in the left side.
6. If not found return -1
7. Stop the program. 

# PROGRAM

```python
def binary_search(arr, x):
    low = 0
    high = len(arr) - 1
    mid = 0
    while low <= high:
        mid = (high + low) // 2
        if arr[mid] < x:
            low = mid + 1
        elif arr[mid] > x:
            high = mid - 1
        else:
            return mid 
    return -1 
arr = [2, 3, 4, 10, 40]
try:
    x = int(input("Enter the element to be searched: ")) 
    result = binary_search(arr, x)
    if result != -1:
        print("Element is present at index", str(result))
        print("Test Case:Pass")
    else:
        print("Element is not present in array")
        print("Test Case:Pass")
except ValueError:  
    print("Enter a valid input!")
    print("Test Case:Fail")
```
# OUTPUT

<img width="412" height="138" alt="image" src="https://github.com/user-attachments/assets/be6c437b-d856-4441-95ea-f085b045ab80" />

<img width="421" height="145" alt="image" src="https://github.com/user-attachments/assets/8012592e-ee6a-4b57-b303-44fa67ba029b" />

<img width="422" height="147" alt="image" src="https://github.com/user-attachments/assets/52b6701c-6984-416b-94a5-b2d5ae32fb36" />

<img width="410" height="142" alt="image" src="https://github.com/user-attachments/assets/32a1c3ae-b5a2-455e-939b-934e939d9bc8" />

<img width="436" height="144" alt="Screenshot 2025-08-29 101651" src="https://github.com/user-attachments/assets/f19193d5-0991-4bed-a274-91b5f6c896c9" />

<img width="440" height="142" alt="image" src="https://github.com/user-attachments/assets/707ee20a-db1f-4cd9-812e-c1d9e1e032c6" />

# RESULT
Thus, the python program of binary search is implemented and the output is verified successfully.
