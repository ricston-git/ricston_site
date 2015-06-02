## About multithreading

Multi-threading is how work performed by a computer can be divided into multiple concurrent streams of execution (generally referred to as threads).

Multi-threading is a common model to implement SM in multi-cored machines, where threads share memory through shared variables. In this model in parallel programming a processor can create multiple threads that will be executed in parallel. Each thread has its own stack, variables and ID, considered private state. For every thread there is a unique heap shared by all, then considered shared memory.

In order to allow a volume of work to be most effectively and safely divided into multiple concurrent streams of execution, a number of critical areas need to be addressed.

*   **Scheduling**: ensure worker tasks are able to progress independently and effectively (e.g. deadlock/livelock avoidance)
*   **Publication**: ensure data altered in one thread is only visible to others as expected
*   **Synchronization**: ensure critical regions are protected from multiple concurrent updates causing data loss/corruption.

The underlying tenet of concurrent processing is Amdahl's law ([graph](http://upload.wikimedia.org/wikipedia/commons/e/ea/AmdahlsLaw.svg)). This law governs the diminishing amount of throughput that can be achieved by greater numbers of concurrent processors/cores. Therefore the overall aim of multi-threading is to minimize the amount of serial execution (exclusive locking) within any concurrent system.

# Frequently Asked Questions

*   [What's the difference between the atomic and nonatomic attributes?](http://stackoverflow.com/questions/588866/atomic-vs-nonatomic-properties)
*   [What's the difference between Invoke() and BeginInvoke()](http://stackoverflow.com/questions/229554/whats-the-difference-between-invoke-and-begininvoke)
*   ["implements Runnable" vs. "extends Thread"](http://stackoverflow.com/questions/541487/java-implements-runnable-vs-extends-thread)
*   [Difference between wait() and sleep()](http://stackoverflow.com/questions/1036754/difference-between-wait-and-sleep)
*   [What are the differences between various threading synchronization options in C#?](http://stackoverflow.com/questions/301160/what-are-the-differences-between-various-threading-synchronization-options-in-c)
*   [What is the difference between a process and a thread](http://stackoverflow.com/questions/200469/what-is-the-difference-between-a-process-and-a-thread)
*   [What is meant by "thread-safe" code?](http://stackoverflow.com/questions/261683/what-is-meant-by-thread-safe-code)
*   [What is a race condition?](http://stackoverflow.com/questions/34510/what-is-a-race-condition)
*   [What are the "things to know" when diving into multi-threaded programming in C++](http://stackoverflow.com/questions/2118090/what-are-the-things-to-know-when-diving-into-multi-threaded-programming-in-c)
*   [How should I unit test threaded code?](http://stackoverflow.com/questions/12159/how-should-i-unit-test-threaded-code) [What is Daemon thread in java](http://stackoverflow.com/questions/2213340/what-is-daemon-thread-in-java)

# Books

*   ["Threading in C#"](http://www.albahari.com/threading/) (free e-book)
*   ["Java Concurrency in Practice"](http://www.javaconcurrencyinpractice.com/)
*   ["C++ Concurrency in Action"](http://www.manning.com/williams/)
*   ["Principles of Concurrent and Distributed Programming"](http://rads.stackoverflow.com/amzn/click/032131283X)
*   ["Concurrent Programming on Windows"](http://rads.stackoverflow.com/amzn/click/032143482X)
*   [Java Threads, By Scott Oaks, Henry Wong](http://shop.oreilly.com/product/9780596007829.do)

# More information:

*   [Multithreading (computer architecture)](http://en.wikipedia.org/wiki/Multithreading_%28computer_architecture%29) (Wikipedia)
*   [Multithreading (software)](http://en.wikipedia.org/wiki/Multithreading_%28software%29#Multithreading) (Wikipedia)