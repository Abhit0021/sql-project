# sql-project
sql project on personal expnse tracker

CREATE TABLE users (

  userid int,
  
  name varchar(15),
  
  email varchar(20)
  
);

CREATE TABLE categories(

  categorieId int,
  
   categoriename varchar(15),
   
   categorieuserId int
   
);

CREATE TABLE transactions(

transactionid int,

amount int,

date varchar(15),

description varchar(17),

);

CREATE TABLE income(

incomeid int,

amount int,

source varchar(15),

date varchar(15)

);

CREATE TABLE goals(

goalid int,

name varchar(15),

targetamount int,

currentamount int,

deadline varchar(15)

);

CREATE TABLE recurring_expenses(

recurringid int,

amount int,

categoryid int,

frequency varchar(15),

startdate varchar(15),

enddate varchar(11)

);

INSERT INTO users(userid,name,email) 

VALUES (1, 'Vishesh', 'Vishesh@gmail.com');

INSERT INTO users(userid,name,email) 

VALUES (2, 'Abhit', 'abhit@gmail.com');

INSERT INTO users(userid,name,email) 

VALUES (3, 'Aditya', 'Aditya@gmail.com');

INSERT INTO users(userid,name,email) 

VALUES (4, 'Prawahan', 'Prawahan@gmail.com');

INSERT INTO users(userid,name,email) 

VALUES (5, 'Abeer', 'Abeer@gmail.com');

INSERT INTO users(userid,name,email) 

VALUES (6, 'Yash', 'Yash@gmail.com');

INSERT INTO users(userid,name,email) 

VALUES (7, 'Chirag', 'Chirag@gmail.com');


  INSERT INTO categories(categorieId,categoriename,categorieuserId) 
  
VALUES(1,'Groceries',1);

  INSERT INTO categories(categorieId,categoriename,categorieuserId) 
  
VALUES(2,'Rent',1);

  INSERT INTO categories(categorieId,categoriename,categorieuserId) 
  
VALUES(3,'Utilities',2);

  INSERT INTO categories(categorieId,categoriename,categorieuserId) 
  
VALUES(4,'Entertainment',3);

  INSERT INTO categories(categorieId,categoriename,categorieuserId) 
  
VALUES(5,'Health',4);

  INSERT INTO categories(categorieId,categoriename,categorieuserId) 
  
VALUES(6,'Transport',5);

  INSERT INTO categories(categorieId,categoriename,categorieuserId) 
  
VALUES(7,'Education',6);

 INSERT INTO transactions(transactionid,amount,date,description ) 
 
VALUES(1,50,'2025-01-01','weekly Groceries');

 INSERT INTO transactions(transactionid,amount,date,description ) 
 
VALUES(2,1000,'2025-01-01','monthly rent');

 INSERT INTO transactions(transactionid,amount,date,description ) 
 
VALUES(3,60,'2025-01-01','bills');

 INSERT INTO transactions(transactionid,amount,date,description ) 
 
VALUES(4,30,'2025-01-01','movie tickets');

 INSERT INTO transactions(transactionid,amount,date,description ) 
 
VALUES(5,200,'2025-01-01','savings deposit');

 INSERT INTO transactions(transactionid,amount,date,description ) 
 
VALUES(6,75,'2025-01-01','doctor visit');

 INSERT INTO transactions(transactionid,amount,date,description ) 
 
VALUES(7,40,'2025-01-01','taxi ride');

 INSERT INTO income(incomeid,amount,source,date) 
 
VALUES(1,5000,'Salary','2025-01-01');

INSERT INTO income(incomeid,amount,source,date) 

VALUES(2,3000,'Freelance','2025-01-01');

INSERT INTO income(incomeid,amount,source,date) 

VALUES(3,4000,'Business','2025-01-01');

INSERT INTO income(incomeid,amount,source,date) 

VALUES(4,2500,'Part time job','2025-01-01');

INSERT INTO income(incomeid,amount,source,date) 

VALUES(5,1500,'Investment','2025-01-01');

INSERT INTO income(incomeid,amount,source,date) 

VALUES(6,2000,'Consultant','2025-01-01');

INSERT INTO income(incomeid,amount,source,date) 

VALUES(7,1000,'Other','2025-01-01');

INSERT INTO goals(goalid,name,targetamount,currentamount,deadline) 

VALUES(1,'Vacation',2000,500,'2025-12-31');

INSERT INTO goals(goalid,name,targetamount,currentamount,deadline) 

VALUES(2,'Car',10000,2000,'2026-06-30');

INSERT INTO goals(goalid,name,targetamount,currentamount,deadline) 

VALUES(3,'Education',15000,5000,'2027-05-15');

INSERT INTO goals(goalid,name,targetamount,currentamount,deadline) 

VALUES(4,'Home',50000,10000,'2030-01-01');

INSERT INTO goals(goalid,name,targetamount,currentamount,deadline) 

VALUES(5,'Wedding',30000,10000,'2028-09-15');

INSERT INTO goals(goalid,name,targetamount,currentamount,deadline) 

VALUES(6,'Charity',5000,500,'2025-07-01');

INSERT INTO goals(goalid,name,targetamount,currentamount,deadline) 

VALUES(7,'Travel',8000,1000,'2026-11-20');

INSERT INTO recurring_expenses(recurringid,amount,categoryid,frequency,startdate,enddate) 

VALUES(1,1000,2,'monthly','2025-01-01','2025-12-31');

INSERT INTO recurring_expenses(recurringid,amount,categoryid,frequency,startdate,enddate)

VALUES(2,50,1,'weekly','2025-01-01','2025-06-30');

INSERT INTO recurring_expenses(recurringid,amount,categoryid,frequency,startdate,enddate) 

VALUES(3,60,3,'monthly','2025-01-01','2025-12-31');

INSERT INTO recurring_expenses(recurringid,amount,categoryid,frequency,startdate,enddate) 

VALUES(4,200,4,'quarterly','2025-01-01','2025-01-01');

INSERT INTO recurring_expenses(recurringid,amount,categoryid,frequency,startdate,enddate) 

VALUES(5,300,5,'annually','2025-01-01','2025-12-31');

INSERT INTO recurring_expenses(recurringid,amount,categoryid,frequency,startdate,enddate) 

VALUES(6,500,6,'monthly','2025-01-01','2025-12-31');

INSERT INTO recurring_expenses(recurringid,amount,categoryid,frequency,startdate,enddate) 

VALUES(7,100,2,'weekly','2025-01-01','2025-03-31');

SELECT * FROM users;

SELECT * FROM categories;

SELECT * FROM transactions;

SELECT * FROM income;

SELECT * FROM goals;

SELECT * FROM recurring_expenses;
