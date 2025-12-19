### What is Binary?
Computers understand only two values: `0` and `1`

Memory stores data in binary, Like (numbers, letters, programs, images ...)

---

### Memory
A running program uses `RAM` memory.

It's divided into two important parts: `Stack` and `Heap`

- #### What is Stack?
  * Automatic memory
  * Very fast
  * Used for local variables and function calls

  > Each time a function is called, a stack frame is created.

Characteristics
  * Memory is created automatically
  * Memory is freed automatically when function end
  * Limited size
  * Follows Last In, First Out

- #### What is Heap?
  * Dynamic memory
  * Used for manual memory reservation
 
  ⚠️​ Memory must be freed manually

Characteristics
  * Slower than stack
  * Much larger than stack

> [!NOTE]
> Stack errors → stack overflow
> Heap errors → memory leaks

---

- ### Stack Overflow?
A stack overflow happens when the stack runs out of space.
 * #### Common Causes

       void f(void)      // Infinite recursion
       {
           f();
       }
   
 > Each call creates a new stack frame → stack fills → crash.

    int arr[10000000];        // Very large local variables

 > Too much memory on the stack → overflow.

 * Very large local variables

---

### ⚠️ Memory Leak

