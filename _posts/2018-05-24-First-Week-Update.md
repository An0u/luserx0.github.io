---
layout: post
title:  "First week progress"
date:   2018-05-24 
---

# First Week's Progress  
Hey everyone!! Now that I have completed my first week in the pit I would like
to share my experience.  
### I never thought  
I would have to deal with so many deployment issues.   
Learning to write NetBSD KLMs is much easier than dealing with the NetBSD
deployment issues of building HEAD of source systems with debugging options.  
Spending 2 days writing the kernel modul is ok, but adding 2 more to debug the
kernel is hella time-consuming.  

# The first evaluation goals:
*1. Finish and submit an example kernel module (panic_string)
*2. Add support for KUBSAN build option of the kernel.

    There will pop up build issues as -fsanitize=undefined enforces stricter
    warnings. Please keep reporting them to the developers and we will
    address them.

    There are extra points to keep reporting them with patches.
*3. Add a stub kubsan kernel module, that implements required functions 
    as dummy ones. Get this kernel to build

*4. Get the kernel with kubsan to boot and run.

    There will be likely a need to disable -fsanitize=undefined for a part
    of bootloader code. Please follow the linux case, and determine where we
    need to disable it.

### For each goal about 10 days are provided.

## Current Progress & Solutions  

I'm still working on the panic_string module. It's almost complete, it's being
tested against the kernel currently. It has passed many revisions and features
of safety have been added. Many standarb lib C functions weren't available and
had to be rewritten.

*Still not finished*

The biggest lesson I've learnt so far is to ask help. Actually, is identifying
when I am stuck. Not being in the mood of reproducing last year's mistakes, I
decided to hire cloud resources to deal with the deploying and testing of
NetBSD. This way I will have good to solutions to hard problems.

* I've been reading thoroughly through the books:
    1) Expert C Programming by Linden
    2) FreeBSD Device Drivers from No Starch
    3) The UNIX Programming Environment by Kernighan & Pike

## This week's goals
1) Finish the module kernel debugging
2) Set up Testing & DEployment envs
3) Finish the aforementioned books
4) Start some reading on OS theory
5) FINALLY, create the new personal website

* Extra: Report weekly to both mentors - every Monday  

Regards from this side of development,  
Hope next time I have more to report :)  
Harry
