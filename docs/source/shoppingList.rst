=========================
Shopping list information
==========================

This page is aimed at future developers of the applicatioj


Design alterations
--------------------------
- Item list: The list requires a method to remove items without “purchasing” them such as accidental additions to the list.
- The quantity has been moved under the item name to make it more readable.
- Most buttons are icon buttons to improve navigation.

Adding a spent cost
-----------------------
All costs are checked with the addShoppingItem method.
There is one parameter called cost. 
Theres a check for an empty valid which will lead to an automatic fail. Then it checks that
the cost is a valid double within the allowed range. Then the number of decimal points are checked

Item creation
-----------------
Items are checked and created using the addShoppingItem method. 
There is two parameters the collected quantity and name of the item, firstly theres a check for a quantity given,
if there is no input the item quantity is set to 0. 
Then theres a check to ensure that the quantity is an integer value if not the check fails.
Finally it checks the item name is within the character set.
