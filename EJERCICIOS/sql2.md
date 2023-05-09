https://www.db-fiddle.com/f/7ZftZp8ia8YKxFEWk3QET7/1

![image](https://user-images.githubusercontent.com/125502308/236016413-7df492f1-7f02-49fb-bd7b-e2dddb62a869.png)

https://www.db-fiddle.com/f/7ZftZp8ia8YKxFEWk3QET7/2
https://www.db-fiddle.com/f/7ZftZp8ia8YKxFEWk3QET7/3


CREATE DATABASE tiendita;
USE tiendita;



CREATE TABLE fabricante(
  codigo INT, PRIMARY KEY,
  nombre_fab VARCHAR(50)
 );
 
 CREATE TABLE pdrocuto(
   codigo_producto INT PRIMARY KEY,
   nombre_producto VARCHAR(100),
   precio_producto FLOAT,
   codigo1 INT, 
   FOREIGN KEY(codigo1) REFERENCES fabricante(codigo)

 );
 
 INSERT INTO fabricante VALUES(1,'SEAGATE');
 INSERT INTO fabricante VALUES(2,'CRUCIAL');
 INSERT INTO fabricante VALUES(3,'SAMSUNG');
 INSERT INTO fabricante VALUES(4,'GIGABYTE');
 INSERT INTO fabricante VALUES(5,'ASUS');
 INSERT INTO fabricante VALUES(6,'LENOVO');
 INSERT INTO fabricante VALUES(7,'HP');
 
  INSERT INTO producto VALUES(7,'HP');
