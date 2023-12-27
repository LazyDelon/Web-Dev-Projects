# XXXX

## 📣 Learn about database systems


### 1. Narrow database definition

➤ &nbsp; **Store these definitions and restrictions in a database.**

➤ &nbsp; **After faithfully abstracting and generalizing real phenomena, some integrity limits of the material are clearly defined and standardized.**


### 2. Extensive database definition

➤ &nbsp; **collection of related data.**

➤ &nbsp; **The storage method of word processing software such as Microsoft Word, Excel, and Access is called a "database."**


### 🎓 Database

➤ &nbsp; **It consists of "files" in the operating system's file system.**

➤ &nbsp; **It is managed and accessed by the "Database Management System".**

➤ &nbsp; **The size of the underlying file affects the storage space of the Database.**

➤ &nbsp; **When storage space is insufficient, the file must be expanded from the bottom layer for database use.**



### 🎓 Database System

➤ &nbsp; **Store and manage data and business ownership through database management systems.**

➤ &nbsp; **It consists of some relevant information, The "applications" that access this data form a collection of logical "applications" to meet the needs of the enterprise.**


## 📣 Structured Query Language (SQL)

### 1. Data Manipulation Language (DML)

➤ &nbsp; **Mainly used to access data in data tables or view tables.  
Commonly used instructions include: `SELECT`, `INSERT`, `UPDATE` and `DELETE`.**



### 2. Data Definition Language (DDL)

➤ &nbsp; **It mainly performs command operations such as creating, deleting, and modifying the structure definitions of different objects. For example:  `create`, `delete`, `change`.**


### 3. Data Control Language (DCL)

➤ &nbsp; **Mainly used to control the security of the database management system. Commonly used instructions include: `GRANT`, `DENY`, `REVOKE`.**



## 📋 Setting up your environment

**Please go to the official website to download XAMPP through the following link. The official website is called Apache Firiends. Because it is not called XAMPP, it is often mistaken for not being the official website. However, it is actually the official website for downloading XAMPP.**

**You can download Visual Studio Code [here](https://www.apachefriends.org/zh_tw/index.html).**




### 🎓 XAMPP

**XAMPP is a software package that can easily integrate Apache (web server), PHP (server-side language), Perl (programming language) and MariaDB (database). Through XAMPP, you can quickly and easily set up a website.**

**When setting up a website, we need to use a web server to allow visitors to connect to our website. Currently, the more common web servers include Apache HTTP server (Apache for short) and Microsoft's Internet Information Server (IIS for short). Web pages (including various files such as images, videos, etc.) can be provided to the requester through the web server.**

**There are currently many websites that use PHP + MySQL. For example, the well-known WordPress is a free and open source content management system that uses PHP and MySQL as the platform. Therefore, whether it is used for a completely self-hosted website (a website written by oneself) or using CMS such as WordPress and Joomla All can be set up through XAMPP.**

&nbsp; <img src="./Images/xampp - download.png" alt="Download"/>

**XAMPP installation is not difficult, just click a series of "YES" and "NEXT". Finally, just pay attention to the installation service selection screen. If the server is at home, just select Apache and MySQL. If If the server will be placed elsewhere, you need to check File Zilla FTP Server. This is an FTP software used to upload other data.**

### 🎓 Basic environment description

**Finally, let’s briefly explain the basic environment of XAMPP:**

&nbsp; <img src="./Images/xampp - Environment configuration.png" alt="Environment configuration"/>

$\color{red}{\textsf{1. Red box: Service and status area. When the service is started, the Module status area will turn green.}}$

$\color{blue}{\textsf{2. Blue box: Execution code, PID(s) refers to the execution code of the service on the operating system, which can be compared with the work administrator.}}$

$\color{orange}{\textsf{3. Orange box: Channel used by the service.}}$

$\color{purple}{\textsf{4. Purple box: Service control area, used to start and stop servers and modify configuration files.}}$

$\color{green}{\textsf{5. Green box: Service execution status report, used to report the current service execution status.}}$



### 🎓 Open the Web page

**Now just click on Apache's start button and you're done. At this point, the Start button will change to the Stop button. If you need to turn it off, press Stop again. If you want to completely exit xampp, you need to press the Quit button in the lower right corner to completely exit.(If you cannot exit normally, [please refer to: XAMPP cannot exit normally](https://kumo.tw/article.php?id=16).)**

&nbsp; <img src="./Images/xampp -  open web.png" alt="open the web page"/>

**Then press the Admin button and the XAMPP default webpage will automatically open. If it can be opened successfully, it means that XAMPP has been successfully installed. This webpage is located at `/xammpp/htdocst/dashboard/index.html`. It usually has the XAMPP welcome message and some Regarding XAMPP's frequently asked questions and operation instructions, you can delete the files and folders under htdocst according to your own needs, and then create your own folders and web pages.**

&nbsp; <img src="./Images/xampp -  Apache.png" alt="Apache" style="width:650px"/>

**If you need to use MySQL, remember to press the Start button of MySQL. Click Admin to connect to MySQL.**

&nbsp; <img src="./Images/xampp -  MySQL.png" alt="MySQL"/>

➤  **資料來源：** [**XAMPP 介紹、下載與教學**](https://kumo.tw/article.php?id=15#basic)   
