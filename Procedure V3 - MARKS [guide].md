##### NORMAL QUERYIES

select \* from mark;

select \* from mark where st\_id="TG1702";

select \* from mark where c\_code="ICT005";

select \* from mark where st\_id="TG1702" AND c\_code="ICT005";

##### 

##### VIEWS

select \* from grade;

select \* from view v\_mark\_weight\_temp;



##### PROCEDURES

1. final marks \& grade (coursewise or studentwise or both)

CALL Final\_Marks\_Only("TG1701","ICT001");



2\. admin perspective view (to view quiz1,2,3,assignment,mid,final marks (marks out of 100), then give final mark + grade)

CALL Student\_Course\_Details('TG1701', 'ICT001'); 

