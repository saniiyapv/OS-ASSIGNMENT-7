Description of SJF (Non-Preemptive) Scheduling Program

The program sjf.c implements the Shortest Job First (SJF) Non-Preemptive CPU Scheduling algorithm, which is used by operating systems to schedule processes efficiently.

🔹 What is SJF Scheduling?

SJF is a scheduling algorithm where the process with the smallest burst time (execution time) is selected for execution next.

Non-preemptive means once a process starts executing, it cannot be interrupted until it finishes.

The goal is to minimize average waiting time.

🔹 How the Program Works

Input Phase

The user enters the number of processes n.

For each process:

Process ID (PID)

Arrival Time (AT)

Burst Time (BT)

Process Selection

At any given time, the program selects the process:

That has already arrived (AT ≤ current time)

Has the smallest burst time among available processes

Execution

The selected process runs completely (non-preemptive).

The system time is updated after execution.

Time Calculations

Waiting Time (WT) = Start Time − Arrival Time

Turnaround Time (TAT) = Waiting Time + Burst Time

Repeat

Steps continue until all processes are completed.

🔹 Output Generated

The program displays:

Waiting Time for each process

Turnaround Time for each process

Average Waiting Time

Average Turnaround Time

🔹 Key Features

Uses a structure to store process details.

Dynamically selects the shortest job among arrived processes.

Handles cases where CPU is idle (no process has arrived yet).

Efficient for minimizing waiting time compared to FCFS.

🔹 Advantages

✔ Reduces average waiting time
✔ Efficient for batch processing systems
✔ Simple to implement
