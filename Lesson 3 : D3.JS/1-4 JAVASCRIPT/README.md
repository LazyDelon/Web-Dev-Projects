

# D3.JS Development for Beginners - JAVASCRIPT

## 🎓 Course

|      |	**Course** |	**File** |
| ---- | ---- | ---- |
| **01**	| **Change HTML Content** | **Ex21.html** |
| **02**	| **Change Attribute Value** | **Ex22.html** |
| **03**	| **Change CSS** | **Ex23.html** |
| **04**	| **Hide HTML Elements** | **Ex24.html** |
| **05**	| **JavaScript in `<head>`** | **Ex25.html** |
| **06**	| **External JavaScript** | **Ex26.html** |
| **07**	| **JavaScript Variables** | **Ex27.html** |
| **08**	| **The typeof Operator** | **Ex28.html** |
| **09**	| **The typeof Operator** | **Ex29.html** |
| **10**	| **Difference Between Null and Undefined** | **Ex30.html** |
| **11**	| **JavaScript Functions** | **Ex31.html** |
| **12**	| **Objects Definition** | **Ex32.html** |
| **13**	| **Creating an Array** | **Ex33.html** |
| **14**	| **Using the JavaScript Keyword new** | **Ex34.html** |
| **15**	| **Access the Elements of an Array** | **Ex35.html** |


#### 🎓 Change HTML Content

**One of many JavaScript HTML methods is getElementById().**

* **The example below "finds" an HTML element (with id="demo"), and changes the element content (innerHTML) to "Hello KUN Shan University":**

```Ex21.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> What Can JavaScript Do？ </h2>

        <p id="demo"> JavaScript Can Change HTML Content. </p>

        <button type="button" onclick='document.getElementById("demo").innerHTML = "Hello Ksu Shan University！"'> Click Me！ </button>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex21 Results.png" alt="Ex21 Results"/>

___




#### 🎓 Change Attribute Value

```Ex22.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2>What Can JavaScript Do?</h2>

        <p>JavaScript Can Change HTML Attribute Values.</p>

        <p>In This Case JavaScript Changes the Value of the src (source) attribute of an image.</p>

        <button onclick="document.getElementById('MyImage').src='pic_bulbon.gif'"> Turn on the light </button>

        <img id="MyImage" src="pic_bulboff.gif" style="width: 100px;">

        <button onclick="document.getElementById('MyImage').src='pic_bulboff.gif'"> Turn off the light </button>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex22 Results.png" alt="Ex22 Results"/>

___




#### 🎓 Change CSS


```Ex23.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2>What Can JavaScript Do?</h2>

        <p id="demo"> JavaScript Can Change the style of an HTML Element. </p>

        <button type="button" onclick="document.getElementById('demo').style.fontSize='35px'"> Click Me！ </button>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex23 Results.png" alt="Ex23 Results"/>

___




#### 🎓 Hide HTML Elements


```Ex24.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2>What Can JavaScript Do?</h2>

        <p id="demo"> JavaScript Can Hide HTML Elements. </p>

        <button type="button" onclick="document.getElementById('demo').style.display='none'"> Click Me！ </button>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex24 Results.png" alt="Ex24 Results"/>

___




#### 🎓 JavaScript in `<head>`


```Ex25.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <script>

            function MyFunction() {
                document.getElementById("demo").innerHTML = "Paragraph Changed.";
            }
        </script>
    </head>
    
    <body>
        
        <h2> JavaScript in Head </h2>

        <p id="demo"> A Paragraph. </p>

        <button type="button" onclick="MyFunction()"> Try It！ </button>
    </body>
</html>
```



#### ➤ Result

&nbsp; <img src="./Images/Ex25 Results.png" alt="Ex25 Results"/>

___


#### 🎓 External JavaScript

**External JavaScript Advantages**

* **Placing scripts in external files has some advantages:**

* **It separates HTML and code**

* **It makes HTML and JavaScript easier to read and maintain**

* **Cached JavaScript files can speed up page loads**

* **To add several script files to one page - use several script tags:**

```Ex26.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> External JavaScript </h2>

        <p id="demo"> A Paragraph. </p>

        <button type="button" onclick="MyFunction()"> Try It！ </button>

        <p> (MyFunction is stored in an external file called "Ex26.js") </p>
        
        <script src="Ex26.js"> </script>
    </body>
</html>
```

```Ex26.JS
function MyFunction() {
    document.getElementById("demo").innerHTML = "Paragraph Changed.";
}
```


#### ➤ Result

&nbsp; <img src="./Images/Ex26 Results.png" alt="Ex26 Results"/>

___





#### 🎓 JavaScript Variables

```Ex27.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> JavaScript Variables </h2>

        <p> In This Example x, y and z are Variables. </p>

        <p id="demo"> </p>

        <script>

            var x = 5;
            var y = 15;
            var z = x + y;

            document.getElementById("demo").innerHTML = "The Value Of Z is： " + z;
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex27 Results.png" alt="Ex27 Results"/>

___



#### 🎓 JavaScript Types are Dynamic

* **JavaScript has dynamic types. This means that the same variable can be used to hold different data types:**

```
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> JavaScript Data Types </h2>

        <p> 
            JavaScript has dynamic types. 
            This means that the same variable 
            can be used to hold different data types： 
        </p>

        <p id="demo"> </p>

        <script>

            var x;      //Now x is underfined
             
            x = 5;      //Now x is a Number

            x = "John"; //Now x is a String
        </script>
    </body>
</html>
```




#### 🎓 JavaScript Identifiers

**All JavaScript variables must be identified with unique names.
These unique names are called identifiers. The general rules for
constructing names for variables (unique identifiers) are:**

* **Names can contain letters, digits, underscores, and dollar signs.**
  
* **Names must begin with a letter**

* **Names can also begin with $ and _ (but we will not use it in this tutorial)**
  
* **Names are case sensitive (y and Y are different variables)**
  
* **Reserved words (like JavaScript keywords) cannot be used as names**
  
**JavaScript identifiers are case-sensitive.**




#### 🎓 The typeof Operator

* **You can use the JavaScript typeof operator to find the type of a JavaScript variable. The typeof operator returns the type of a variable or an expression:**

```Ex28.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> JavaScript TypeOf </h2>

        <p> 
            The typeof operator returns the 
            types of a variable or an expression. 
        </p>

        <p id="demo"> </p>

        <script>

            document.getElementById("demo").innerHTML = 
            typeof ""       +   "<br>"  +
            typeof "john"   +   "<br>"  +
            typeof "John Doe";
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex28 Results.png" alt="Ex28 Results"/>

___




#### 🎓 The typeof Operator

```Ex29.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> JavaScript TypeOf </h2>

        <p> 
            The typeof operator returns the 
            types of a variable or an expression. 
        </p>

        <p id="demo"> </p>

        <script>

            document.getElementById("demo").innerHTML = 
            typeof 0        +   "<br>"  +
            typeof 314      +   "<br>"  +
            typeof 3.14     +   "<br>"  +
            typeof (3)      +   "<br>"  +
            typeof (3 + 4);
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex29 Results.png" alt="Ex29 Results"/>

___




#### 🎓 Difference Between Null and Undefined

```Ex30.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> JavaScript </h2>

        <p> Underfined and null are equal in value but different in type： </p>

        <p id="demo"> </p>

        <script>

            document.getElementById("demo").innerHTML = 
            typeof null              +   "<br>"       +
            typeof undefined         +   "<br> <br>"  +
            (null == undefined)      +   "<br>"       +
            (null === undefined);
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex30 Results.png" alt="Ex30 Results"/>

___





#### 🎓 JavaScript Functions


* **A JavaScript function is a block of code designed to perform a particular task. A JavaScript function is executed when "something" invokes it (calls it).**
  

```Ex31.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> JavaScript Functions </h2>

        <p> 
            This example calls a function which performs
            a calculation, and returns the result： 
        </p>

        <p id="demo"> </p>

        <script>

            function MyFunction(p1, p2) {
                return p1 * p2;
            }

            document.getElementById("demo").innerHTML = MyFunction(2, 11);
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex31 Results.png" alt="Ex31 Results"/>

___


#### 🎓 JavaScript Function Syntax 

* **A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses (). Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).**

* **The parentheses may include parameter names separated by commas: (parameter1, parameter2, ...) The code to be executed,
by the function, is placed inside curly brackets: { }**



#### 🎓 Objects Definition

```Ex32.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> JavaScript Objects </h2>

        <p id="demo"> </p>

        <script>

            var person = {
                FirstName:  "Lazy"  ,
                LastName:   "Delon" ,
                Age: 24             ,
                EyeColor: "blue"
            };

            // Display Some Data from the Object：
            document.getElementById("demo").innerHTML = person.FirstName + person.LastName
            + " is " + person.Age + " years old.";
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex32 Results.png" alt="Ex32 Results"/>

___






#### 🎓 Creating an Array

```Ex33.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> JavaScript Arrays </h2>

        <p id="demo"> </p>

        <script>

            var Cars = [
                "BMW  \t",
                "Benz \t",
                "Audi"
            ];

            document.getElementById("demo").innerHTML = Cars;
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex33 Results.png" alt="Ex33 Results"/>

___







#### 🎓 Using the JavaScript Keyword new

* **The following example also creates an Array, and assigns values to it:**

```Ex34.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> JavaScript Arrays </h2>

        <p id="demo"> </p>

        <script>

            var Cars = new Array("Mazda \t", "Toyota \t", "Porsche");

            document.getElementById("demo").innerHTML = Cars;
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex34 Results.png" alt="Ex34 Results"/>

___


* **The two examples above do exactly the same. There is no need to use new Array().**
* **For simplicity, readability and execution speed, use the first one (the array literal method).**





#### 🎓 Access the Elements of an Array

```Ex35.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> JavaScript Arrays </h2>

        <p>
            JavaScript array elements are accessed 
            using numeric indexes (starting from 0).
        </p>

        <p id="demo"> </p>

        <script>

            var Cars = ["Mazda \t", "Toyota \t", "Porsche"];

            document.getElementById("demo").innerHTML = Cars[2];
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex35 Results.png" alt="Ex35 Results"/>

___
