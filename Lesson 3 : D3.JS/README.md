# Web Development for Beginners - D3.JS

## 📣 D3.JS Overview


### 🎓 What is D3?


* **The full name of D3 is `Data-Driven Documents`, you know it is a Data-driven documentation.**

* **In fact, it is a JavaScript function library . Using it, the main If it is used for data visualization.**

* **D3 provides a variety of easy-to-use functions that simplify JavaScript operations The difficulty of the data.**

* **Because it is JavaScript itself, you can also use JavaScript realize all functions, but D3 can reduce the workload of engineers, especially It’s about data visualization.**

* **D3 simplifies the complex steps of visualization into a few simple functions. Engineers only need to input a few simple data to convert it into various graphics.**




### 🎓 Why use D3.JS

**There are now some chart libraries from Open sources, such as Echarts,
HighCharts, G2.js, etc. So what is the difference between D3 and these chart libraries?**

* **D3 is based on SVG, which enlarges images without distortion. (Because D3.js v4 version already supports canvas).**

* **Choosing D3, you can develop any imaginable chart in your mind, giving designers a lot of freedom in design.**

* **D3 is relatively low-level, but once you master the design method and its simplicity, it is more handy than other tools. The following figure shows the difference between D3 and other visualization tools:**


&nbsp; <img src="./Images/D3.JS visualization tools.png" alt="Visualization Tools"/>



### 🎓 What is SVG

**SVG, which stands for Scalable Vector Graphics, is a graphics format used to describe two-dimensional vector graphics. It is an open standard developed by W3C.**

**SVG can use XML format to define graphics. Except for versions before IE8, most browsers support SVG and can embed SVG text directly into HTML for display. SVG has the following features:**

* **SVG draws vector graphics, so there will be no distortion when the image is enlarged.**

* **Based on XML, JavaScript event handlers can be added to each element.**

* **Each graphic is considered an object, and if you change the properties of the object, the graphic will also change.**



### 🎓 What knowledge is needed to learn D3

**What knowledge is required?**
  
* **HTML: used to configure web content**
  
* **CSS: used to style web pages**
  
* **JavaScript: an interpreter language (Interpreter) used to set the behavior of web pages**

* **DOM: Document Object Model, used to modify the content and structure of files. (when you Write the html code for your page and it will be converted into a hierarchical structure on the browser. Each tag in html is converted into an element in the DOM with a parent-child hierarchy.)**
  
* **SVG: Scalable vector graphics for drawing visual graphics**

### 🎓 HyperText Markup Language (HTML)

**As we know, HTML is used to structure the content of the webpage. It is stored in a text file with the extension ".html". For example,**


```HTML
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <title> 文檔標題 </title>
    </head>
    
    <body>
        
        文檔內容...
    </body>
</html>
```

### 🎓 Document Object Model (DOM)

**The full name of DOM is Document Object Model. The Chinese translation is Document Object Model. It looks very abstract, but in fact it defines each tag in an HTML document, including text, pictures, etc., as objects, and these objects will eventually form a [**Tree structure**](https://hackmd.io/@qhrUT5qfQ9uYar_RFMX-PQ/Skp8Q1Eed)   , there is a schematic diagram below for reference.**


&nbsp; <img src="./Images/D3.JS DOM Tree.png" alt="DOM Tree"/>


### 🎓 Way 1: down

**D3.js is an open-source library and the source code of thelibrary is freely available on the web at [**https://d3js.org**](https://d3js.org/)  website. Visit the D3.js website and download the latest version of D3.js (d3.zip). As of now, the latest version is v6.**

**After the download is complete, unzip the file and look for d3.min.js. This is the minified version of the D3.js source code. Copy the d3.min.js file and paste it into your project's root folder or any other folder, where you want to keep all the library files. Include the d3.min.js file in your HTML page as shown below.**


## 📣 A brief introduction to JavaScript

### 🎓 JavaScript

* **JavaScript is a mature dynamic programming language. When applied to HTML documents, it can provide dynamic interactive functions for web pages.**

* **JavaScript is a programming language that helps you add interactive features to your website. For example, a game might respond to, or dynamically change, content when a button is pressed or data is entered into a form.
format, and display animations, etc.**

* **You can do many things with JavaScript. You can start with simple features, such as tickers, photo albums, dynamic layouts, response button clicks, etc. After you become familiar with this programming language, you can even create applications such as games, 2D plane and three-dimensional images, database systems, etc.!**

* **JavaScript itself is very simple yet flexible.**

* **JavaScript combines HTML and CSS to build front-end web display and interactive architecture**


## 📣 Overview and Installation

### 🎓 What is D3.js?

* **D3.js is a JavaScript library used to create interactive visualizations in the browser.**

* **The D3.js library allows us to manipulate elements of a webpage in the context of a data set. 
These elements can be HTML, SVG, or Canvas elements and can be introduced, removed, 
or edited according to the contents of the data set. It is a library for manipulating the DOM objects.**

* **D3.js can be a valuable aid in data exploration, it gives you control over your data's representation and lets you add interactivity.**


### 🎓 Why Do We Need D3.js?

* **D3.js is one of the premier framework when compare to other libraries. This is because it works on the web and its
data visualizations are par excellence. Another reason it has worked so well is owing to its flexibility.**

* **Since it works seamlessly with the existing web technologies and can manipulate any part of the
document object model, it is as flexible as the Client Side Web Technology Stack (HTML, CSS, and SVG). It has a
great community support and is easier to learn.**



### 🎓 D3.js Benefits

**D3.js is an open source project and works without any plugin. 
It requires very less code and comes up with the following benefits −**

* **Great data visualization.**
* 
* **It is modular. You can download a small piece of D3.js,
    which you want to use. No need to load the whole library every time.**

* **Easy to build a charting component.**
* 
* **DOM manipulation.**

  
### 🎓 Requirements before we starts

**Before we start, we need the following components −**

* **D3.js library**
* **Editor**
* **Web browser**
* **Web server**
  
**3 ways to run D3 under different scenarios**




### 🎓 Way 1. Download

**After the download is complete, unzip the file and look for d3.min.js. 
This is the minified version of the D3.js source code. 
Copy the d3.min.js file and paste it into your project's root folder or any other folder, 
where you want to keep all the library files. Include the d3.min.js file in your HTML page as shown below.**

```D3.JS
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>
    </head>
    
    <body>

        <script>

            // write your d3 code here...
        </script>
    </body>
</html>
```

**D3.js is a JavaScript code, so we should write all our D3 code within "script" tag. 
We may need to manipulate the existing DOM elements, so it is advisable to write the D3 code just before the end of the "body" tag.**
