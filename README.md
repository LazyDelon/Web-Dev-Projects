# Web Development for Beginners - A Curriculum
[![Semantic｜語法更有意義](svg)](位置)
[![Offline Storage｜離線存取](svg)](位置)
[![Device Access｜設備兼容性](svg)](位置)
[![Connectivity｜連線、即時通訊](svg)](位置)
[![Multimedia｜網頁多媒體](svg)](位置)
[![3D/ Effects/ Graphics｜3D圖形及特效](svg)](位置)
[![Integration/ Performance｜效能與整合](svg)](位置)

➤  **資料來源：**[**xxxx**](https://zh.wikipedia.org/zh-tw/HTML5) 

## 📣 What is HTML5?

**HTML5 is the fifth revised version of HTML. The standard was completed by W3C in October 2014.**

**Broadly speaking, HTML5 refers to a set of technology combinations that include HTML, CSS and JavaScript. These three technologies have also been innovated, with the purpose of reducing the need for plug-ins in web browsers, such as: Adobe Flash, Microsoft Silverlight, and Oracle JavaFX. And provide more standards sets that can effectively enhance network applications.**

**Among them, HTML5 has added new projects that in the past could only be completed with Flash.For example, functions such as video, audio, drawing, and animation...Adobe Flash will cease to be fully updated in 2020, and the affected mainstream browsers will stop supporting Adobe Flash!**

➤  **資料來源：** [**維基百科**](https://zh.wikipedia.org/zh-tw/HTML5)   

&nbsp; <img src="./Images/Semantic Element Differences .jpg" alt="Differences"/>

**HTML5 not only adds new audio and video functions, but also adds many more meaningful grammatical features and elements, using grammatical tags to make the structure simpler! In the past, websites would be full of `<div>` and `<table>` wrapping content, but now you only need to use `<section>`, `<article>`, `<header>`, `<footer>`, `<aside>` and `<nav>`, so that The source code of the web page is more simplified and structured, so that crawlers can better understand the content of the website, thus improving search engine rankings!**

➤  **資料來源：**[**W3School 標籤列表**](https://www.w3schools.com/tags/default.asp) 


## 📋 Setting up your environment

### Create a new folder for your website

#### 1. Open Visual Studio Code。

&nbsp;&nbsp; **When you start Visual Studio Code, the Welcome page opens.**  
&nbsp;&nbsp; **Note that you can create new files or open folders in the Start list.**

&nbsp; <img src="./Images/vscode - get started.png" alt="Get Started"/>

#### 2. Open Folder

- [ ] **Select Open Folder from the Start list in Welcome,**  
- [ ] **Select File > Open Folder from the Visual Studio Code menu.**

&nbsp; <img src="./Images/vscode - open folder.png" alt="Open Folder"/>

#### 3. Create Some Files

&nbsp; <img src="./Images/vscode - explorer view.png" alt=" Create Files"/>

#### 4. Install Extension Modules or Kits

&nbsp; <img src="./Images/vscode - extension.png" alt="Mod or Kits"/>

#### 5. Open in Browser

&nbsp; <img src="./Images/vscode - open in browser.png" alt="Open in Browser"/>

#### 6. View the Page Using Developer Tools

&nbsp; <img src="./Images/vscode - developer tools elements tab.png" alt="Using Developer Tools"/>

>  **Recommended Visual Studio Code extensions:**
>
> * **[Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer&WT.mc_id=academic-77807-sagibbon) - to preview HTML pages within Visual Studio Code**
> * **[Copilot](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot&WT.mc_id=academic-77807-sagibbon) - to help you write code faster**

➤  **資料來源：**[**使用 Visual Studio Code 開始進行網頁程式開發**](https://learn.microsoft.com/zh-tw/training/modules/get-started-with-web-development/) 

## 🌱 Quickstart - HTML Tag Structure

**A minimal HTML Tag Structure looks something like this：**  
**You can open it in the Example.html file in the 1 - Structure folder.**

```html
<!Doctype HTML>
<html>
	<head>
		<title>
			My Website
		</title>
	</head>
	<body>
		Hello, World!	
	</body>
</html>
```














```bash
                    ╭┈┈┈┈┈┈┈┈┈┈┈╮
                    ┆  Element  ┆
                    ╰┈┈┈┈┈┬┈┈┈┈┈╯
                          ▼ 
     ╭┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┴┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈╮
  開始標籤              文本内容               結束標籤
     ▼               ╰┈┈┈┈┬┈┈┈┈╯               ▼
╭┈┈┈┈┴┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┴┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┴┈┈┈┈╮
┆ <div class="ab">   this my content        </div>  ┆
╰┈┈┈┈┈┈╱┈┈┈┈┈┈┈┈╲┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈╲┈┈┈┈┈╯
   属性名稱      属性值                    注意结束"/"符號
    name        value
     ╰┈┈┈┈┈┈┬┈┈┈┈┈╯
     Attribute(属性)
```


#### 1. HTML5 Semantic Layout Section

**There are many new semantic tags (semantic elements) in the HTML5 standard, which allow web pages to create more semantically structured content, helping search engines and developers to more clearly interpret the structure of web pages, so making good use of HTML5 semantic tags can also Enhance the SEO (search engine optimization) of web pages.**

**The main semantic structure tags of HTML5 are `<section>`, `<article>`, `<nav>`, `<header>`, `<footer>`, `<main>`, and `<aside>`。Use semantic tags to replace the semantically meaningless `<div>` in older versions.**

&nbsp; <img src="./Images/Semantic Element .png" alt="Semantic Element"/>

#### 2. HTML5 Web Storage

HTML5 provides a technology that can store data on the client side, which is divided into "Local Storage" and "Session Storage". The difference between the two is：

* Local Storage：can store data across pages, and the data will not disappear when the page is closed (for example: some website forms will still remember the information entered before when we close and reopen them halfway through filling in the form)

* Session Storage: Data cannot be stored across pages. The data will disappear when the page is closed.

| Parameters | Local Storage | Session Storage | 
| ---- | ---- | ---- | 
| Capacity | 10 Mb | 5 Mb | 
| Browser | HTML5 | HTML5 | 
| Accessible from | Any Window | Same tab |
| Expires | Never | On tab close |
| Storage location | Browser only | Browser only | 
| Sent with requests | No | No |


### Device Access

### Connectivity

### Multimedia
### 3D/ Effects/ Graphics
### Integration/ Performance
