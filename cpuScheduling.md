# CPU Scheduling in Operating System

## What is CPU Scheduling?

CPU Scheduling is the process by which the Operating System decides which process in the ready queue gets access to the CPU.

Since there is only one CPU (in single-core systems) and multiple processes, scheduling is necessary to ensure efficient CPU utilization.

---

# Why CPU Scheduling is Needed

- Multiple processes exist in the Ready Queue.
- Only one process can execute at a time.
- OS must decide which process runs next.
- Improves CPU utilization and performance.

---

# Types of Scheduling

## 1. Preemptive Scheduling

- CPU can be taken away from a running process.
- More responsive.
- Used in modern operating systems.

Example:
- Round Robin
- Preemptive Priority
- Shortest Remaining Time First (SRTF)

---

## 2. Non-Preemptive Scheduling

- Once a process starts executing, it runs until completion.
- Simpler but less responsive.

Example:
- FCFS
- Non-preemptive SJF
- Non-preemptive Priority

---

# Scheduling Algorithms

---

## 1. FCFS (First Come First Serve)

### Rule:
Processes are executed in order of arrival.

### Characteristics:
- Non-preemptive
- Simple to implement
- May cause Convoy Effect

### Problem:
Short processes wait behind long processes.

---

## 2. SJF (Shortest Job First)

### Rule:
Process with smallest burst time executes first.

### Characteristics:
- Can be preemptive or non-preemptive
- Gives minimum average waiting time
- May cause starvation

### Preemptive version:
Shortest Remaining Time First (SRTF)

---

## 3. Round Robin (RR)

### Rule:
Each process gets a fixed time quantum.

### Characteristics:
- Preemptive
- Fair scheduling
- Used in real systems
- Performance depends on time quantum

### If time quantum is too small:
- Too many context switches

### If time quantum is too large:
- Behaves like FCFS

---

## 4. Priority Scheduling

### Rule:
Process with highest priority executes first.

### Characteristics:
- Can be preemptive or non-preemptive
- May cause starvation

### Solution to starvation:
Aging (gradually increasing priority of waiting processes)

---

# Important Scheduling Terms

## 1. Arrival Time (AT)
Time at which process enters ready queue.

## 2. Burst Time (BT)
Time required by process for execution.

## 3. Completion Time (CT)
Time at which process finishes execution.

## 4. Turnaround Time (TAT)

TAT = Completion Time - Arrival Time

Represents total time process spends in system.

## 5. Waiting Time (WT)

WT = Turnaround Time - Burst Time

Represents time spent waiting in ready queue.

## 6. Response Time (RT)

RT = First CPU allocation time - Arrival Time

---

# Performance Criteria

A good scheduling algorithm should:

- Maximize CPU utilization
- Minimize waiting time
- Minimize turnaround time
- Minimize response time
- Avoid starvation

---

# Comparison of Algorithms

| Algorithm | Preemptive | Starvation | Used in Real OS |
|------------|------------|------------|-----------------|
| FCFS | No | No | Rare |
| SJF | Both | Yes | Rare |
| Round Robin | Yes | No | Yes |
| Priority | Both | Yes | Yes |

---

