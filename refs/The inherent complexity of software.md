# The inherent complexity of software
#### status: 
#### created: 2022-08-03
---
“Einstein argued that there must be simplified explanations of nature, because God is not capricious or arbitrary. No such faith comforts the software engineer. Much of the complexity that he must master is arbitrary complexity” -- p 32

## Defining software complexity
in the world of software we often see software with no complexity. these software more likely constructed and maintained by one person works in *isolation* , such systems tend to have limited functionality and and short life span .
the difference between those tedious software and the *industrial-strength*  software is that the last is intensely hard to understand all the subtleties of its design. **complexity is essential for large software, we may master it but we can never make it go away**

## why software inherently complex
### the complexity of the problem domain

the design of an industrial-strength software require a complex implementation of it's functionality, on top of this complexity there is other *implicit requirements* such as **performance**, **usability**,**scalability**, which adds another *external complexity*, the cause of it is the *communication gap* between the user and the developer because of the different perspective of each one on the nature of the problem , the user may have a vague idea about what he want's , moreover, the requirements of a software system change during it's development which .
large software system is a capital investment so we cant scrap it each time the requirements change , we need to have a strong view about our design, document and prototyping help us in this point also asking the user questions that eliminate the dark corners in the design.
*maintenance* is the correction of errors while *evolution* is when we respond to changing requirement and *preservation* is when we keep an ancient peace of software in operation

### The Difficulty of Managing the Development Process
>" Just a few decades ago, assembly language programs of only a few thousand lines of code stressed the limits of our software engineering abilities. " p 35

we strive to write less code by reusing frameworks  or invent a mechanism that give us the *illusion of simplicity*.
nowadays, software systems enforce us to create new systems or reuse other existing software in a *novel way*
these system measured in hundreds of thousands even million lines of code and no one can understand them *completely*  so need a **team of developers** ideally a *small team of developers* because team development have problems with it that is when the team get bigger the communication problem evolve with it particularly when the team is geographically dispersed.

With a team of developers, the key management challenge is always to maintain a unity and integrity of design.  

### The Flexibility Possible through Software

software offers the *ultimate flexibility* cause it's possible for a developer to **express** any kind of **abstraction** 
this *flexibility* force us to build virtually all the primitives blocks for the higher abstraction to *stand* on.
As a result, software development remains a 
labor-intensive business.   

###  The Problems of Characterizing the Behavior of Discrete Systems

in a large application that have many variables and maybe many threads this application have a state that determined by the values of all the variables  and the current address and calling stack of each process within the system . we execute this application on computer, as a result we have a *discrete system* which are by there nature have finite number of states in a very large code base we have a very large number of **possible** states , So we design our systems with a *separation of concerns* so that the change in one *part* don't have a big effect on another part .
the *transition* between a state an another caused by an *external event* that in the worst circumstances can corrupt the state of a system because it's designer **failed** to take into account certain *interaction* among events
in discrete system external event can change the system *internal state* therefor, we have to test our systems 

# 

---
