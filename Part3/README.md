# Reasons for concurrency and parallelism


To complete this exercise you will have to use git. Create one or several commits that adds answers to the following questions and push it to your groups repository to complete the task.

When answering the questions, remember to use all the resources at your disposal. Asking the internet isn't a form of "cheating", it's a way of learning.

 ### What is concurrency? What is parallelism? What's the difference?
 > Concurrency means that multiple tasks runs in overlapping time periods, that is not at exactly the same time.
 Parallelism means that processes runs at exactly the same time, for example with multicore processor.

 ### Why have machines become increasingly multicore in the past decade?
 > Increasing the clock frequency would result in to much power consumption and thus machines have become increasingly multicore to make programs faster without increasing the clock frequency.

 ### What kinds of problems motivates the need for concurrent execution?
 (Or phrased differently: What problems do concurrency help in solving?)
 > If we want multiple applications running at the same time on one machine, or if we want multiple machines to connect to the same server/network at the same time.

 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > *Your answer here*

 ### What are the differences between processes, threads, green threads, and coroutines?
 > Proesses are instances of a program that runs in its own memory space, separte from other processes.
 Threads are created by processes, and runs in the same memory space as the process that created it.
 Green threads are threads that are scheduled by a runtime library or virtual machine instead of the OS.

 ### Which one of these do `pthread_create()` (C/POSIX), `threading.Thread()` (Python), `go` (Go) create?
 > `pthread_create()` -> Thread
 `threading.Thread()` -> Thread
 `go` ->

 ### How does pythons Global Interpreter Lock (GIL) influence the way a python Thread behaves?
 > It allows only one thread to execute at a time.

 ### With this in mind: What is the workaround for the GIL (Hint: it's another module)?
 > You can use multiprocesses and the multiprocessing module.

 ### What does `func GOMAXPROCS(n int) int` change?
 > "GOMAXPROCS sets the maximum number of CPUs that can be executing simultaneously"
