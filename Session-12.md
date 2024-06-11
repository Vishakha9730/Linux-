# Process Management in Linux-
# What is Process?
- Process is any program in its excecution.
- It generally takes an input, processes it and gives us the appropriate output.
- An active program which running now on the Operating System is known as the process.
# Why Process Management is required-
##### 1)Resource Allocation-
##### 2)Concurrency-
##### 3)Isolation-
##### 4)Process Prioritization-
##### 5)Process Lifecycle-

# Types of Processes:

## Foreground Processes: 
- they run on the screen and need input from the user.
- also referred to as interactive processes

## Background Processes: 
- they run in the background and usually do not need user input.
- referred to as non-interactive or automatic processes
- for example: Antivirus.
## Commands-
#### &-
- Starts the command immediately in the background.
#### Ctrl+Z-
- Stops the job temporarily so that it can be managed.
#### Ctrl+C- 
- Can be used to cancel the current interactive job
#### bg- 
- Continues the job that has just been frozen using Ctrl+Z in the background.
#### fg-
- Brings the last job that was moved to background execution back to the foreground.
#### jobs-
- Shows which jobs are currently running from current shell. 
- Displays job numbers that can be used as an argument to the command bg and fg.
## Daemon Process-
- is a type of background process that runs continuously, typically providing system services or performing tasks without direct user interaction even if terminating terminal.
- example- init, crond
# Parent Process and Child Process-
- The parent process is the process that creates another process.
- A child process is a process that is created by another process, known as its parent process.
### PID-
- Every process in the system is assigned a unique numeric identifier called a Process ID (PID).
- PIDs are used by the operating system to manage and identify processes.
- echo $$
- pidof [process name]
### PPID-
- The Parent Process ID (PPID) indicates the PID of the parent process that created the current process.
- echo $PPID
  

# Process Management Lifecycle-
#### Following are the States of Process Management Lifecycle-

### New/Create:
- The process has been created but has not yet been scheduled for execution.
- During creation, the operating system allocates resources to the process, such as memory space, CPU time, and other necessary resources.
- The operating system assigns a unique identifier to the process known as the Process ID (PID), which is used to manage and identify the process.
### Ready:
- The process is ready to be executed.
- In this state, the process is ready to execute but is waiting for the CPU to be allocated to it.
- The process may also be waiting for other events, such as I/O operations to complete or signals from other processes.
### Running: 
- The process is currently being executed.
- In the running state, the process's instructions are executed by the CPU, and it performs its intended tasks.
### Waiting:
- The process is waiting for an event to occur, such as the completion of an I/O operation.
### Terminated: 
- Eventually, the process completes its execution or is terminated.
- When a process terminates, it releases the resources it was using, including memory, files, and other system resources.
- The operating system removes the process from its process table and deallocates its resources, marking the end of its lifecycle.

  
 ![image](https://github.com/vishakhadhonde9/Linux-Second-half-/assets/97825776/1dd38ebe-44e8-43f6-af9d-cb0d962e9d39)

## Zombie Process-
- Process that has finished its task, but its parent process hasn't yet collected its exit status from the operating system.

