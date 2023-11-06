## EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands
## DATE: 06-11-23
## AIM :
To create a manager database and execute DML queries using SQL.
## DML(Data Manipulation Language)
The SQL commands that deal with the manipulation of data present in the database belong to DML or Data Manipulation Language and this includes most of the SQL statements. It is the component of the SQL statement that controls access to data and to the database. Basically, DCL statements are grouped with DML statements.
## List of DML commands:
INSERT: It is used to insert data into a table.
UPDATE: It is used to update existing data within a table.
DELETE: It is used to delete records from a database table.
## Create the table as given below:
```
create table manager(enumber number(6),ename char(15),salary number(5),commission number(4),annualsalary number(7),Hiredate date,designation char(10),deptno number(2),reporting char(10));
```
## insert the following values into the table:
```
insert into manager values(7369,'Dharsan',2500,500,30000,'30-June-81','clerk',10,'John');
insert into manager values(7839,'Subu',3000,400,36000,'1-Jul-82','manager',null,'James');
insert into manager values(7934,'Aadhi',3500,300,42000,'1-May-82','manager',30,NULL);
insert into manager values(7788,'Vikash',4000,0,48000,'12-Aug-82','clerk',50,'Bond');
```
## Q1) Update all the records of manager table by increasing 10% of their salary as bonus.
## QUERY:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/95da8277-e306-4ead-91d2-03ba418d308a)
## OUTPUT:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/660ba5a2-72b1-46c6-b8aa-bc73b2e613fa)
## Q2) Delete the records from manager table where the salary less than 2750.
## QUERY:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/3db88767-529c-4f70-8195-119da60d800b)
## OUTPUT:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/68cd986f-77e5-431f-99c3-d54240a90527)
## Q3) Display each name of the employee as “Name” and annual salary as “Annual Salary” (Note: Salary in emp table is the monthly salary)
## QUERY:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/66b670e0-1317-483d-a687-682efe4e2abb)
## OUTPUT:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/a391a9a0-845b-40eb-a551-e388d1292acf)
## Q5) List the names of Clerks from emp table.
## QUERY:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/1a1903c5-f928-4c9b-b371-93d9af055aa2)

## OUTPUT:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/4d15ded5-67af-405e-97dc-d218ed1007fb)
## Q6) List the names of employee who are not Managers.
## QUERY:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/a7b988df-a438-4fbf-b47b-a9b2391b3170)
## OUTPUT:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/c6224f1b-73cb-4e9a-b859-6962229e062b)
## Q7) List the names of employees not eligible for commission.
## QUERY:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/2f38f4a6-90e5-4193-8b25-1bcbf8def001)
## OUTPUT:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/f3da8845-efeb-46d6-8b8d-55dfd0e8fd5f)
## Q8) List employees whose name either start or end with ‘s’.
## QUERY:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/9abc26e4-1e36-4a69-99ec-e4cf4f685c59)
## OUTPUT:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/763fd3d8-aef9-4ca1-b7ab-d84ff2d20858)
## Q9) Sort emp table in ascending order by hire-date and list ename, job, deptno and hire-date.
## QUERY:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/17a149b9-6e17-4d1d-8adf-d230a2a379f7)

## OUTPUT:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/0622c012-79c9-4b54-9fa5-242d3d0af89d)

## Q10) List the Details of Employees who have joined before 30 Sept 81.
## QUERY:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/1f5ff184-57c4-4054-9673-85072bd2ecad)

## OUTPUT:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/9da342d7-fd07-445d-a4d5-1347e57e4c12)

## Q11) List ename, deptno and sal after sorting emp table in ascending order by deptno and then descending order by sal.
## QUERY:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/b5ce1576-9a7f-4d44-bc4d-436281d50cf5)

## OUTPUT:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/b9332522-11a8-4ca8-b451-afa5dd405e4d)

## Q12) List the names of employees not belonging to dept no 30,40 & 10
## QUERY:![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/c3b2b558-2a60-44c5-a8cc-45d8fc24f7ab)

## OUTPUT:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/ccf3d925-3184-4fd1-9f05-7e23f110c3e7)

## Q13) Find number of rows in the table EMP
## QUERY:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/543dc6a5-5713-49f5-af10-86eb3263ce12)

## OUTPUT:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/76548349-1aab-465b-8d64-83c4ad13c2c9)

## Q14) Find maximum, minimum and average salary in EMP table.
## QUERY:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/b7abfe9a-9496-456e-9734-760dcc574a80)

## OUTPUT:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/60e2c585-be87-45b2-b099-4abcd38b3bd9)

## Q15) List the jobs and number of employees in each job. The result should be in the descending order of the number of employees.
## QUERY:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/f4e3371e-7ce2-4ed9-9fb5-e684aaed11ab)

## OUTPUT:
![image](https://github.com/Kishore2o/EX-2-Data-Manipulation-Language-DML-and-Data-Control-Language-DCL-Commands/assets/118679883/651b8dd2-514c-4644-bd12-3452883ddb0e)

## RESULT :
To create a manager database and execute DML queries using SQL is executed successfully.
