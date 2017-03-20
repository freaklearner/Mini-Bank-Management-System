# Mini-Bank-Management-System
Its a small application software for bank management system which offers major functions that are offered by a Bank like account creation, money deposit or withdraw and mini statements reports etc

## To run this project you need to create a Database"test" and 3 tables in it.

### Table 1: login
sql query for "login" table

create table login(
id int NOT NULL AUTO_ICREMENT,
usr varchar(100) NOT NULL,
psw varchar(100) NOT NULL,
PRIMARY KEY(id));

### Table 2: stmt
sql query for "stmt" table

create table stmt(
id int NOT NULL AUTO_ICREMENT,
acc int(10) NOT NULL,
dt datetime NOT NULL,
dbt decimal,
crdt decimal,
balance decimal,
PRIMARY KEY(id));

### Table 3: account
sql query for "account" table

create table account(
id int NOT NULL AUTO_ICREMENT,
acc int(10) NOT NULL unique,
name varchar(100) NOT NULL,
adrs varchar(200) NOT NULL,
cont char(10) NOT NULL,
balance decimal,
PRIMARY KEY(id));

### Note: Manually add a row in account table as Account number is automatically created in reference of previously created account number so to avoid having an error on running first time add a row in account table usinf insert query.











