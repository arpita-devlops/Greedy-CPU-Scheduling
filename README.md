This project provides an implementation of various CPU scheduling algorithms in C++, including First Come First Serve (FCFS), Round Robin (RR), Shortest Process Next (SPN), Shortest Remaining Time (SRT), Highest Response Ratio Next (HRRN), Feedback (FB), and Aging.

Algorithms Overview
1. First Come First Serve (FCFS):
Non-preemptive: Executes processes in the order they arrive.
Simple but inefficient with long burst times, leading to poor performance.

2. Round Robin (RR) with Varying Time Quantum
Time-sharing approach where processes receive a fixed time slice.
More efficient with variable quantum, improving waiting times and preventing starvation.

3. Shortest Process Next (SPN)
Non-preemptive: Prioritizes processes with the shortest burst time.
Reduces average waiting time but may cause longer processes to wait.


4. Shortest Remaining Time (SRT)
Preemptive version of SPN, where a process can be interrupted by one with a shorter remaining time.
Minimizes average waiting time and adapts when burst times are unknown.


5. Highest Response Ratio Next (HRRN)
Non-preemptive: Prioritizes processes based on their response ratio (waiting time/burst time).
Efficient for minimizing waiting time and works well when burst times are unknown.


6. Feedback (FB)
Multi-level priority scheduling: Processes are assigned to different priority queues.
Suitable for handling processes with different priorities and burst times.


7. Feedback with Varying Time Quantum (FBV)
Similar to Feedback but with different time slices for each priority level.


8. Aging
Increases the priority of waiting processes to prevent starvation.
Gradually boosts lower-priority processes to ensure execution.
