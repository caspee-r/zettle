# getting started with algorithms
#### status: 
#### created: 2022-06-29
---
# definition of an algorithm
- algorithms are a computational  relation that turns the input to output .
- there is no thing such the best algorithm ever , instead there is the best algorithm for a certain problem case.
- algorithm tend to be correct if for all the input instances we get the right output 
- if we control the **error** **rate** of a certain  algorithm it may be useful in some cases

# hard problems vs "we can do it" problems
There is a wide variety of problems that we can solve  with efficient algorithm thought, it's not always the case because there is also some problems  don't have any **efficient algorithm**  .
we call those problem ==NP-complete problem== .

# algorithms as  technologies
do we need algorithms in a world with insane fast computers and free memory?, well the answer here is yes
and the reason is that you have to see if your solution ends with the right output   
- in most time we can solve a particular problem with different ways(algorithms) 
- every *way* differ from the other  in term of efficiency and the approach
- hardware and software are the least significant part that effect the running time of an algorithm
- for instance for small input size  we consider insertion sort to be faster than the merge sort but when  n goes bigger the merge sort is the faster
- the right algorithm can have a huge impact on the system performance, same as fast  hardware
> hardware make use of algorithms in their design
- many technologies use algorithms to do their job properly 

# algorithms running time
the running time of an algorithm depends on :
1. the machine specification 
2. the input

###### the relation between t  and n
there is a relation between **the running time**  of an algorithm and the **input size**
so we can *describe* the running time as a function of n which is the input size
###### what is a running time exactly ? 
we discussed in previous reference note that an algorithm is a procedure of operations, therefor the running time is the number of primitive operations or *steps* **executed**
we generally assume a **constant** amount of time required to execute each line.
###### why we set the time of executing each line to a  **constant** amount of time ?
to be **machine-independent** as much as possible
###### what is the meaning of "machine independent"?
this mean that *the running time* not **specific** to a particular machine
> [!NOTE] 
>One line may take a different amount of time than another line, but we shall assume that each execution of the ith line takes time ci, where ci is a
constant. This viewpoint is in keeping with the RAM model, and it also reflects
how the pseudocode would be implemented on most actual computers. 
###### the running time of loops
as we know loops are operations that may get executed more than one time so its block will be executed as long as the loop keep looping so it's running time will be a sum of it's costs :
$\sum_{n=1} ^{n} a_i x^i$

> When a for or while loop exits in the usual way (i.e., due to the test in the loop header), the test is executed one time more than the loop body.

---
### references
[[@cormenIntroductionAlgorithms2009]]