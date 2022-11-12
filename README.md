# Philosophers-42

## About project: 

In computer science, the dining philosophers problem is an example problem often used in concurrent algorithm design to illustrate synchronization issues and techniques for resolving them.

It was originally formulated in 1965 by Edsger Dijkstra as a student exam exercise, presented in terms of computers competing for access to tape drive peripherals. Soon after, Tony Hoare gave the problem its present formulation.

Silent philosophers sit around a round table, each philosopher has a bowl of spaghetti in front of them. Forks lie on the table between each pair of nearest philosophers.

Every philosopher can either eat, or sleep, or meditate. Eating is not limited by the amount of spaghetti left - an infinite supply is implied. However, the philosopher can only eat when he is holding two forks - taken from the right and from the left.

Each philosopher may take the nearest fork (if one is available) or put it down if he is already holding one. Picking up each fork and returning it to the table are separate actions that must be performed one after the other.

The question of the task is to develop a behavior model (parallel algorithm) in which none of the philosophers will starve, that is, he will forever alternate between eating and thinking.

The task is to implement a program that solves this problem using mutex or semaphore. 

Mutex and semaphore are both techniques designed to achieve mutual exclusion of shared resources. In other words, it is the biggest task of concurrent programming, a method for controlling (management) access to shared resources by multiple processes or threads.

Mutex - mutual exclusion technique based on an object owned by a process (thread). Semaphore - mutual exclusion technique in which a counting variable value indicating the number of processes (threads) that can access the current shared resource is placed.


## Index:
- [philo](https://github.com/Anastasiia-Ni/Philosophers-42/tree/master/philo) Philosophers with threads and mutexes
- [philo_bonus](https://github.com/Anastasiia-Ni/Philosophers-42/tree/master/philo_bonus) Philosophers with processes and semaphores


## Installation:
```
$ git clone git@github.com:Anastasiia-Ni/Philosophers-42.git
$ cd Philosophers-42
$ cd philo
$ make
```

## Usage:

- `./philo arg1 arg2 arg3 arg4 arg5`    

 - arg1 = number_of_philosophers (the number of philosophers and also the number of forks)
 - arg2 = time_to_die (time in milliseconds from the start of their last meal to death)
 - arg3 = time_to_eat (the time it takes for a philosopher to eat)
 - arg4 = time_to_sleep (the time a philosopher will spend sleeping)
 - arg5 (optional) = number_of_times_each_philosopher_must_eat (if all philosophers ate this amount meal simulation stops)
