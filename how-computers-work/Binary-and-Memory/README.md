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

##### Characteristics:
  * Memory is created automatically
  * Memory is freed automatically when function end
  * Limited size
  * Follows Last In, First Out

---

- #### What is Heap?
  * Dynamic memory
  * Used for manual memory reservation
 
  ⚠️​ Memory must be freed manually

##### Characteristics:
  * Slower than stack
  * Much larger than stack

> [!NOTE]
> Stack errors → stack overflow
> Heap errors → memory leaks

---

### ⚠️ Segmentation Fault
This happens when a program tries to access or modify a part of memory that it is not allowed to access or
modify.

#### The main causes of the Segmentation Fault:
- Dereferencing NULL Pointer

      int *p = NULL;   // p points to nothing
      *p = 10;

- Array Out-of-Bounds Access

      int arr[5];      // Valid indexes are 0 to 4
      arr[10] = 3;

- Stack Overflow

      void f(void)     // Infinite calls fill the stack → stack overflow
      {
          f();
      }

- Uninitialized Variables

      int x;           // x has no initial value (undefined behavior)
      printf("%d\n", x);

- Dangling Pointer

      int *p = malloc(sizeof(int));
      free(p);
      *p = 5;          // pointer use after free() (undefined behavior)

- Writing to Read-Only Memory

      char *s = "hello";
      s[0] = 'H';       // string cannot be modified because it are in read-only mode.

  
Accessing it causes segmentation fault

---

### ⚠️ Memory Leak
Memory is allocated but never freed.
it causes memory usage increases and Long-running programs become slow or crash.

    int *p = malloc(sizeof(int));
    // free(p) is missing






