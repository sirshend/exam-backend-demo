In each of shells, first do
cd .. (go to the previous level ```exam_blockchains``` for activating the virtual env)
source v1/bin/activate
cd exam_approval_backend
Once all work is done, deactivate the virtual-env with ```deactivate```


sudo mongod --dbpath .
mongosh
sudo brew services start mongodb-community
While stopping:
exit from mongosh shell by pressing Ctrl+C twice
Ctrl+C from mongod.
sudo brew services stop mongodb-community

mysql.server start
sudo brew services start mysql
mysql -u root -p (and not ```mysql -u sirshendu -p 271828``` or any combination of sirshendu and/or 271828, like ```mysql -u sirshendu -p```  or ```mysql -u root -271828```)
While stopping:
```exit``` from the shell after ```mysql -u root -p```
sudo brew services stop mysql
mysql.server stop

in exam_approval_backend with virtualenv on, use
python manage.py migrate
python manage.py runserver


########################################

exam_approval_backend git:(main) mysql.server start
Starting MySQL
 SUCCESS!
➜  exam_approval_backend git:(main) sudo brew services start mysql
Password:
Warning: Taking root:admin ownership of some mysql paths:
  /usr/local/Cellar/mysql/8.0.33_3/bin
  /usr/local/Cellar/mysql/8.0.33_3/bin/mysqld_safe
  /usr/local/opt/mysql
  /usr/local/opt/mysql/bin
  /usr/local/var/homebrew/linked/mysql
This will require manual removal of these paths using `sudo rm` on
brew upgrade/reinstall/uninstall.
Warning: mysql must be run as non-root to start at user login!
==> Successfully started `mysql` (label: homebrew.mxcl.mysql)
➜  exam_approval_backend git:(main) mysql -u root -p
Enter password:
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 8
Server version: 8.0.33 Homebrew

Copyright (c) 2000, 2023, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql>


##########################################
##########################################
127.0.0.1:8000/api/register
{
    "name": "d" ,
    "role": "student" ,
    "password": "12345",
    "email": "abcd@gmail.com"
}
{
    "name": "s1" ,
    "role": "student" ,
    "password": "12345",
    "email": "s1@gmail.com"
}
{
    "name": "p1" ,
    "role": "professor" ,
    "password": "12345",
    "email": "p1@gmail.com"
}

{
    "name": "e" ,
    "role": "professor" ,
    "password": "12345",
    "email": "bbcd@gmail.com"
}


127.0.0.1:8000/api/login
{
    "name":  ,
    "password":
}


127.0.0.1:8000/api/apply-for-exam:

{
    "name": ,
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJuYW1lIjoiYzIiLCJleHAiOjE2OTI2ODgzMzN9.RrEqiG9JbkSmah5GodyZd7NZ3-jYb7-5ItjrXYh413Y",
    "partners": "pro1"
}

{
    "name": "s1",
    "token": "",
    "partners": "p1"
}
##################### students and partners must/may be lists or arrays
127.0.0.1:8000/api/approve-requests
{
    "name": "p1",
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJuYW1lIjoicDIiLCJleHAiOjE2OTI3Nzg5ODN9.FwwaB913RI__dNKZ6fPF7Wd7GHIwggWmWUWwcLqnY9c",
    "students": ["s1"]
}

{
"name": "p1",
"token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJuYW1lIjoicDEiLCJleHAiOjE2OTI3ODA0NjB9.B43P2_ORfNGmI1atXs-pZv6IduZB3t96plHmWDT3qo0",
"students": ["s2"]
}

{
"name": "p2",
"token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJuYW1lIjoicDIiLCJleHAiOjE2OTI3ODA1NjB9.aLVLpVffyjmrWEu4Vm-2MOpTbaN9tgP3_Ns1UqDSpzI",
"students": ["s2"]
}

http://127.0.0.1:8000/api/check-status/

{
    "name": "s2",
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJuYW1lIjoiczIiLCJleHAiOjE2OTI3ODAxNzB9.6OXWlyi4puFxcqS_hdZVtjh4_e9Taskn42FJYfnfrHY"
}



###############################################################################
###############################################################################
In each of shells, first do
cd .. (go to the previous level ```exam_blockchains``` for activating the virtual env)
source v1/bin/activate
cd exam_approval_backend
Once all work is done, deactivate the virtual-env with ```deactivate```


sudo mongod --dbpath .
mongosh
sudo brew services start mongodb-community
While stopping:
exit from mongosh shell by pressing Ctrl+C twice
Ctrl+C from mongod.
sudo brew services stop mongodb-community

mysql.server start
sudo brew services start mysql
mysql -u root -p (and not ```mysql -u sirshendu -p 271828``` or any combination of sirshendu and/or 271828, like ```mysql -u sirshendu -p```  or ```mysql -u root -271828```)
While stopping:
```exit``` from the shell after ```mysql -u root -p```
sudo brew services stop mysql
mysql.server stop

in exam_approval_backend with virtualenv on, use
python manage.py migrate
python manage.py runserver


########################################

exam_approval_backend git:(main) mysql.server start
Starting MySQL
 SUCCESS!
➜  exam_approval_backend git:(main) sudo brew services start mysql
Password:
Warning: Taking root:admin ownership of some mysql paths:
  /usr/local/Cellar/mysql/8.0.33_3/bin
  /usr/local/Cellar/mysql/8.0.33_3/bin/mysqld_safe
  /usr/local/opt/mysql
  /usr/local/opt/mysql/bin
  /usr/local/var/homebrew/linked/mysql
This will require manual removal of these paths using `sudo rm` on
brew upgrade/reinstall/uninstall.
Warning: mysql must be run as non-root to start at user login!
==> Successfully started `mysql` (label: homebrew.mxcl.mysql)
➜  exam_approval_backend git:(main) mysql -u root -p
Enter password:
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 8
Server version: 8.0.33 Homebrew

Copyright (c) 2000, 2023, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql>