show databases;
create database if not exists anildb;

use anildb;

create table ANE
(
pid int(5),
pcode int(5),
pname varchar(20),
pprice int(5)
);

select * from ANE;

insert into ANE(pid, pcode, pname, pprice)
values(1, 37, "PEN",  5);

insert into ANE(pid, pcode, pname, pprice)
values(2, 07, "WATCH",  1500);

alter table ANE add phone_numer int(10);

alter table ANE rename to Student;
select * from Student;

delete from Student where pid=2;

alter table Student drop column pcode;

alter table ANE rename column pprice TO price;