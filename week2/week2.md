# Digital logic circuits

## Simple circuit

![](../images/bff024c6650d54c991df9145005328fdfd8f4f1a74c9ccb044c4b80413532f42.png){ width=350px }

A simple circuit has three elements: switch, battery and load

![](../images/a9cbd322849ec9f2a0720639e4eece46abf50f41f66c3722692300e376a629ba.png){ width=350px }

Switches can either be used "in series" (the circuit will only work when both switches are closed) or "in parallel" (the circuit will work when one of the both switches are closed). 

The in series circuit is equivalent to the AND truth table, where closed is equivalent to true and the truth table is only true when both values are true (closed).

The in parallel circuit is equivalent to the OR truth table, where closed is equivalent to true and the truth table is only false when both values are false (open). 

\newpage

## Combinatorial circuit

- cominatorial: type of digital circuit whose output only depends on the current input.
- sequential: output depends on both the current input and previous outputs. This means a sequential circuit
preserves a memory of the input while a combinational circuit does not (out of scope for this course)

![](../images/76ad9f8e868083c0086ef963a970b70797b0ad33b96cb3c8877a51a550801c58.png){ width=350px }

Rules for cominatorial circuits

1. Never combine the input wires.
2. Never feed back the output of a gate into the same gate

- combinatorial equivalence: two circuits can have the same output but built completely differently
- circuit minimization: for production of electrical circuit it makes sense minimizing more complicated circuits to simplified ones so that they cost lesser in production.

## Logic gates

![](../images/1cf1039d79cb09cc8e880834f5ae93dca4fa27b6a260ec0b048e89a924b8600c.png){ width=450px }

## Disjunctive Normal Form (DNF)

Also called "Or of And's" $$ G(p,q) \equiv (p \land q) \lor (\neg p \land q) $$

- Best when output is 0
- AND together all variables where output is 1
- OR togetjer all the 1 rows
- Simplify

## Conjunctive Normal Form (CNF)

Also called "And of Or's" $$ G(p,q) \equiv (p \lor q) \land (\neg p \lor q) $$

- Best when output is mostly 1
- Indentify rows with output 0
- OR together all variables in some row (negeate when 1)
- AND together the 0 rows

\newpage

## Multiplexer

This Multiplexer selects the output of the AND operation if the selector S=0, otherwise it selects the output of the OR operation.

![](../images/f9e34d3d43f4ce2b757462f39153856655d943327546ecd8849bc7e9b0ae1c55.png){ width=350px }

## Binary to decimal

For the binary number, read the numbers from bottom to top.

![](../images/0c2f1ebd157e2c2a658a42fa650b523a14a0c7dd019dfaece94b33fe69d430b0.png){ width=350px }

\newpage

## Decimal to binary

Multiply each digit with it's binary equivalent.

![](../images/a553e644a36eb69577055bcf434b4b7d4bf2191bbd3882e19d808cb9aa9f6389.png){ width=350px }

## Half-Adder

![](../images/757ddc03aa8d36ffde6e7d8d2c0a86be454b97944b58e17426d98b37e7cd5038.png){ width=250px }
![](../images/d1bbd60fa94e74035ca43aebad28bc1ae1a9d9783881ed09a4009514b4c12ef2.png){ width=250px }
![](../images/4dc9eff915a5b14dac5ae43b12c432981c5276b2b3aa4a93492d2a3e79ab6768.png){ width=250px } 

## Full-Adder

![](../images/322b8fadf6e0e508916d04a89b0b098607ebf139765f0cb5e26a109a7f60d919.png)
![](../images/c71f1cfad90a28c2efb8a0439665834386dc0813d1ff326191ce24a66c63612a.png)

![](../images/bb39ac333503e6ed0737df20d28993fd1da2660e544a4bf73352bf86b6565617.png)