# 網站安全學習目標
## 基本觀念
```
http協定
網站基本組成:網站伺服器(web server)+網站應用程式(web application)
網站應用程式(web application)==伺服器端程式(server-side programming)+客戶端程式(client-side programming)
伺服器端程式(server-side programming) = PHP(教育界常用)  ASP.NET(公家機關)  JSP(公家機關)  Python/Flask|Dnago 
客戶端程式(client-side programming|Web 應用框架)= HTML 5 + CSS 3  + JAVASCRIPT ==> 
客戶端程式Framework:Bootstrap(RWD)  jQuery|jQuery mobile  Angular(Google)

```
## 測試技術
```


```

## 子模組
```
4-1.網站運作原理
4-2.網站測試技術與Web-CTF實戰
4-3.網站漏洞與測試:DVWA實戰測試
4-4.強化網站安全的技術: 原始碼檢測  漏洞掃描  滲透測試  應用程式防火牆
4-5.強化網站安全的應用程式防火牆[錄影課程|選讀課程]
4-6.強化網站安全的應用程式防火牆實戰[錄影課程|選讀課程]
```
### 4-1.網站運作原理
```
本課程將教授網站基礎運作原理、網站組成，同時理解瀏覽器與網站伺服器之間溝通協定(HTTP)
網站運作組成:
網站伺服器(web server)+網站應用程式(web application)

網站運作的協定:HTTP

```
### 4-2.網站測試技術與Web-CTF實戰
```
本課程透過CTF平台實際演練，教授學生基本的測試工具，包括developer tools、curl、burpsuite等工具，
再配合Linux系統使用常用Curl工具解題，使學生能對CTF產生熱情與興趣
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
# OWASP
```
The Open Web Application Security Project (OWASP)開放式Web應用程式安全項目（OWASP）是一個線上社群、非營利組織，
在Web應用安全領域提供免費的文章、方法、檔案、工具和技術。
```
```
OWASP Application Security Verification Standard (ASVS) ver.4 (2019)
OWASP Secure Coding Practices
OWASP Top Ten Proactive Controls (2018)
OWASP Top Ten Risks (2017)
OWASP Testing Guide v4(2014)
OWASP Cheatsheet Series

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
