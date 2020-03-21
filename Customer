create table customer1(
cust_no number(20),
cname varchar2(20),
city varchar2(30),
primary key(cust_no)
);
create table order1(
order_no number(15),
odate date,
cust_no number(20),
order_amt number(20),
primary key(order_no),
foreign key(cust_no)references customer1(cust_no)
);
create table item(
item_no number(10),
price number(20),
primary key(item_no)
);
create table order1_item(
order_no number(20),
item_no number(15),
foreign key(order_no)references order1(order_no),
foreign key(item_no)references item(item_no)
);
drop table order1_item;
create table warehouse(
warehouse_no number(15),
city varchar2(20),
primary key(warehouse_no)
);
create table shipment(
order_no number(20),
warehouse_no number(20),
ship_date date,
foreign key(order_no)references order1(order_no),
foreign key(warehouse_no)references warehouse(warehouse_no)
);
insert into customer1 values('771','pushpa k','bangalore');
insert into customer1 values('772','suman','mumbai');
insert into customer1 values('773','saurav','calicut');
insert into customer1 values('774','laila','hyderabad');
insert into customer1 values('775','faizal','bangalore');
commit;
select * from customer1;
insert into order1 values('111','22-jan-02','771','18000');
insert into order1 values('112','30-july-02','774','6000');
insert into order1 values('113','03-apr-03','775','9000');
insert into order1 values('114','03-nov-03','775','29000');
insert into order1 values('115','10-dec-03','773','29000');
insert into order1 values('116','19-aug-04','772','56000');
insert into order1 values('117','10-sep-04','771','20000');
insert into order1 values('118','20-nov-04','775','29000');
insert into order1 values('119','13-feb-05','774','29000');
insert into order1 values('120','13-oct-05','775','29000');
commit;
select * from order1;
