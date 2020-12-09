# 網站安全學習目標
```
http協定
網站基本組成:網站伺服器(web server)+網站應用程式(web application)
網站應用程式(web application)==伺服器端程式(server-side programming)+客戶端程式(client-side programming)
伺服器端程式(server-side programming) = PHP(教育界常用)  ASP.NET(公家機關)  JSP(公家機關)  Python/Flask|Dnago 
客戶端程式(client-side programming|Web 應用框架)= HTML 5 + CSS 3  + JAVASCRIPT ==> 
客戶端程式Framework:Bootstrap(RWD)  jQuery|jQuery mobile  Angular(Google)

```
# 網站伺服器(web server)
```
Apache==> PHP
Tomacat ==> JSP
Spring ==> JAVE EE
IIS ==> APS.NET
```
# 網站伺服器(web server)的漏洞
```
https://www.cvedetails.com/vulnerability-list/vendor_id-45/Apache.html
```
# 網站應用程式(web application)的漏洞
```
OWASP Top Ten Web Application Security Risks(2004|2007|2010|2013|2017)
https://owasp.org/www-project-top-ten/
```
```
OWASP API Security Top 10 2019
https://owasp.org/www-project-api-security/

API1:2019 - Broken Object Level Authorization 失效的對象級授權
API2:2019 - Broken User Authentication 失效的用戶認證
API3:2019 - Excessive Data Exposure 過度的數據暴露
API4:2019 - Lack of Resources & Rate Limiting 資源缺失 & 速率限制  ==> HTTP DDOS 
API5:2019 - Broken Function Level Authorization 功能級別授權已損壞
API6:2019 - Mass Assignment 批量分配

API7:2019 - Security Misconfiguration 安全性錯誤配置
   APACHE的安全性設定==> Apache Security – 10 Tips for a Secure Installation 
   https://www.acunetix.com/blog/articles/10-tips-secure-apache-installation/
   
   incomplete or ad-hoc configurations, 
   open cloud storage, 
   misconfigured HTTP headers, 
   unnecessary HTTP methods, 
   permissive Cross-Origin resource sharing (CORS)
   verbose error messages containing sensitive information
   
API8:2019 – Injection 注入
API9:2019 - Improper Assets Management 資產管理不當
API10:2019 - Insufficient Logging & Monitoring 日誌和監控不足
```

### HTTP DOS 攻擊測試 (1)
```
# update repos first
sudo apt-get update

# Install the tool
sudo apt-get install slowhttptest

# 
slowhttptest -c 500 -H -g -o ./output_file -i 10 -r 200 -t GET -u http://yourwebsite-or-server-ip.com -x 24 -p 2

https://ourcodeworld.com/articles/read/949/how-to-perform-a-dos-attack-slow-http-with-slowhttptest-test-your-server-slowloris-protection-in-kali-linux
https://www.youtube.com/watch?v=lNzMIeyLIPM

```
### HTTP DOS 攻擊測試 (2)
```
slowhttptest – A tool to test for slow HTTP DoS vulnerabilities
https://github.com/shekyan/slowhttptest

https://blog.csdn.net/Kevinhanser/article/details/79905182
```
