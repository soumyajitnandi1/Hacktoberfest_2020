# PROBLEM STATEMENT :

There are N guests (numbered 1 through N) coming to Chef's wedding. Each guest is part of a family; for each valid i, the i-th guest is part of family Fi. You need to help Chef find an optimal seating arrangement.</br></br>

Chef may buy a number of tables, which are large enough for any number of guests, but the people sitting at each table must have consecutive numbers ― for any two guests i and j (i<j) sitting at the same table, guests i+1,i+2,…,j−1 must also sit at that table. Chef would have liked to seat all guests at a single table; however, he noticed that two guests i and j are likely to get into an argument if Fi=Fj and they are sitting at the same table.</br></br>

Each table costs K rupees. Chef defines the inefficiency of a seating arrangement as the total cost of tables plus the number of guests who are likely to get into an argument with another guest. Tell Chef the minimum possible inefficiency which he can achieve.</br></br>



# INPUT :

The first line of the input contains a single integer T denoting the number of test cases. The description of T test cases follows.</br>
The first line of each test case contains two space-separated integers N and K.</br>
The second line contains N space-separated integers F1,F2,…,FN.</br>



# OUTPUT :

For each test case, print a single line containing one integer ― the smallest possible inefficiency.</br>



# CONSTRAINTS :

1≤T≤100</br>
1≤N≤1,000</br>
1≤K≤1,000</br>
1≤Fi≤100 for each valid i</br>
The sum of N across test cases is ≤5,000</br>



# INPUT FORMAT :

3</br>
5 1</br>
5 1 3 3 3</br>
5 14</br>
1 4 2 4 4</br>
5 2</br>
3 5 4 5 1</br>



# OUTPUT FORMAT :

3</br>
17</br>
4</br>



# EXPLANATION :

Example case 1: The optimal solution is to use three tables with groups of guests [1,2,3], [4] and [5]. None of the tables have any guests that are likely to get into an argument, so the inefficiency is 3⋅K=3.</br></br>

Example case 2: The optimal solution is to seat all guests at one table. Then, guests 2, 4 and 5 are likely to get into an argument with each other, so the inefficiency is K+3=17.</br>
