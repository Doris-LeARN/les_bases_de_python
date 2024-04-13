## Exercice 1

Have the function **MathChallenge** take the num parameter being passed and return the next number greater than num using the same digits. 
For example if num is 123 return 132 , if it's 12453 return 12534 . If a number has no gratter permutations, return - 1 ( ie. 999)

## Exercice 2
A- The Caesar cipher is a encryption technique that involves shifting each letter by a certain number of positions in the alphabet.
For example, with a shift of 3 , "A" becomes "D" , "B" becomes "E" , and so on.
Write a Python function **encrypt_message** that takes an input string and a shift, then encrypts the text using the Caesar cipher. Ensure that the function preserves uppercase and lowercase letters and does not modify characters that are not letters 
B- Now that you have a Caesar cipher encryption function, the exercice is to write a function to decrypt a message that was encrypted using the  Caesar cipher .
Write a Python function **decrypt_message** that takes encrypted text and shifts it to decrypt it using Caesar cipher. Make sure the function works with the same shift that was used for encryption.

## Exercice 3
Justin Bieber has been kidnapped by a gang and hidden. Just before the police could raid the gang's hideout, they intercepted a coded text message from a phone in the hideout. The only evidence found was a partially burnt piece of paper with letters on it. The gang is known for using Caesar ciphers with a positive shift to encrypt messages . You believe that the paper had an original message written on it. The police can't decode it and need your help to crack the code and save Justin.. You know the code for  encrypting a Caesar cipher ( encrypt_message) , but you don't know the offset (shift) they used.

intercepted_msg = "Yn cbyvpr neevir . Ba fr pnffr rg ba erge bhir nh pnzchf q'Nobzrl-Pnyniv, Wneqva H qnaf 30zva ."

fragment = "rive"

Find the encrypted message to save Justin Bieber!

##  Exercice 4
1- Write a function named **capital_indexes** . The function takes s single parameter , which is a string. Your function should return a list of all the indexes in the string that have capital letters.
For example, calling capital_indexes("HeLlO") should return the list [0,2,4]
2- Write a function that takes a list of lists and flattens it into a one-dimensional list.
Name your function **flatten**. It should take a single parameter and return a list 
For example, calling flatten([[1,2],[3,4]]) should return the list  [1,2,3,4]

## Exercice  5 

1-
Write a function **decompose** that , given n and N satisfying 0< N < 2^n, returns a list of length n representing the binary representation ( with n digits ) of the integer N .

For example decompose(5,13) should return [1,0,1,1,0]

Note: it is recommended to determine the least significant bit first , then the second, and so on,iterating n times using Euclidean division by 2.

2-

Write a function **part** that , given a list L= [x0,x1,.....,xn-1] , of length n , returns the sorted list of indices i such that L[i]=1 .

For example part([1,0,1,1,0]) returns [0,2,3]

Mandatory : use the list comprehension


3-

From this, deduce a function **enumeration** that, given an integer n successively prints all the subsets of {0,1,2,...,n-1} . We will print the subsets in such a way that they appear in the natural order corresponding to the value of N . 

For example enumerationt(3)  prints successively [],[0],[1],[0,1],[2],[0,2],[1,2],[0,1,2]

This function should generate and print all the subsets of the set {0,1,2,.....,n-1} in a specific order



4-

For any non-null list L = [x0, x1, ..., xn-1], we define integers r and s as follows:

-r is the minimum index i in {0,1,2, ..., n-1} such that xi = 1.

-s is the largest integer (between r + 1 and n) such that for all i in [r, s - 1], xi = 1.

For example, for L = [0, 1, 1, 1, 0, 1, 1, 0, 1, 0], we have r = 1 and s = 4 because (x1, x2, x3) is the first (maximal) sequence of consecutive digits 1 contained in the list L.
If the list L is [0, 0, 1, 1, 1], we have r = 2 and s = 5.

Write a function **sequence(L)** that, given such a non-null list L, returns the pair (r, s).


5-

Let's consider a non-empty list L = [x0, x1, ..., xn] such that we have defined integers r and s as in question 4. We assume s < n. In L, we perform the following transformation, consisting of the following successive operations:

-We set all the terms in the sequence (xr, xr+1, ..., xs-1) to 0.

-We change xs to 1 (note that we assumed s < n).

-We change all the terms in the sequence (x0, x1, ..., xs-r-2) to 1.

For example, if L = [0, 0, 1, 1, 1, 0, 1, 1, 0, 1, 0], we transform L into [1, 1, 0, 0, 0, **1**, 1, 1, 0, 1, 0]. In other words, we move the last digit 1 of the sequence to the right by one position (as highlighted in the example), and we move the preceding digit 1s as far to the left as possible. This way, the count of digit 1s remains unchanged.

Write a function **successor(L)** that, given a list L satisfying s < n, modifies L according to the transformation defined above.


6-

Let p be a natural number such that 0 < p ≤ n. Consider the list L = [1, 1, ..., 1, 0, 0, 0, ..., 0] of length n, containing exactly p digits 1 followed by zeros. It can be shown (assumed here) that the successors of L (according to the procedure in 5)) describe, in natural order, the binary representations of all subsets of size p.

Write a function **generation(n, p, k)** that, given integers satisfying 0 < p < n and an integer k satisfying 1 ≤ k ≤ C(n, p), returns the k-th subset of size p from the set {0, 1, 2, ..., n-1}.

For example, generation(5, 3, 1) returns [0, 1, 2] and generation(5, 3, 2) returns [0, 1, 3].
 
