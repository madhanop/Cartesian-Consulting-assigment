create database cartesian
use dataset
CREATE TABLE Customers1 (Customer_Id varchar(255) );
INSERT INTO Customers1 VALUES ('Abhinash'),('Vipin'),('Mahesh'),('Bijoy'),('Bhabani'),('Ashutosh')
CREATE TABLE Voucher (Voucher_Id varchar(255) UNIQUE);
INSERT INTO Voucher VALUES('ABXFH'),('SDFGH'),('ERTYY'),('PPLKM')
 ;with cte 
 as(select *,row_number() over(order by Customer_Id) rr from Customers1)
 ,cte2 as(select *,row_number() over(order by Voucher_Id) rr from Voucher)
    
 select Customer_Id Customer_Key,Voucher_Id Gift_Voucher_Key
 from cte c1
 join cte2 c2 on c1.rr=c2.rr



