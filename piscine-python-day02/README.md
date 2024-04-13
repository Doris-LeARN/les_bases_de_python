## Exercice 01
In order to maintain a registry of the 1000 laureates of the Women AI & Data Academy until 2027, the president asks you to write a function get_matricule that assigns each laureate a matricule in the form 23WIADAXXXX based on their position in the list, where XXXX represents the laureate's position in the list.

For example, for:
classmates = ["Stella",Eulalie","Nabilath","Boushirath","Arielle","Diane","Nicole","Kawsar","Maryse","Joy","Celsia","Nancy","Loïse","Alexia","Carmine","Elohim","Odette","Hermione"]
get_matricule("Stella") will return 23WIADA0001.
get_matricule("Joy") will return 23WIADA0010.
For Léa, a laureate in the second cohort at position 102:
get_matricule("Léa") will return 23WIADA0102.
And the last laureate, Sandrine, is at the 1000th position, so we will have:
get_matricule("Sandrine") will return 23WIADA1000.

## Exercice 02
Create a function show_transactions that takes a list as parameter and displays each of its elements for example show_transactions ([512,42.08,-12] displays :

You received 512 euros

You received 42.08 euros

You spent 12 euros

## Exercice 03
You have the transaction history in this format:

 transactions_history = { "transactions" : [
 
 {
 
 "value":-42,
 
 "category":"transport"
 
 },
 
 {
 
 "value":1234,
 
 "category":"salary"
 
 },
 
  {
 
 "value":-23,
 
 "category":"transport"
 
 },
 
  {
 
 "value":-24,
 
 "category":"transport"
 
 },
 
  {
 
 "value":465,
 
 "category":"salary"
 
 },
 
  {
 
 "value":-453,
 
 "category":"shopping"
 
 },
 
 ]
 
 }
 
You can clearly see that it's a dictionary in which the key represents the money inflow or outflow, and the value represents the category associated with that key.

Write a function add_transaction that takes as parameters the transaction history, the category, and the category value and adds this transaction to the transaction history.

For example add_transaction(transactions_history,"shopping",-200) will return:

transactions_history = { "transactions" : [
 
 {
 
 "value":-42,
 
 "category":"transport"
 
 },
 
 {
 
 "value":1234,
 
 "category":"salary"
 
 },
 
  {
 
 "value":-23,
 
 "category":"transport"
 
 },
 
  {
 
 "value":-24,
 
 "category":"transport"
 
 },
 
  {
 
 "value":465,
 
 "category":"salary"
 
 },
 
  {
 
 "value":-453,
 
 "category":"shopping"
 
 },
 
  {
 
 "value":-200,
 
 "category":"shopping"
 
 },
 
 ]
 
 }
 
Caution! This function should not be case-sensitive, meaning add_transaction(transactions_history, "shopping", -200), add_transaction(transactions_history, "Shopping", -200), and even add_transaction(transactions_history, "SHOPPING", -200) should all have the same output.

Write a function get_category_value that takes this dictionary as a parameter and returns another dictionary with the category as the key and the list of values for that category as the value.

For example, get_category_value(transactions_history) will return :

{

"transport":[-42,-23,-24],

"salary":[1234,465],

"shopping":[-453]

}

Write a function show_transactions_by_category that takes a dictionary in the format of transactions_history as a parameter and returns the details of money inflows and outflows by category.

For example, show_transactions_by_category(transactions_history) will return  :

Transport :

You spent 42 euros

You spent 23 euros

You spent 24 euros

Total :   89 euros

======================

Salary :

You received 1234 euros

You received 465 euros

Total : 1699 euros

======================

Shopping :

You spent 453 euros

Total : 453 euros

======================

Balance : 1157 euros

## Exercice 4

We know that the probability of the point being inside the quarter disk is equal to pi/4. Write the function pi_approx(pts) that will use the randomly drawn points 'pts' to return an estimation of the float pi. 'pts' is a 2-dimensional list of float values

-Each item in 'pts' represents a point.

-A point is represented by an array containing exactly two numbers, x and y, such that 0 <= x <= 1 and 0 <= y <= 1.

-'pts' is never None and always contains at least one item

## Exercice 5
Supermarkets are increasingly equipped with self-checkout machines. Most of these machines only accept payment by credit card, although a significant portion of consumers still pay in cash (with bills and coins). One of the challenges encountered with cash payment is providing optimal change, meaning with the minimal number of coins and bills. This is a problem that each of us faces daily, especially at self-checkout machines.

In this exercise, you are asked to find an optimal solution for providing change in a specific case: when a self-checkout machine contains only 2€ coins, 5€ bills, and 10€ bills. To simplify the problem, we will assume that all these coins and bills are available in unlimited quantities.

The change is expressed as a dictionary with three keys: 'two', 'five', and 'ten', which respectively represent the number of 2€ coins, 5€ bills, and 10€ bills.

For example, if we take example #2 from the table (6€), we should obtain the following dictionary:

'two': 3, # 3 coins of 2€

'five': 0 # no 5€ bills

'ten': 0 # no 10€ bills

Implement the change(cash) function, which returns a dictionary with the 'two', 'five', and 'ten' attributes representing the change to be provided. If it is impossible to provide the change (as in example #1), return None. To earn maximum points, your solution should always provide change when possible and with the minimum number of coins and bills.

Constraints: 0 < Cash < 9007199254740991"

## Exercice 6

Create two Python functions that transform a list as follows:
[1, 1, 1, 2, 3, 3, 1, 5, 10, 10, 10] ==> [1, 2, 3, 1, 5, 10]
Repetitions are eliminated. The name of the function will be 'comprime', which takes a list 'data' as an argument and returns a list. Check for special cases that could lead to errors.

(1, 1, 1, 2, 3, 3, 1, 5, 10, 10, 10) ==> [1, 3, 2, 1, 3, 2, 1, 1, 5, 1, 10, 3]

Repetitions are eliminated, and the number of consecutive identical elements is immediately replaced by the value. 
The name of the function will be 'compte', which takes a list as an argument ('compte(data)') and returns a list.

For both versions, provide the result of these functions for the example (1, 1, 1, 2, 3, 3, 1, 5, 10, 10, 10). 

