# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**

A process is an independent program that has its own memory space and resources, while a thread is a smaller unit of execution within a process. 
Threads share the same memory which makes communication between them faster and easier. 
Processes, on the other hand are heavier and take more time to create and manage. 
In this assignment, threads were used because they are more efficient for simulating multiple tasks running at the same time. 
Using threads also reduces overhead and improves performance compared to using separate processes.
---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**
 it is moved back to the ready queue. 
This allows other processes to use the CPU before it gets another turn. 
The process will continue execution in the next cycle when it reaches the front of the queue again. 
This behavior ensures fairness and prevents any single process from dominating the CPU time.
Example from my output:
P1 executed for 2000 ms, remaining time: 3000 ms  
P1 is added back to the ready queue  
```

**Explanation of example:**
This shows that P1 used its time quantum but still had remaining work, so it was re-queued to continue later.
---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

[Write your answer here. For each state, explain when P1 enters that state during the simulation. Use your understanding of the code to trace through the lifecycle.]

1. **New**: The thread is created but has not started yet.    

2. **Runnable**:The thread enters this state after calling start() and is ready to run.

3. **Running**:  The thread is actively executing on the CPU

4. **Waiting**:  The thread may enter this state when sleep() is called during execution.

5. **Terminated**:  The thread reaches this state when it finishes execution and no longer runs

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: [Web Server ]    
**Description**: 
A web server handles multiple client requests at the same time.

**Why Round-Robin works well here**: 
It ensures that each request gets a fair share of CPU time and improves responsiveness

### Example 2: [Mobile Applications]

**Description**: 
Mobile apps run tasks like loading data and updating the user interface simultaneously
**Why Round-Robin works well here**: 
It allows smooth performance by switching between tasks quickly and fairly.

---

## Summary

**Key concepts I understood through these questions:**
1. The difference between threads and processes  
2. How Round-Robin scheduling distributes CPU time  
3. The lifecycle of a thread   

**Concepts I need to study more:**
1. Thread synchronization techniques  
2. Advanced CPU scheduling algorithms
