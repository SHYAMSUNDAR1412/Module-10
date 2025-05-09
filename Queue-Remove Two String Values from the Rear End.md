# Queue-Remove Two String Values from the Rear End in Python 🧵

This Python program demonstrates how to manage a list of strings and remove the last two elements (i.e., from the rear of the list).

## 🎯 Aim

To write a Python program to:
- Accept `n` string values from the user
- Remove the last two values (rear end of the list)
- Display the updated list

## 🧠 Algorithm

1. Create an empty list `q`.
2. Read an integer `n` from the user (number of strings).
3. Loop `n` times:
   - Read a string input.
   - Append it to the list `q`.
4. Remove the last element using `pop()`.
5. Remove the next last element using `pop()` again.
6. Display the updated list.

##  Program:
q = []
n=int(input())
for i in range(n):
   q.append(input()) 
q.pop(0)
q.pop(0) 
print(q)

### Output:
![image](https://github.com/user-attachments/assets/d99ac0cc-4906-4746-9e8e-ce55570f8698)


## Result:
Thus the program has been successfully executed..
