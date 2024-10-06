**Assignment: Circular Linked List and Linked List Prime Number Calculation**

**Problem 1: Simple Process Scheduling Algorithm**

**Approach:**

The problem is solved using a circular linked list to simulate a round-robin CPU scheduling algorithm. Each process is represented as a node with attributes process_id, execution_time, and remaining_time.
The scheduler assigns a fixed time quantum to each process, reducing its remaining_time per cycle. Processes with zero remaining_time are removed from the list.
The system displays the state of all processes after each cycle.

**Optional Task:**

A new process can randomly arrive while the scheduler is running. This feature is implemented by inserting new nodes during the simulation, with a reduced probability to avoid infinite loops.

**Assumptions:**

-All processes are initialized with their execution_time before starting the scheduler.

-A fixed time quantum is assigned to all processes.

-New processes have a 30% chance of arriving during a cycle, managed via random operations to prevent infinite loops.

-The scheduler runs until all processes complete.

**Challenges:**

-Infinite Loop (Optional Task): Initially, new processes arriving during execution caused an infinite loop. This was resolved by reducing the chance of a new process arriving to 30% using random operations.

-Handling the insertion and deletion of nodes while ensuring the circular linked list structure remains intact.

**Problem 2: Very Large Prime Number Calculation**

**Approach:**

The task is to store and check the primality of a large number split across a singly linked list. The number is divided into 64-bit chunks, each stored in a node.
A deterministic or probabilistic algorithm (Miller-Rabin test) is applied to check the primality of the full number by traversing the list.

**Assumptions:**

-The large number is provided as input, split into parts, and stored in the linked list.

-Arithmetic operations, like addition and modulo, are applied across multiple nodes as part of the primality test.

**Challenges:**

-Time Complexity: Storing large numbers in the linked list and performing arithmetic operations increased the time complexity significantly. As a result, testing the primality of very large numbers took too long.

-Limitation: To optimize the process, the implementation was limited to numbers with up to 5-6 digits for faster results, rather than a full 1024-bit number.

**OUTPUT SCREEN SHOTS;**

**TASK 1:**

![image](https://github.com/user-attachments/assets/d30b2115-bab4-4ae1-ba48-7c029eea2591)

**TASK 2:**

![Screenshot 2024-10-06 153112](https://github.com/user-attachments/assets/d4160daf-30dd-4b00-8b05-fc7257e5cb80)
![Screenshot 2024-10-06 154656](https://github.com/user-attachments/assets/508b0a8e-cfdb-478a-a521-673d90039d53)
