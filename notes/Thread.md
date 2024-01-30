# Understanding Programs, Processes, and Threads

📝 **Program:**

- **Definition (Simplified):** A program is like a recipe book 📖. It contains a set of instructions in a programming language. It's static and doesn't actively do anything on its own.
- **Official Definition:** A program is a collection of instructions that can be executed by a computer to perform a specific task. It is typically stored in a file on a storage device and becomes a process when loaded into memory.

🔄 **Process:**

- **Definition (Simplified):** A process is like a chef 🍳 following a recipe. It's an active, running instance of a program. When loaded into computer memory, it has its own space and resources for execution.
- **Official Definition:** A process is an independent program in execution, with its own memory space, resources, and program counter. It is the basic unit of execution in a computer's operating system.

- **Components of a Process:**
  - **Stack:** Holds temporary data and function information.
  - **Data Section:** Contains global variables.
  - **Heap:** Dynamically allocated memory during runtime.

🔄 **Thread:**

- **Definition (Simplified):** A thread is like a single cook 🧑‍🍳 in the kitchen, each working on a specific task. It's the smallest unit of execution managed by the operating system. Threads within a process share the same resources but run independently.
- **Official Definition:** A thread is the smallest unit of execution within a process. It consists of a program counter, a register set, and a stack. Threads within the same process share the same code and data sections but have their own program counters and registers.

- **Differences with Process:**
  - **Creation/Termination:**
    - Thread: Easier to create and terminate.
    - Process: Not as easy to create and terminate.
  - **Communication:**
    - Thread: Easier to communicate between threads within the same process.
    - Process: Requires operating system intervention for communication.
  - **Context Switching:**
    - Thread: Faster context switching.
    - Process: Slower context switching.
  - **Weight:**
    - Thread: Lightweight, as threads within a process share resources.
    - Process: Heavyweight, as each process has its own set of resources.

🔄 **Types of Processes:**

- **I/O Bound Process:**

  - **Definition (Simplified):** If a program spends more time waiting for input/output operations than doing computations, it's called an I/O bound process 🔄.
  - **Official Definition:** An I/O bound process is a type of process that spends more time waiting for input/output operations to complete than performing actual computations.

- **CPU Bound Process:**
  - **Definition (Simplified):** If a program spends more time doing computations and infrequently needs input/output operations, it's called a CPU bound process ⚙️.
  - **Official Definition:** A CPU bound process is a type of process that primarily engages in computations and generates input/output requests infrequently.

### Summary:

- A program is a set of instructions on a hard disk.
- When a program runs in the computer's memory, it becomes a process.
- A thread is the smallest unit of execution, and multiple threads can exist within a process.
- There are two main types of processes: I/O bound (waiting for external operations) and CPU bound (doing a lot of computations).
