# knowledge on VLOOKUP

To change a text string in spreadsheet cell F8 to a numerical value, what is the correct function? 

=NUM(F8)
=CONVERT(F8)
=MATCH(F8)
=VALUE(F8)

> To change the text string in spreadsheet cell F8 to a numerical value, the correct syntax is =VALUE(F8). Within the parenthesis, the VALUE syntax must include a reference to the specific cell whose value the function should convert.

What is the purpose of an absolute reference within a function, such as "$C$3"?

To represent missing values in a formula or function
To remove unnecessary instructions from a formula or function
To lock rows and columns so they won't change when a function is copied
To make formulas and functions unconditional

> The purpose of an absolute reference is to lock the reference to a row or column so values won't change when a function is copied. 

In VLOOKUP, TRUE tells the function to search for exact matches, and FALSE tells the function to look for approximate matches.

True
False

> In VLOOKUP, TRUE tells the function to search for approximate matches, and FALSE tells the function to look for exact matches.

The following is a selection from a spreadsheet:


To search for the population of Nigeria, what is the correct VLOOKUP syntax?

=VLOOKUP(Nigeria, A2:C10, 3, false)   
=VLOOKUP(Nigeria, A2:C10, 3, true)    
=VLOOKUP("Nigeria", A2:C10, 2, false)   
=VLOOKUP(Nigeria, A2,C10, 2, true)    

> To search for the population of Nigeria, the syntax is =VLOOKUP("Nigeria", A2:C10, 2, false). “Nigeria” is the reference. A2:C10 is the table array. The 2 indicates the position of the column from which the value should be returned. And the word false instructs the function to return an exact match.

To search for the height of the building in Mecca, what is the correct VLOOKUP syntax?

=VLOOKUP(Mecca, A2:D7, 2, false)    
=VLOOKUP(Mecca, A2,D7, 3, true)   
=VLOOKUP("Mecca", A2:D7, 3, false)    
=VLOOKUP(Mecca, A2:D7, 2, true)   

> To search for the height of the building in Mecca, the correct syntax is =VLOOKUP("Mecca", A2:D7, 3, false). “Mecca” is the reference. A2:D7 is the table array. The 3 indicates the number of the column from which the value should be returned. And the word false instructs the function to return an exact match.


