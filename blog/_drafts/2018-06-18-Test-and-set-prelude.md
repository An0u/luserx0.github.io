---
layout: post
title:  "Test-and-set NetBSD HOWTO"
date:   2018-06-27
---

# Test-and-set  

https://en.wikipedia.org/wiki/Test-and-set
https://en.wikipedia.org/wiki/Linearizability
https://stackoverflow.com/questions/3659336/compare-and-swap-vs-test-and-set#
https://github.com/torvalds/linux/blob/5924bbecd0267d87c24110cbe2041b5075173a25/arch/x86/include/asm/bitops.h
https://github.com/torvalds/linux/blob/ead751507de86d90fa250431e9990a8b881f713c/include/linux/bitops.h


1)
test-and-set: 
modifies the contents of a memory location and returns its old value as a single atomic operation.

compare-and-swap:
atomically compares the contents of a memory location to a given value and, only if they are the same, 
modifies the contents of that memory location to a given new value.

2)
In concurrent programming, an operation (or set of operations) is atomic, linearizable, indivisible or uninterruptible 
if it appears to the rest of the system to occur at once without being interrupted. 
Atomicity is a guarantee of isolation from interrupts, signals, concurrent processes and threads. 
It is relevant for thread safety and reentrancy. Additionally, atomic operations commonly have a succeed-or-fail 
definition—they either successfully change the state of the system, or have no relevant effect.

3)
Linearizability is a strong correctness condition, which constrains what outputs are possible 
when an object is accessed by multiple processes concurrently. It is a safety property which ensures that 
operations do not complete in an unexpected or unpredictable manner. 
If a system is linearizable it allows a programmer to reason about the system.

4)
In computer science, a semaphore is a variable or abstract data type used to control access to a 
common resource by multiple processes in a concurrent system such as a multitasking operating system. 
Semaphore is simply a variable. This variable is used to solve critical section problems 
and to achieve process synchronization in the multi processing environment.

A trivial semaphore is a plain variable that is changed (for example, incremented or decremented, or toggled) 
depending on programmer-defined conditions.

5)
Maurice Herlihy (1991) proved that test-and-set has a finite consensus number 
and can solve the wait-free consensus problem for at-most two concurrent processes.[2] 
In contrast, compare-and-swap offers a more general solution to this problem.

The calling process obtains the lock if the old value was 0 otherwise while-loop spins waiting to acquire the lock. 
This is called a spinlock. "Test and Test-and-set" is another example.

6)
Consensus (computer science):
A fundamental problem in distributed computing and multi-agent systems is to achieve overall system reliability 
in the presence of a number of faulty processes. 
This often requires processes to agree on some data value that is needed during computation.

7)
Test and test-and-set
Test-and-set
Compare-and-swap

Three methods of implementation ^^

./tests/lib/libc/sync/all_sync_ops_linkable.c:	__sync_lock_test_and_set(&u8, 5);

