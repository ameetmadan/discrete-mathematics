# Proportional Logic

- The field of Natural Language Processing (NLP) is advancing at a high speed, with devices such as Amazon Alexa, Google Home etc. using the underlying technology to turn spoken language into commands. This technology is based on proportional logic, because it tries to immitate the human language -> the same sentence can be said in multiple ways, but always keeping the same meaning. 

- A statement is either **true** or **false**, it can not be both. 

## Compound statements (connectives)

| Name | Term        | Symbol         |
| ---- | ----------- | -------------- |
| NOT  | Negation    | $$ \sim  $$    |
| AND  | Conjunction | $$  \wedge  $$ |
| OR   | Disjunction | $$  \lor  $$   |

- Variables in proportional logic can only have two values, either true or false. This is why they are called boolean variables.
- Negation (~) has presedence over ∧ or ∨.

| Name                                      | Term            |
| ----------------------------------------- | --------------- |
| "It is hot"                               | $$ p $$         |
| "It is sunny"                             | $$ q $$         |
| "It is not hot but it is sunny"           | $$ \sim p∧q $$  |
| "It is neither hot nor sunny"             | $$ \sim(p∧q) $$ |
| "It is not true that it is hot and sunny" | $$ \neg(p∧q) $$ |


### Truth tables

#### Negation
| $$ p $$ | $$ \sim p $$ |
| ------- | ------------ |
| T       | F            |
| F       | T            |

#### Conjunction
| $$ p $$ | $$  q $$ | $$ (p \land q) $$ |
| ------- | -------- | ----------------- |
| T       | T        | T                 |
| T       | F        | F                 |
| F       | T        | F                 |
| F       | F        | F                 |

#### Disjunction
| $$ p $$ | $$ q $$ | $$ (p \lor q)  $$ |
| ------- | ------- | ----------------- |
| T       | T       | T                 |
| T       | F       | T                 |
| F       | T       | T                 |
| F       | F       | F                 |

#### Exclusive or (XOR)
$$ p \oplus q \equiv (p \lor q ) \land \sim(p \land q) $$ 
| $$ p $$ | $$ q $$ | $$ p \lor q $$ | $$ p \land q $$ | $$ \sim(p \land q) $$ | $$ p \oplus q $$ |
| ------- | ------- | -------------- | --------------- | --------------------- | ---------------- |
| T       | T       | T              | T               | F                     | F                |
| T       | F       | T              | F               | T                     | T                |
| F       | T       | T              | F               | T                     | T                |
| F       | F       | F              | F               | T                     | F                |

#### Three input statements

| $$ p $$ | $$ q $$ | $$ r $$ | $$ s $$ | $$ t $$ | $$ f $$ |
| ------- | ------- | ------- | ------- | ------- | ------- |
|         |         |         |         |         |         |