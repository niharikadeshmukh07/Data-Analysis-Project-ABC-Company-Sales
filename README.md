# Data Analysis Using SQL
1. create Customer table 
   create table customer(customer_code int primary key,customer_name varchar(45),customer_type varchar(45));
   
2. load data into Customer table
   load data infile 'C:/ProgramData/MySQL/MySQL Server 8.0/Uploads/customer.csv' into table customer fields terminated by ',' ignore 1 lines;
   
3. create date table 
   create table  date (order_date varchar(45) primary key,cy_date varchar(45),year varchar(45), month_name varchar(20), date_yy_mmm varchar(45));

4. load data into date table
   load data infile 'C:/ProgramData/MySQL/MySQL Server 8.0/Uploads/date.csv' into table date fields terminated by ',' ignore 1 lines;

5. create market table
   create table market (markets_code varchar(45) primary key ,markets_name varchar(45),zone varchar(45));

6. load data into market table
   load data infile 'C:/ProgramData/MySQL/MySQL Server 8.0/Uploads/market.csv' into table market fields terminated by ',' ignore 1 lines;

7. create product table
   create table product (product_code varchar(45) primary key,product_type varchar(45));

8. load data into product table
   load data infile 'C:/ProgramData/MySQL/MySQL Server 8.0/Uploads/product.csv' into table product fields terminated by ',' ignore 1 lines;

9. create transaction table 
   create table transaction (product_code varchar(45),customer_code varchar(45),markets_code varchar(45),order_date varchar(45),sales_qty         varchar(45),sales_amount varchar(45) ,currency varchar(45));

10.load data into transaction table
   load data infile 'C:/ProgramData/MySQL/MySQL Server 8.0/Uploads/transactions.csv' into table transaction fields terminated by ',' ignore 1 lines;
 
