# # 📚 Stack using Linked List: Check and Display Whether the Stack is Full or Not

This Python program demonstrates how to check if a stack (using `LifoQueue` from the `queue` module) is full or not. It uses the `full()` method to determine the stack's status and then displays the appropriate message.

## 🎯 Aim

To write a Python program that:
- Creates a stack (jar) using the LifoQueue class.
- Adds a fixed number of snack items to the stack.
- Displays the total quantity of snacks and checks whether the jar is full.
- Simulates sales by removing items from the stack.
- Checks and displays whether the jar is empty after sales.

## 🧠 Algorithm

1. **Import the LifoQueue class**

   * Import `LifoQueue` from the `queue` module to implement the stack.

2. **Create a Stack (Jar)**

   * Instantiate a `LifoQueue` object with a maximum size of 8.

3. **Add Snack Items to the Stack**

   * Use the `put()` method to add snack items (e.g., 'Snack_1', 'Snack_2', etc.) to the stack.

4. **Display Current Quantity and Full Status**

   * Use the `qsize()` method to show the current number of items in the jar.
   * Use the `full()` method to check if the jar (stack) is full.

5. **Simulate Snack Sales**

   * Remove items using the `get()` method to represent snacks being sold.

6. **Check and Display Empty Status**

   * Use the `empty()` method to check if the jar is empty.
   * Display the remaining number of snacks using `qsize()`.

## 📝 Program
```
from queue import LifoQueue

stack = LifoQueue(maxsize=8)

stack.put('Snack_1')
stack.put('Snack_2')
stack.put('Snack_3')
stack.put('Snack_4')
stack.put('Snack_5')

print("Present quantity of snacks in the jar: ",stack.qsize(), end=" Snacks")
print("\nIs the jar full? ", stack.full())

print('\nAfter sales:')
print(stack.get())
print(stack.get())
print(stack.get())

print("\nIs the jar empty? ", stack.empty())
print("Current quantity of snacks in the jar: ", stack.qsize(), end=" Snacks")
```

## Sample Input & Output

<img width="1049" height="372" alt="image" src="https://github.com/user-attachments/assets/040bbd78-0ea1-4a68-aea2-4e29fbc300c2" />

## Result
The program successfully demonstrates stack operations using the `LifoQueue` class in Python. It shows how to:

* Add elements (push) into the stack,
* Remove elements (pop) from the stack, and
* Check whether the stack is **full** or **empty** using built-in methods.
