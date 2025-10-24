# SR_flipflop

**Theory**

An SR flip-flop (Set-Reset flip-flop) is a bistable sequential circuit that can store one bit of binary information. It has two inputs:

Set (S) – used to set the output to 1

Reset (R) – used to reset the output to 0

Construction
It can be built using NOR gates or NAND gates, with feedback connections creating a stable memory element.

It has two outputs: Q (the main output) and Q' (the complement of Q).

Working Principle
When S = 1 and R = 0, the flip-flop is set, and Q = 1.

When S = 0 and R = 1, the flip-flop is reset, and Q = 0.

When S = 0 and R = 0, the flip-flop maintains its previous state (memory hold).

When S = 1 and R = 1, it leads to an invalid or undefined state (both Q and Q' are the same), which is avoided in proper operation.

Truth Table
S	R	Q (next state)	Q' (complement)	Description
0	0	No change	No change	Hold state
0	1	0	1	Reset
1	0	1	0	Set
1	1	Invalid	Invalid	Invalid/Forbidden state
Operation Modes
Set (S = 1, R = 0): Q = 1, Q' = 0

Reset (S = 0, R = 1): Q = 0, Q' = 1

Hold (S = 0, R = 0): Previous state preserved

Invalid (S = 1, R = 1): Both outputs are the same (not used in normal operation)

Applications
Used in memory units, flip-flop-based registers, during data storage, and in control circuits.

Widely used for synchronization and temporary data storage in digital systems.

Important Notes
To avoid race conditions and invalid states, SR flip-flops are often used with clock signals or replaced with JK or D flip-flops in more advanced applications.

In actual implementations, active-LOW or active-HIGH inputs are used depending on the type of gates (NAND or NOR).
