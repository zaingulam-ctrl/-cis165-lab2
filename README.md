# CIS 165 Lab 2

**Course section:** CIS-165-W099)

## Initial plans 

**sum.cpp:** I need two integers, 50 and 100. I'll add them and store the answer
in a variable called total. Then I'll print total with a label.

**mpg.cpp:** I need the gallons (16) and the miles (312). I'll divide miles by
gallons and store that in a variable, then print it with a label and "MPG".
I need a data type that can hold decimals.



## Test table

| Program | Values used | Expected result before running | Actual output | Match or fix |
|---|---|---|---|---|
| sum.cpp, assigned | 50 and 100 | 50 + 100 = 150 | The total of 50 and 100 is: 150 | Match |
| sum.cpp, changed | 20 and 35 | 20 + 35 = 55 | The total of 20 and 35 is: 55 | Match |
| mpg.cpp, assigned | 312 miles; 16 gallons | 312 / 16 = 19.5 | Miles per gallon: 19.5 MPG | Match |
| mpg.cpp, changed | 250 miles; 8 gallons | 250 / 8 = 31.25 | Miles per gallon: 31.25 MPG | Match |


After testing, I changed both files back to the original assigned values
(50 and 100; 312 miles and 16 gallons) and reran both programs. They gave the
correct results again. 

## Code explanations

**sum.cpp:**
I first made the numbers 50 and 100 start out in the variables first_number and
second_number. The line int total = first_number + second_number; adds them
and stores the answer in total. Then cout prints the value of total with a
label. I stored the calculation in total first because it keeps the math
separate from the printing. It also makes the result easy to check.

**mpg.cpp:** 
The formula is miles divided by gallons. I used double for miles,
gallons, and miles_per_gallon so the answer can keep its decimal part. If it
divides two integers, it gets rid of the fractional part, so 312 / 16 is
exactly 19.5 but integer division on something like 250 / 8 would give 31
instead of 31.25. Using doubles avoids that. For my changed value test, I set
miles to 250 and gallons to 8. The program calculated 250.0 / 8.0 = 31.25,
stored it in miles_per_gallon, and printed "Miles per gallon: 31.25 MPG".
