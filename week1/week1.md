# Proportional Logic

- The field of Natural Language Processing (NLP) is advancing at a high speed, with devices such as Amazon Alexa, Google Home etc. using the underlying technology to turn spoken language into commands. This technology is based on proportional logic, because it tries to immitate the human language -> the same sentence can be said in multiple ways, but always keeping the same meaning. 

- A statement is either **true** or **false**, it can not be both. 

## Compound statements (connectives)

| Name  |    Term     |     Symbol     |
| :---: | :---------: | :------------: |
|  NOT  |  Negation   |  $$ \sim  $$   |
|  AND  | Conjunction | $$  \wedge  $$ |
|  OR   | Disjunction |  $$  \lor  $$  |

- Variables in proportional logic can only have two values, either true or false. This is why they are called boolean variables.
- Negation has presedence over conjunction and disjunction.
 
| Name                                      |      Term       |
| ----------------------------------------- | :-------------: |
| "It is hot"                               |     $$ p $$     |
| "It is sunny"                             |     $$ q $$     |
| "It is not hot but it is sunny"           | $$ \sim p∧q $$  |
| "It is neither hot nor sunny"             | $$ \sim(p∧q) $$ |
| "It is not true that it is hot and sunny" | $$ \neg(p∧q) $$ |

\newpage

### Truth tables

#### Negation

| $$ p $$ | $$ \sim p $$ |
| :-----: | :----------: |
|    T    |      F       |
|    F    |      T       |


#### Conjunction

| $$ p $$ | $$  q $$ | $$ (p \land q) $$ |
| :-----: | :------: | :---------------: |
|    T    |    T     |         T         |
|    T    |    F     |         F         |
|    F    |    T     |         F         |
|    F    |    F     |         F         |

#### Disjunction

| $$ p $$ | $$ q $$ | $$ (p \lor q)  $$ |
| :-----: | :-----: | :---------------: |
|    T    |    T    |         T         |
|    T    |    F    |         T         |
|    F    |    T    |         T         |
|    F    |    F    |         F         |

#### Exclusive or (XOR)

$$ p \oplus q \equiv (p \lor q ) \land \sim(p \land q) $$ 

| $$ p $$ | $$ q $$ | $$ p \lor q $$ | $$ p \land q $$ | $$ \sim(p \land q) $$ | $$ p \oplus q $$ |
| :-----: | :-----: | :------------: | :-------------: | :-------------------: | :--------------: |
|    T    |    T    |       T        |        T        |           F           |        F         |
|    T    |    F    |       T        |        F        |           T           |        T         |
|    F    |    T    |       T        |        F        |           T           |        T         |
|    F    |    F    |       F        |        F        |           T           |        F         |

\newpage

#### Three input statements

With three statements, it makes sense to evaluate the each of the statements individually and then put the stements together.

| $$ p $$ | $$ q $$ | $$ r $$ | $$ p \land q $$ | $$ \sim r $$ | $$ (p \land q) \lor \sim r $$ |
| :-----: | :-----: | :-----: | :-------------: | :----------: | :---------------------------: |
|    T    |    T    |    T    |        T        |      F       |               T               |
|    T    |    T    |    F    |        T        |      T       |               T               |
|    T    |    F    |    T    |        F        |      F       |               F               |
|    T    |    F    |    F    |        F        |      T       |               T               |
|    F    |    T    |    T    |        F        |      F       |               F               |
|    F    |    T    |    F    |        F        |      T       |               T               |
|    F    |    F    |    T    |        F        |      F       |               F               |
|    F    |    F    |    F    |        F        |      T       |               T               |

#### De Morgan's law

When the negation sign is applied to a parantheses, the expressions "and" as well as "or" are interchanged.

$$ \sim(p \lor q) \equiv \sim p \land  \sim q  $$ 
$$ \sim(p \land q) \equiv \sim p \lor  \sim q  $$ 

#### Tautology and contradiction

A tautology (denoted by the symbol t) is a statement that is always true regardless
of the truth values of its component statements
$$ p \land t \equiv \bf t $$

A contradiction (denote by the symbol c) is a statement that is always false
regardless of the truth values of its component statements
$$ p \land c \equiv  \bf c $$

\newpage

## Basic logical equivalences

|         Name         |                             Laws                              |
| :------------------: | :-----------------------------------------------------------: |
|     Commutative      |               $$ p \land q \equiv q \land p $$                |
|     Associative      |     $$ (p \land q) \land r \equiv p \land (q \land r) $$      |
|     Distributive     | $$ p \land (q \lor r) \equiv (p \land q) \lor (p \land r)  $$ |
|       Identity       |                   $$ p \land t \equiv p $$                    |
|       Negation       |               $$  p \lor \sim p \equiv \bf t $$               |
|   Double negative    |                 $$ \sim (\sim p) \equiv p $$                  |
|      Idempotent      |                   $$ p \land p \equiv p $$                    |
|   Universal bound    |               $$ p \lor \bf t \equiv \bf t  $$                |
|     De Morgan's      |       $$ \sim (p \land q) \equiv \sim p \lor \sim q $$        |
|      Absorption      |               $$ p \lor (p \land q) \equiv p $$               |
| Negations of t and c |                   $$ \sim \bf t \equiv c $$                   |


|         Name         |                             Laws                             |
| :------------------: | :----------------------------------------------------------: |
|     Commutative      |                $$ p \lor q \equiv q \lor p $$                |
|     Associative      |       $$ (p \lor q) \lor r \equiv p \lor (q \lor r) $$       |
|     Distributive     | $$  p \lor (q \land r) \equiv (p \lor q) \land (p \lor r) $$ |
|       Identity       |                   $$ p \lor c \equiv p $$                    |
|       Negation       |              $$ p \land \sim p \equiv \bf c $$               |
|   Double negative    |                            N. A.                             |
|      Idempotent      |                   $$ p \land p \equiv p $$                   |
|   Universal bound    |               $$ p \land \bf c \equiv \bf c $$               |
|     De Morgan's      |       $$ \sim (p \lor q) \equiv \sim p \land \sim q $$       |
|      Absorption      |              $$ p \land (p \lor q) \equiv p $$               |
| Negations of t and c |                  $$ \sim \bf c \equiv t $$                   |

\newpage

## Condtional statements

If-then conditional statements, if is the hypothesis and q is the conclusion 

| $$ p $$ | $$ q $$ | $$ p \rightarrow q  $$ | $$ \sim p \lor q $$ |
| :-----: | :-----: | :--------------------: | :-----------------: |
|    T    |    T    |           T            |          T          |
|    T    |    F    |           F            |          F          |
|    F    |    T    |           T            |          F          |
|    F    |    F    |           T            |          T          |


If-and only if means p implies q and q implies p. 

$$ (p \rightarrow q ) \land (q \rightarrow p ) $$

| $$ p $$ | $$ q $$ | $$ p \leftrightarrow q  $$ |
| :-----: | :-----: | :------------------------: |
|    T    |    T    |             T              |
|    T    |    F    |             F              |
|    F    |    T    |             F              |
|    F    |    F    |             T              |