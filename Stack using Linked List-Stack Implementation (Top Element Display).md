# 📚 Stack using Linked List: Stack Implementation (Top Element Display)

## 🎯 Aim

To write a Python program that implements a stack using the deque class from the collections module.
The program simulates a rescue operation where rescuers are added to a stack and the top element (last rescuer added) is removed to assist in an emergency.

---

## 🧠 **Algorithm**

1. **Start the program.**
2. **Import** the `deque` class from the `collections` module.
3. **Initialize** an empty stack named `path_hole` using `deque()`.
4. **Push elements** (e.g., ‘Senior Rescuer’, ‘Junior Rescuer’, and ‘Trainee Rescuer’) into the stack using the `append()` method.
5. **Display** all rescuers currently in the path hole.
6. When the **senior rescuer** needs help, **pop** the top element (last rescuer added) using the `pop()` method.
7. **Display** the name of the rescuer who goes to bring the oxygen cylinder.
8. **End the program.**

---

## 💻 Program
```
from collections import deque

path_hole = deque()

path_hole.append('Senior Rescuer')
path_hole.append('Junior Rescuer')
path_hole.append('Trainee Rescuer')

print('Who are all in the path hole for rescue?')
print(path_hole)

print('\nSenior rescuer is short of oxygen.')
print("Who can bring extra oxygen cylinder to help senior rescuer?")
print(path_hole.pop())
```

## Output

<img width="1140" height="243" alt="image" src="https://github.com/user-attachments/assets/99fb6a65-833d-4e28-a62d-f3fe9407f931" />

## Result
The program successfully demonstrates stack operations using the deque class.
It shows how elements are pushed onto and popped from a stack, following the Last-In-First-Out (LIFO) principle.
This real-life analogy of rescuers clearly illustrates how stacks manage data where the last element added is the first to respond or be removed.
