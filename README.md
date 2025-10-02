
# Stack in C++

## Theory

A **Stack** is a linear data structure that follows the **LIFO (Last In, First Out)** principle.

This means that the **last element inserted** is the **first one removed**.

All insertions and deletions happen at one end, called the **top**. A **top pointer** keeps track of the current topmost element.

* If an element is pushed into a full stack → **Stack Overflow** occurs.
* If an element is popped from an empty stack → **Stack Underflow** occurs.

Stacks are widely used in real-world applications such as:

* **Function call management** (call stack in programming languages).
* **Undo/Redo operations** in text editors.
* **Expression evaluation** in compilers.
* **Backtracking algorithms** (e.g., maze solving, recursion).

---

## Key Operations

### Push

* Inserts an element at the top.
* If the stack is full → **Stack Overflow**.

### Pop

* Removes the topmost element.
* If the stack is empty → **Stack Underflow**.

---

## Characteristics of Stack

* **Linear Data Structure** → Elements arranged sequentially.
* **LIFO Principle** → Last element added is the first removed.
* **Top Pointer** → Tracks the current top element.
* **Fixed Size (Array Implementation)** → Has a maximum capacity.

---

## Applications of Stack

* **Function Call Management** → Call stack manages execution and return of functions.
* **Expression Evaluation** → Used in conversion/evaluation of infix, postfix, prefix expressions.
* **Undo/Redo Operations** → Stores previous states in editors and graphics software.
* **Memory Management** → Stack memory stores local variables and call info.
* **Backtracking Algorithms** → Recursion, parsing, maze solving, etc.

---

## Algorithm

### Push Operation

1. Start.
2. Check if the stack is full (`top >= MAX - 1`).

   * If yes → display `"Stack Overflow"` and stop.
3. Increment `top` by 1.
4. Insert new element at `arr[top]`.
5. Display success message.
6. Stop.

### Pop Operation

1. Start.
2. Check if the stack is empty (`top < 0`).

   * If yes → display `"Stack Underflow"` and stop.
3. Display the element at `arr[top]`.
4. Decrement `top` by 1.
5. Stop.

---

## Conclusion

This experiment demonstrated the **stack data structure** and its **LIFO behavior**:

* **Push** adds an element at the top.
* **Pop** removes the topmost element.
* **Overflow/Underflow** conditions highlight the need for boundary checks.
* Stacks are fundamental in programming and real-world applications such as function call management, expression evaluation, memory management, and algorithm design.
* Using arrays, stacks can be implemented efficiently with **fixed-size memory allocation**, suitable when the maximum number of elements is known.
