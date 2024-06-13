# Commands used in Process Management-
## ps(process  status)-
 - used to list currently running processes.
 - provides information about these processes, such as their process ID (PID), terminal associated with the process, CPU and memory usage, and more.
 - provides a snapshot of the current processes on your system.
#### ps [options]
* e: This option displays information about every process on the system.
* f: This option generates a full listing, providing more details about the processes and their relationships.
* u: This option displays the owner of each process and additional information like CPU and memory usage.
* x: This option lists all processes regardless of whether they are associated with a terminal.
* aux: This option shows a detailed list of all processes running on the system, including those owned by other users.

## top-
- top command is used to show the Linux processes.
- it provides dynamic real-time view of running system.
- usually, this command shows the summary information of the system and the list of processes or threads which are currently managed by the Linux Kernel.
# Adjust Process Priority-
- When Linux processes are started, they are started with a specific priority.
- By default, all regular processes are equal and are started with the same priority, which is the priority number 0.
- In some cases, it is useful to change the default priority that was assigned to the process when it was started.
- You can do that using the nice and renice commands.
- - the niceness value ranges from -20(highest prioprity) to 19(lowewst priority).
* To check nice value:
  ##### ps -l PID

## renice command-
-  used to change the niceness value of an existing process.
-  to alter priority of running process, we use renice command.
#### Syntax:
* renice value PID

## kill command-
- used to terminate process manually.
- kill command sends a signal to a process that terminates the process.
#### Syntax-
 kill -[signal number] PID
- Three of these signals work for all processes :
- The signal SIGTERM (15) is used to ask a process to stop.
- The signal SIGKILL (9) is used to force a process to stop.
- The SIGHUP (1) signal is used to hang up a process.

