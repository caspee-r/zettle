# the RAM model
#### status: 
#### created: 2022-06-30
---
#### what is a ram model
	we think about the *RAM Model* as an abstraction of how 
	does computers works, it's a simple model which capture 
	the essential behavior of a computer and make it easier 
	to work with . 
	This model encapsulates the core functionality of 
    computers but does not mimic them completely

#### Benefits
we use the ram model to analyse *machine-independent algorithms*. 
the model gives us  an excellent understanding of how an algorithm will perform  without run it on a computer

> Algorithms can be understood and studied in a language-
and machine-independent manner. 
-*the algorithm  design manual*

#### Properties
- walk on the instructions and execute them one by one
- basic arithmetic and logical operation considered to be simple operations that takes constant time (adding,subtracting,multi,if,call)  
- loops and subroutines considered as complex operations that take more then one step (because sorting an array with n=10 differ from sorting array with n=10000)
- the data types are **integers and floating points**
- the absence of cashes, virtual memory and the memory hierarchy

#### The RAM model of computation
the *ram model of computation* measures the running time by multiply each step by its coast then  summing up  all of them 

---
### referances
- [[@cormenIntroductionAlgorithms2009]] p:24
- [[@deutschRAMModelComputation2018]]
- [[@skienaAlgorithmDesignManual2008]] p:44


