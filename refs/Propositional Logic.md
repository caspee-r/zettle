# Propositional Logic
#### status: 
#### created: 2022-07-31
---
### what is a proposition
proposition is a *declarative* sentence that can be assigned a **truth value** either true or false.
### Premises
*Premises* are propositions that's support and proves a conclusion *logically*
### Conclusion
it's a proposition that's logically follows from a premise
### what is not a proposition 
1. Orders
2. Questions
3. sentence with variables ..ex(x is an integer)
4. self-referential sentences

###  how we reasoning using propositions
we build our propositions on top of atomic proposition using **propositional connectives**.
using **truth table** we can propagate all the truth value within our propositional connectives.

### atomic propositions
those are the simplest build block in the propositional logic we can connect different atomic proposition with propositional connectives and we call the new *connected* sentence a **compound proposition**

### examples of atomic propositions
- The Shape of the Earth is a flat shape
- 100 > 39
- the ocean bigger than the river
- My weight is more than 100 lbs

### propositional connectives
#### Unary :
-  not, called negation, denoted **¬**;
#### Binary
-  and, called conjunction, denoted **∧** (or sometimes &);
-  or, called disjunction, denoted **∨**;
-  if . . . then . . . , called implication, or conditional, denoted **→**;
-  . . . if and only if . . . , called biconditional, denoted **↔**.

==**all connectives** take a truth value and *output* a truth value

### compound propositions
a result of *connecting* atomic propositions with propositional connectives
### truth tables
tell us all the possible outcomes(truth values) of *statements* and *connectives* using *propositional arithmetic* . we denote **true** as **T** and **false** as **F** as a convenient 
#### propositional arithmetic
• The proposition ¬A is true if and only if
the proposition A is false.
• The proposition A ∧ B is true if and only if
both A and B are true.
• The proposition A ∨ B is true if and only if
either of A or B (possibly both) is true.
• The proposition A → B is true if and only if
A is false or B is true, that is, if the truth of A implies the truth of B.
• The proposition A ↔ B is true if and only if
A and B have the same truth values

#### negation 
|   P   |   ¬P   |
|:-----:|:-----:|
| **T** | **F** |
| **F** | **T** |
#### conjunction
|   p   |   q   | p ∧ q |
|:-----:|:-----:|:-----:|
| **T** | **T** | **T** |
| **F** | **T** | **F** |
| **T** | **F** | **F** |
| **F** | **F** | **F** |
#### disjunction
| p     | q     | p ∨ q |
| :-----: | :-----: | :-----: |
| **T** | **T** | **T**      |
| **F** | **T** |    **T**   |
| **T** | **F** |   **T**    |
| **F** | **F** |  **F**     |

#### conditional 
| p     | q     | p→q |
| :-----: | :-----: | :-----: |
| **T** | **T** | **T**      | 
| **F** | **T** |    **T**   |
| **T** | **F** |   **F**    |
| **F** | **F** |  **T**     |
#### biconditional
| p     | q     | p↔q |
| :-----: | :-----: | :-----: |
| **T** | **T** | **T**      |
| **F** | **T** |    **F**   |
| **T** | **F** |   **F**    |
| **F** | **F** |  **T**     |

### The meaning of the connectives in natural language and in logic


### it's limits
the use of proposition logic very limiting in the reasoning process which we express it in terms of propositions and their truth values

---
### references
- [[@gorankoLogicToolGuide2016]]