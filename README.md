# Implementation-of-First-and-Follow

Aim -

To implement First and Follow.

Algorithm –

For computing the first:

Step 1 – If X is a terminal then FIRST(X) = {X}
Example: F -&gt; (E) | id
We can write it as FIRST(F) -&gt; { ( , id }
Step 2 – If X is a non terminal like E -&gt; T then to get FIRST(E) substitute T with other productions until you get a terminal as the first symbol
Step 3 – If X -&gt; ε then add ε to FIRST(X).

For computing the follow:

Step 1 – Always check the right side of the productions for a non-terminal, whose FOLLOW set is being found. (never see the left side).
Step 2 – (a) If that non-terminal (S,A,B…) is followed by any terminal (a,b…,*,+,(,)…) , then add that “terminal” into FOLLOW set.
(b) If that non-terminal is followed by any other non-terminal then add “FIRST of other 
nonterminal” into FOLLOW set.
