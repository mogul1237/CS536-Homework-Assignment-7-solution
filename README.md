# CS536-Homework-Assignment-7-solution

Download Here: [CS536 Homework Assignment 7 solution](https://jarviscodinghub.com/assignment/cs536-homework-assignment-7-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

Question 1:
Assume that the following productions have been added to the grammar for the moo language:
varDecl → typedef
typedef → TYPEDEF type ID SEMICOLON
What other productions need to be changed and/or added to the moo grammar to allow typedefs?
Question 2:
Now consider the name-analysis phase of the compiler. Note that, in addition to the usual errors for multiplydefined names and for uses of undefined names, the name analyzer must enforce the following rules:
The declaration typedef T xxx; is an error if T is not a built-in type (e.g., int, bool) or a struct type
(in which case T will be of the form: struct ttt) or a new type defined by a previous typedef in the
current or an enclosing scope.
The declaration typedef T xxx; is an error if xxx has already been declared in the current scope (as a
variable, function, parameter, or new type).
A variable, function, or parameter can only be declared to be of type T if T is either a built-in type or a
new type defined by a previous typedef in the current or an enclosing scope. (A variable can still be
declared to be of type struct ttt as before.)
Briefly answer each of the following questions:
a. What information should be stored with each name in the symbol table?
b. What should be done to process a typedef: typedef T xxx;?
c. What should be done to process a declaration of a variable, function, or parameter named xxx and
declared to be of type T?
d. What should be done to process the use of a name xxx in a statement?
Question 3:
Apply your solution in Question 2 and show the entries that would be in the symbol table after processing the
following declarations:
struct MonthDayYear {
int month;
int day;
int year;
};
typedef struct MonthDayYear date;
date today;
typedef int dollars;
dollars salary;
typedef dollars moreDollars;
moreDollars md;
int d;
Note that you only need to show the symbol table for this question, and you don’t need to show the symbol table
inside the struct.
