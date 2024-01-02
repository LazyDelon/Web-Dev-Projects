

# D3.JS Development for Beginners - Inner Crawler DOM

## 🎓 Course

|      |	**Course** |	**File** |
| ---- | ---- | ---- |
| **01**	| **A. Finding HTML Element by Id** | **Ex36.html** |
| **02**	| **xxx** | **Ex37.html** |
| **03**	| **xxx** | **Ex38.html** |
| **04**	| **xxx** | **Ex39.html** |
| **05**	| **xxx** | **Ex40.html** |
| **06**	| **xxx** | **Ex41.html** |



#### 🎓 Document Object Model (DOM)

* **The Document Object Model (DOM) is the programming interface for HTML, XML, and SVG documents. It provides a structured representation of a document (tree) and defines methods that allow programs to access and change the document's structure, style, and content. DOM provides a structured representation of documents consisting of nodes and objects that have properties and functions. Nodes can also have event handlers attached, which will be executed once the event is triggered. Essentially, it links web pages or programming languages ​​together.**

* **Although JavaScript is often used to access the DOM, it is not Part of the JavaScript language, and it can also be accessed by other languages, such as Java, C, etc.**


&nbsp; <img src="./Images/D3.JS DOM Tree.png" alt="DOM Tree"/>


#### 🎓 Operations on the DOM

* **JavaScript can change all HTML elements in the page**

* **JavaScript can change all HTML attributes in the page**

* **JavaScript can change all CSS styles in the page**

* **JavaScript can remove existing HTML elements and attributes**

* **JavaScript can add new HTML elements and attributes**

* **JavaScript can react to all existing HTML events in the page**

* **JavaScript can create new HTML events in the page**

**Note: The interaction between JavaScript and HTML is handled through events, which occur when the user or browser operates on the page. When the page is loading, an event is called. When the user clicks the button, the click is also an event. Other examples include events such as pressing any key, closing the window, resizing the window, etc.**



#### 📋 Find HTML elements

* **This page teaches you how to find and access HTML elements in HTML pages. Typically, you want to use JavaScript to manipulate HTML elements.**

* **To do this, you must first find the element. There are many ways to do this:**

**A. Find HTML elements by id**
**B. Find HTML elements by tag name**
**C. Find HTML elements by category name**
**D. Find HTML elements using CSS selectors**
**E. Find HTML elements through the HTML object collection**



#### 🎓 A. Finding HTML Element by Id

* **The easiest way to find an HTML element in the DOM, is by using the element id.**

```Ex36.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> Finding HTML Elements by Id </h2>

        <p id="intro"> Hello World！ </p>
        
        <p> This example demonstrates the <b> getElementsById </b> method. </p>

        <p id="demo"> </p>

        <script>

            var MyElement = document.getElementById("intro");

            document.getElementById("demo").innerHTML = 
            "The text from the intro paragraph is " + MyElement.innerHTML;
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex36 Results.png" alt="Ex36 Results"/>

___




#### 🎓 B. Finding HTML Elements by Tag Name

* **This example finds all <p> elements:**

```Ex37.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> Finding HTML Elements by Tag Name </h2>

        <p> Index 0 </p>

        <p> Hello World！ </p>
        
        <p> This example demonstrates the <b> getElementsByTagName </b> method. </p>

        <p id="demo"> </p>

        <script>

            var MyElement = document.getElementsByTagName("p");

            document.getElementById("demo").innerHTML = 
            "The text in Second paragraph (index 1) is：" + MyElement[1].innerHTML;
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex37 Results.png" alt="Ex37 Results"/>

___




#### 🎓 C. Finding HTML Elements by Class Name

* **If you want to find all HTML elements with the same class name, use getElementsByClassName(). This example returns a list of all elements with class="intro".**

```Ex38.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> Finding HTML Elements by Class Name </h2>

        <p> Hello World！ </p>

        <p class="intro"> The DOM is very useful. </p>
        
        <p class="intro"> This example demonstrates the 
        <b> getElementsByClassName </b> method. </p>

        <p id="demo"> </p>

        <script>

            var MyElement = document.getElementsByClassName("intro");

            document.getElementById("demo").innerHTML = 
            'The first paragraph (index 0) with class="intro"：' + MyElement[0].innerHTML;
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex38 Results.png" alt="Ex38 Results"/>

___




#### 🎓 D. Finding HTML Elements by CSS Selectors

* **If you want to find all HTML elements that match a specified CSS selector
(id, class names, types, attributes, values of attributes, etc),
use the querySelectorAll() method. This example returns a list of all <p> elements with class="intro".**

```Ex39.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> Finding HTML Elements by Query Selector </h2>

        <p> Hello World！ </p>

        <p class="intro"> The DOM is very useful. </p>
        
        <p class="intro"> This example demonstrates the 
        <b> querySelector </b> method. </p>

        <p id="demo"> </p>

        <script>

            var MyElement = document.querySelectorAll("p.intro");

            document.getElementById("demo").innerHTML = 
            'The first paragraph (index 0) with class="intro"：' + MyElement[0].innerHTML;
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex39 Results.png" alt="Ex39 Results"/>

___




#### 🎓 E. Finding HTML Elements by HTML Object Collections

* **This example finds the form element with id="frm1", in the forms collection, and displays all element values:**


```Ex40.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> Finding HTML Elements Using document.forms </h2>

        <form id="form1" action="/action_page.php">

            FirstName： 
            <input type="text" name="FName" value="Lazy"> <br>

            LastName：
            <input type="text" name="LName" value="Delon"> <br><br>

            <input type="submit" value="Submit">
        </form>

        <p> Click "Try it" to display the value of each element in the form. </p>

        <button onclick="MyFunction()"> Try it </button>

        <p id="demo"> </p>

        <script>

            function MyFunction() {

                var i;
                var text = "";
                var Form1 = document.forms["form1"];

                for(i = 0; i < Form1.length; i++) {
                    text += Form1.elements[i].value + "<br>";
                }

                document.getElementById("demo").innerHTML = text;
            }
        </script>
    </body>
</html>
```



#### ➤ Result

&nbsp; <img src="./Images/Ex40 Results.png" alt="Ex40 Results"/>

___




#### 🎓 Create the Full Animation


```Ex41.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">

        <style>

            #container {
              width: 400px;
              height: 400px;
              position: relative;
              background: yellow;
            }
            #animate {
              width: 50px;
              height: 50px;
              position: absolute;
              background-color: red;
            }
        </style>
    </head>
    
    <body>
        
        <p> <button onclick="MyMove()"> Click Me </button> </p>

        <div id="container">

            <div id="animate"> </div>
        </div>

        <script>

            var id = null;
            
            function MyMove() {

                var pos = 0;
                var elem = document.getElementById("animate");

                clearInterval(id);

                id = setInterval(frame, 5);

                function frame() {

                    if(pos == 350) {

                        clearInterval(id);
                    }

                    else {
                        
                        pos++;
                        
                        elem.style.top = pos + "px";
                        elem.style.left = pos + "px";
                    }
                }
            }
        </script>
    </body>
</html>
```



#### ➤ Result

&nbsp; <img src="./Images/Ex41 Results.png" alt="Ex41 Results"/>

___
