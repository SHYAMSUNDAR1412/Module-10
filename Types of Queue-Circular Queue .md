# 🔄 Types of Queue-Circular Queue in Python

This project demonstrates the implementation of a **Circular Queue** in Python. The queue accepts 3 user values, performs enqueue and dequeue operations, and displays the removed values.

---

## 🎯 Aim

To develop a Python program that implements a Circular Queue:
- Accepts 3 values from the user
- Removes the 3 values from the queue
- Displays the removed values

---

## 🧠 Algorithm

1. **Initialize** a circular queue of fixed size (e.g., 5).
2. **Define the following functions**:
   - `enqueue()`: Inserts an element into the queue.
   - `dequeue()`: Removes an element from the queue.
   - `display()`: Shows the queue contents.
3. Accept 3 values from the user using the `enqueue()` method.
4. Remove 3 values using the `dequeue()` method.
5. Print the removed values.

---

## 💻 Program:
class CircularQueue:
 def __init__(self, size):
    self.size = size
    self.queue = [None] * size
    self.front = -1
    self.rear = -1
def enqueue(self, value):
    if ((self.rear + 1) % self.size == self.front):
       print("Queue is Full!")
    elif self.front == -1:
       self.front = 0
       self.rear = 0
       self.queue[self.rear] = value
    else:
       self.rear = (self.rear + 1) % self.size
       self.queue[self.rear] = value
 def dequeue(self):
       if self.front == -1:
          print("Queue is Empty!")
          return None
          removed_value = self.queue[self.front]
       if self.front == self.rear:
          self.front = -1
          self.rear = -1
       else:
          self.front = (self.front + 1) % self.size
          return removed_value
 def display(self):
      if self.front == -1:
          print("Queue is Empty!")
       else:
          print("Queue contents:")
          i = self.front
      while True:
         print(self.queue[i], end=" ")
         if i == self.rear:
            break
         i = (i + 1) % self.size
      print()
# Main code
cq = CircularQueue(5)
# Enqueue values from user
for i in range(5):
 val = input(f"Enter value {i+1}: ")
 cq.enqueue(val)
print("\nInitial queue:")
cq.display()
# Dequeue 3 elements
print("\nRemoving 3 elements from the queue:")
for i in range(3):
 removed = cq.dequeue()

### Output:
![image](https://github.com/user-attachments/assets/60643abf-13d8-4363-9c52-b830a84d281c)
![image](https://github.com/user-attachments/assets/685187c2-defb-41b8-a639-5192fe50824d)

## Result:
Thus the program has been successfully executed
