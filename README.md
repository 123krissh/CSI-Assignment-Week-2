# 🧠 Singly Linked List in Python (OOP-Based)

This project implements a **Singly Linked List** in Python using **Object-Oriented Programming (OOP)** principles. It supports operations such as:

- Adding a node to the end of the list
- Deleting the nth node
- Printing the entire list
- Handling exceptions like deleting from an empty list or invalid index

---

## 📁 Files

| File         | Description                                |
|--------------|--------------------------------------------|
| `LinkedList.py` | Contains the full Python implementation |
| `README.md`      | Explanation of the code and its design |

---

## 🔧 How It Works

The project uses two classes:

### 1. `Node` Class
Represents a single node in the linked list.

```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
```
### 2. `LinkedList` Class
Manages the linked list and provides the main operations.
```python
class LinkedList:
    def __init__(self):
        self.head = None
```

### 3. `add_node(data)`
Adds a new node to the end of the list.

### 4. `print_list()`
Prints all elements of the list in order, formatted like:
10 -> 20 -> 30 -> None

### 5. `delete_nth_node(n)`
Deletes the nth node (1-based index). It includes exception handling:

Raises an error if the list is empty.

Raises an error if the index is invalid (e.g., too large or less than 1).

## ✅ Sample Output

```bash
Added 10 as the head of the list.

Added 20 to the end of the list.

Added 30 to the end of the list.

Added 40 to the end of the list.

Linked List: 10 -> 20 -> 30 -> 40 -> None

Deleted node at position 2 with value 20.

Linked List: 10 -> 30 -> 40 -> None

Error: Index 10 is out of range.

Error: Cannot delete from an empty list.
```

## 👨‍🏫 OOP Principles Used

| Principle      | Description                                                            | Applied In                                  |
|----------------|------------------------------------------------------------------------|---------------------------------------------|
| **Encapsulation** | Data and methods are wrapped inside classes.                        | `Node`, `LinkedList` classes                |
| **Abstraction**   | User interacts with high-level methods, not internal pointer logic. | `add_node()`, `delete_nth_node()`, `print_list()` |
| **Modularity**    | Code is organized into separate, manageable components (classes).   | Separate `Node` and `LinkedList` classes    |
