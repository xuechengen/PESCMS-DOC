# PESCMS-DOC
After logging in to the system, enter ?g=Create&m=Doc&a=action&back_url or ?g=Create&m=Node&a=action&id=52&back_url page, 
enter="><script>alert(1);</script> after the back_url parameter, and the following page will pop up , Prove that the system has XSS vulnerabilities. 
![image](https://github.com/xuechengen/PESCMS-DOC/blob/main/5.png)
![image](https://github.com/xuechengen/PESCMS-DOC/blob/main/6.png)
Through analyzing the code, /Public/Theme/Create/Default/Doc/Doc_index.php, /Public/Theme/Doc/Default/Login/Login_index.php, 
![image](https://github.com/xuechengen/PESCMS-DOC/blob/main/1.png)
![image](https://github.com/xuechengen/PESCMS-DOC/blob/main/2.png)
![image](https://github.com/xuechengen/PESCMS-DOC/blob/main/3.png)
![image](https://github.com/xuechengen/PESCMS-DOC/blob/main/4.png)
it is found that the back_url parameter is not filtered and exists XSS vulnerability 
