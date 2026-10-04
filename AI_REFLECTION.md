# AI Reflection

**Tools used:** I used ChatGPT to help me check my plan and to explain why
integer division drops decimals.

**One decision:** I asked, "Why does dividing two ints in C++ give a whole
number, and what type should I use for miles per gallon?" It suggested using
double for all three variables. I accepted that because the lab says to keep
the fractional result. 

**Verification:** I compiled both programs and got no warnings. I also calculated the answers by hand before running them
(150 and 19.5, plus my changed values 55 and 31.25), and the outputs matched.
That shows the formulas and data types work, which is a better check than just
trusting that the code looks right.

**Learning:** I can now explain why integer division loses the decimal part and
how storing a result in a variable before cout keeps the code organized. I
still need to practice learning how to understand when to use each data type
