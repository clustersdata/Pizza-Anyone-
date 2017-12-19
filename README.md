# Pizza-Anyone-

Pizza Anyone?

Description

You are responsible for ordering a large pizza for you and your friends. Each of them has told you what he wants on a pizza and what he does not; of course they all understand that since there is only going to be one pizza, no one is likely to have all their requirements satisfied. Can you order a pizza that will satisfy at least one request from all your friends? 

The pizza parlor you are calling offers the following pizza toppings; you can include or omit any of them in a pizza: 

Input Code     Topping 

A              Anchovies 

B              Black Olives 

C              Canadian Bacon 

D              Diced Garlic 

E              Extra Cheese 

F              Fresh Broccoli 

G              Green Peppers 

H              Ham 

I              Italian Sausage 

J              Jalapeno Peppers 

K              Kielbasa 

L              Lean Ground Beef 

M              Mushrooms 

N              Nonfat Feta Cheese 

O              Onions 

P              Pepperoni 

Your friends provide you with a line of text that describes their pizza preferences. For example, the line 

+O-H+P; 

reveals that someone will accept a pizza with onion, or without ham, or with pepperoni, and the line 

-E-I-D+A+J; 

indicates that someone else will accept a pizza that omits extra cheese, or Italian sausage, or diced garlic, or that includes anchovies or jalapenos. 

Input

The input consists of a series of pizza constraints. 
A pizza constraint is a list of 1 to 12 topping constraint lists each on a line by itself followed by a period on a line by itself. 
A topping constraint list is a series of topping requests terminated by a single semicolon. 
An topping request is a sign character (+/-) and then an uppercase letter from A to P.

Output

For each pizza constraint, provide a description of a pizza that satisfies it. A description is the string "Toppings: " in columns 1 through 10 and then a series of letters, in alphabetical order, listing the toppings on the pizza. So, a pizza with onion, anchovies, fresh broccoli and Canadian bacon would be described by: 

Toppings: ACFO 

If no combination toppings can be found which satisfies at least one request of every person, your program should print the string 
"No pizza can satisfy these requests." on a line by itself starting in column 1.

Sample Input

+A+B+C+D-E-F-G-H;
-A-B+C+D-E-F+G+H;
-A+B-C+D-E+F-G+H;
.
+A+B+C+D;
+E+F+F+H;
+A+B-G;
+O+J-F;
+H+I+C;
+P;
+O+M+L;
+M-L+P;
.
+A+B+C+D;
+E+F+F+H;
+A+B-G;
+P-O;
+O+J-F;
+H+I+C;
+P;
+O;
+O+M+L;
-O-P;
+M-L+P;
.

Sample Output

Toppings: 
Toppings: CELP 
No pizza can satisfy these requests. 
