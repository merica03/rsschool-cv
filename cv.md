##Svetlana Rogaloyva
:telephone_number: +375296386944

:email: sv.rogaloyva@gmail.com

###**Objective**
My main expectations and goals:

* Improving of knowledge and get new skills of using development tools;
* Get basic understanding of the best practices of modern applications design.
## Summary I have 9 year experience of working as L2 Support engineer. Technologies I’m working with are SQL, C#, Delphi, 1C. My main responsibilities :

* Supporting of different system;
* Making some changes in the code of the programs;
* Implementation of new features in legacy enterprise applications.
The main reason I’m on this courses is that I want to improve my Web Development skills.

### Skills

-*Foreign language*	English (B1)
-*DB*	Informix, Cache, MSSQL, MySQL, Oracle
-*Programming languages*	Delphi, C#, 1C, JavaScript, HTML, CSS, Git Bash

As an example, I can give the text of the stored procedure from DB Informix: 

```CREATE PROCEDURE update_supplier(vold_list integer, vnew_list integer)

returning varchar(250);
define vorder_id integer;
define vsvc_id integer;
define vnewsvc_id integer;
define vname varchar(250);

foreach cur1 for

  select x.order_id ,y.svc_id, z.name
  into vorder_id, vsvc_id, vname 
  from (prl_order x 
  join prl_ord_svc y
  on x.order_id=y.order_id)
  join prl_svc z
  on y.svc_id=z.svc_id
  where x.id_arm=98 and x.order_date >'31.12.2015' and z.pricelist_id=vold_list
  
  select svc_id 
  into vnewsvc_id
  from prl_svc
  where pricelist_id=vnew_list and name=vname;
  
  update prl_ord_mat
  set svc_id=vnewsvc_id
  where order_id=vorder_id and svc_id=vsvc_id;

  update prl_ord_svc
  set svc_id=vnewsvc_id
  where order_id=vorder_id and svc_id=vsvc_id;

end foreach;
 return '' with resume;

end procedure;
}
```

###Education
Higher education

*2005 - 2009*
**Belarusian State University of Informatics and Radioelectronics**
The Faculty of Computer Systems and Networks