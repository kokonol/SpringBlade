sourceList
===
select * from tfw_parameter

list
===
select p.*,e.name STATUSNAME from tfw_parameter p left join (select num,name from tfw_dict where code=901) e on p.status=e.num 