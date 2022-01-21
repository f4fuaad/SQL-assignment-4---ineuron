# SQL-assignment-4---ineuron
Q-1. Write an SQL query to print the FIRST_NAME from Worker table after replacing ‘a’
with ‘A’.

Ans  Select  replace (FIRST_NAME,’a’,’A’)
         From Worker

Q-2. Write an SQL query to print all Worker details from the Worker table order by
FIRST_NAME Ascending and DEPARTMENT Descending.

Ans Select * from worker 
       Order by FIRST_NAME  ASC, DEPARTMENT  DESC
       
Q-3. Write an SQL query to fetch the names of workers who earn the highest salary.

Ans  select top 1 names_worker, MAX(salary)
        From  worker
        Group by names_worker
