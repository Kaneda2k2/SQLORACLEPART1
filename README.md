# SQLORACLEPART1
#NOCIONES BASICAS SQL CON ORACLE DEDICADO A JDBC
##CREAR BASE DATOS
CREATE DATABASE DABASE_NAME;
##ELIMINA BASE DE DATOS
DROP DATABASE DABASE_NAME:
##CREAR TABLA
CREATE TABLE table_name
(
column_name colum_data_type,
column_name colum_data_type,
column_name colum_data_type,
);
##CREAR TABLA CON CUATRO COLUMNAS
CREATE TABLE Employees
(
id INT NOT NULL,
age INT NOT NULL,
first VARCHAR(255),
last VARCHAR(255),
PRIMARY KEY (id)
);
##ELIMINAR TABLA
DROP TABLE table_name;
##ELIMINAR TABLA
DROP TABLE Employees;
##INSERTAR DATOS
INSERT INTO table_name VALUES (column1,column2)
##INSERTAR DATOS
INSERT INTO table_name VALUES (100,18,"Zara","Ali");
##RECUPERAR DATOS DE UNA BASE DE DATOS
SELECT column_name, column_name,
FROM table_name
WHERE conditions:
##SELECIONA LA ANTIGUEDAD ,PRIMERA Y LULTIMA COLUMNA DE LA TABLA DONDE LAA PRIMERA COLUMNA CONTIENE ZARA
SELECT first,last,age
FROM Employees 
WHERE first LIKE "%Zara%";
##SELECIONA LA ANTIGUEDAD LA PRIMERA Y LA ULTIMA COLUMN DONDE LA COLUMNA ES = 100
SELECT first,last,age
FROME Employees
WHERE id=100;
##ACTUALIZAR DATOS
UPDATE table_name
SET column_name=value,colum_name=value
WHERE conditions;
##ACTUALIZAR COMBINANDO LA EDAD DEL EMPLEADO CUYA IDENTIFICACION ES 100
UPDATE Employees SET age=20 WHERE id=100;
##BORRAR DATOS
DELETE FROM table_name WHERE conditions;
## EJEMMPLO BORRAR REGISTRO 
DELETE FROM Employees WHERE id=100;
