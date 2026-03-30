# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**
So basically a process is just a whole program that runs on its own with its own memory. But threads are a bit different because they live inside the process and share all the memory and stuff together. We actually went with threads for this task because they are much lighter and don't take much work to start up. The best part is they can talk to each other super fast, and this is exactly what we need when we want to switch between different jobs in our simulation.

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**
In a Round-Robin setup, if a process uses up its time quantum but still has more work to do, it just goes straight to the back of the Ready Queue. We do this mainly to keep things fair for everyone; it stops one huge process from hogging the CPU and making every other process wait. By putting it back in line like that, everyone gets a small turn. My program shows this when P1 leaves the CPU because it needed more time, so P2 and P3 finally got a chance to run.
Example from my output:
 ? P1 executing quantum [4000ms] 
  ? Quantum progress: [???????????????] 100%
  ? P1 completed quantum 4000ms ? Overall progress: [????????????????????] 50%
     Remaining time: 3905ms
  ? P1 yields CPU for context switch

  ? P1 added to ready queue ? Burst time: 7905ms

  Explanation of example:
If you look at my output, P1 finished its 4000ms turn but still had a bit of work left to finish. So the system did a context switch and pushed P1 to the end of the line. This is how the scheduler makes sure no one has to wait for too long to get their turn.






---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

[Write your answer here. For each state, explain when P1 enters that state during the simulation. Use your understanding of the code to trace through the lifecycle.]

1. **New**: [When is P1 in New state?]

2. **Runnable**: [When does P1 become Runnable?]

3. **Running**: [When is P1 Running?]

4. **Waiting**: [When/why would P1 be Waiting?]

5. **Terminated**: [When is P1 Terminated?]

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: [Name of application/scenario]

**Description**: 
[Describe the real-world scenario or application]

**Why Round-Robin works well here**: 
[Explain why Round-Robin scheduling is suitable. Consider fairness, responsiveness, predictability, etc.]

### Example 2: [Name of application/scenario]

**Description**: 
[Describe the real-world scenario or application]

**Why Round-Robin works well here**: 
[Explain why Round-Robin scheduling is suitable. Consider fairness, responsiveness, predictability, etc.]

---

## Summary

**Key concepts I understood through these questions:**
1. 
2. 
3. 

**Concepts I need to study more:**
1. 
2. 
