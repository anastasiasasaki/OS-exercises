# Operating-System-Concepts-Projects
Dinosaur book projects to follow along Operating System Concepts 10th edition by Peter B. Galvin, Greg Gagne, A Silberschatz  
Language: C  
OS: Linux (Debian)   

## TODO: 

### 1. Processes & System Calls

Exercise 1: Fork + Exec Playground 
- [ ] Write a program that:
  - [ ] Uses fork()
  - [ ] Parent waits using wait()
  - [ ] Child calls exec() to run /bin/ls
- [ ] Modify it:
  - [ ] Create multiple children
  - [ ] Print PIDs
  - [ ] Make a zombie process temporarily and observe with ps

Exercise 2: Build a Tiny Shell
- [ ] Implement:
  - [ ] Command input loop
  - [ ] fork()
  - [ ] execvp()
  - [ ] Background processes (&)
  - [ ] Basic pipes (|)
- [ ] Understand:
  - [ ] Process control
  - [ ] File descriptors
  - [ ] Pipes
  - [ ] Parent/child synchronization

### 2. CPU Scheduling

Exercise 3: Write a Scheduler Simulator 
- [ ] Simulate:
  - [ ] FCFS
  - [ ] SJF
  - [ ] Round Robin
  - [ ] Priority Scheduling
- [ ] Input:
  - [ ] Burst times
  - [ ] Arrival times
- [ ] Output:
  - [ ] Waiting time
  - [ ] Turnaround time
  - [ ] Gantt chart
- [ ] Compare average waiting times and visualize fairness

### 3. Threads

Exercise 4: Multithreading with Race Conditions 
- [ ] Create multiple threads incrementing a shared counter
- [ ] Observe incorrect results
- [ ] Fix with:
  - [ ] Mutex
  - [ ] Semaphore
- [ ] Measure performance difference with and without locks

### 4. Synchronization

Exercise 5: Implement Classical Problems
- [ ] Implement:
  - [ ] Producer–Consumer (with bounded buffer)
  - [ ] Readers–Writers
  - [ ] Dining Philosophers
- [ ] Intentionally break them, cause deadlock, and fix
- [ ] Understand:
  - [ ] Deadlock
  - [ ] Starvation
  - [ ] Fairness
  - [ ] Mutual exclusion

### 5. Memory Management

Exercise 6: Paging Simulator
- [ ] Simulate page references
- [ ] Implement:
  - [ ] FIFO
  - [ ] LRU
  - [ ] Optimal
- [ ] Count page faults
- [ ] Generate random access patterns and compare algorithms

Exercise 7: Build a Simple Allocator
- [ ] Implement your own malloc:
  - [ ] Use a large static array
  - [ ] Track free blocks
  - [ ] Implement first fit and best fit

### 6. File Systems

Exercise 8: Build a Toy File System
- [ ] Options:
  1. Simulate one in memory
  2. Build one inside a single file
- [ ] Implement:
  - [ ] Directory structure
  - [ ] File creation
  - [ ] Read/write
  - [ ] Inodes (simplified)
- [ ] Understand:
  - [ ] Allocation
  - [ ] Metadata
  - [ ] Block management

## 7. Deadlocks

Exercise 9: Banker's Algorithm Simulator
- [ ] Implement:
  - [ ] Need matrix
  - [ ] Allocation matrix
  - [ ] Safety check
- [ ] Generate random resource requests and see when the system becomes unsafe

### 8. Work With the Real OS
- [ ] On Linux, try:
  - [ ] strace to see system calls
  - [ ] top and htop
  - [ ] vmstat
  - [ ] lsof
  - [ ] cat /proc/[pid]/status
- [ ] Observe memory usage and CPU scheduling with your programs

### Bigger Project Ideas (Capstone-Level)
- [ ] Build a Mini Kernel:
  - [ ] Start with a basic bootloader
  - [ ] Enter protected mode
  - [ ] Implement basic scheduler, memory manager, and simple file system
- [ ] Modify the Linux kernel or study and modify MINIX
