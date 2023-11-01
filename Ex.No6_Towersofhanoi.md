# Ex.No: 6   Logic Programming – Factorial of number   
### DATE:                                                                            
### REGISTER NUMBER : 212221040137
### AIM: 
To  write  a logic program  to solve Towers of Hanoi problem  using SWI-PROLOG. 
### Algorithm:
1. Start the program
2.  Write a rules for finding solution of Towers of Hanoi in SWI-PROLOG.
3.  a )	If only one disk  => Move disk from X to Y.
4.  b)	If Number of disk greater than 0 then
5.        i)	Move  N-1 disks from X to Z.
6.        ii)	Move  Nth disk from X to Y
7.        iii)	Move  N-1 disks from Y to X.
8. Run the program  to find answer of  query.

### Program:

    move(1,X,Y,_) :-
      write('Move top disk from '),
      write(X),
      write(' to '),
      write(Y),
      nl.
    move(N,X,Y,Z) :-
      N>1,
      M is N-1,
      move(M,X,Z,Y),
      move(1,X,Y,_),
      move(M,Z,Y,X).




### Output:

![Screenshot 2023-11-01 085556](https://github.com/Rakesh2k23/AI_Lab_2023-24/assets/141472158/c814cfc3-487e-4dd8-95ce-395204748155)




### Result:
Thus the solution of Towers of Hanoi problem was found by logic programming.
