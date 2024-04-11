Problem Statement: <br>
The goal of this project is to simulate a process scheduler in an operating system. The process scheduler is responsible for selecting the next process to be executed by the CPU based on a specific scheduling algorithm. The project aims to implement and compare different scheduling algorithms to understand their behavior and performance.<br>

Objectives: 

1. Implement the following CPU scheduling algorithms:
    * First-Come, First-Served (FCFS)
    * Shortest Job First (SJF)
    * Priority Scheduling
    * Round Robin (RR)

2. Simulate the execution of processes using each scheduling algorithm and collect performance metrics such as:
    * Average waiting time
    * Average turnaround time
    * CPU utilization
3. Analyze the results and compare the performance of different scheduling algorithms under various workload scenarios. <br>

Implementation Steps:

1. Define the process structure:
    * Create a data structure to represent a process, including attributes like process ID, arrival time, burst time, priority, and other relevant information.

2. Implement the scheduling algorithms:
    * FCFS: Execute processes in the order of their arrival.
    * SJF: Execute processes with the shortest burst time first.
    * Priority Scheduling: Execute processes based on their priority.
    * Round Robin: Execute processes in a time-sliced manner, giving each process a fixed time quantum.

3. Create a queue or list to hold the processes:
    * Maintain a queue or list to store the processes waiting to be executed.
    * Implement functions to add processes to the queue and remove processes from the queue based on the scheduling algorithm.

4. Simulate the process execution:
    * Create a function to simulate the execution of processes based on the selected scheduling algorithm.
    * Keep track of the current time and update the waiting time and turnaround time of each process accordingly.
    * Simulate the execution of processes until all processes are completed.

5. Collect performance metrics:
    * Calculate the average waiting time by summing up the waiting times of all processes and dividing by the total number of processes.
    * Calculate the average turnaround time by summing up the turnaround times of all processes and dividing by the total number of processes.
    * Calculate the CPU utilization by dividing the total time the CPU is busy by the total simulation time.

6. Provide a user interface:
    * Create a simple command-line or graphical user interface to allow the user to input the process details (arrival time, burst time, priority) and select the scheduling algorithm.
    * Display the simulation results, including the performance metrics and the order in which processes were executed.

Testing and Verification:

1. Create test cases with different process workloads and scheduling algorithms.
2. Verify that the implemented scheduling algorithms produce the expected execution order of processes.
3. Compare the calculated performance metrics with the expected theoretical values for each scheduling algorithm.
4. Test edge cases, such as processes with the same arrival time, same burst time, or same priority, to ensure the scheduler handles them correctly.
5. Validate that the simulation results match the expected behavior of each scheduling algorithm.
