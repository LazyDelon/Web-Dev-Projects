
# Web Development for Beginners - D3.JS

## 🎓 Course

|      |	**Course** |	**File** |
| ---- | ---- | ---- |
| **01**	| **Setting Attribute Value Dynamically** | **Ex13.html** |
| **02**	| **Events in D3** | **Ex14.html** |
| **03**	| **xxx** | **Ex15.html** |
| **04**	| **xxx** | **Ex16.html** |
| **05**	| **xxx** | **Ex17.html** |
| **06**	| **xxx** | **Ex18.html** |
| **07**	| **xxx** | **Ex19.html** |
| **08**	| **xxx** | **Ex20.html** |



#### 🎓 Setting Attribute Value Dynamically

* **we have used some logic to check whether the current <p> element'stext contains keywords like "Error" or "Warning". If it contains thekeyword "Error", we return the color red or if it contains the keyword"Warning", we return the color yellow in Ex13.html.**

* **String.prototype.indexOf(): The indexOf() method returns the index within the calling String object of the first occurrence of the specified value, starting the search at fromIndex. Returns -1 if the value is not
found.**

```Ex13.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>
    </head>
    
    <body>
        
        <p> Error： This is Error. </p>
        <p> Warning： This is Warning. </p>

        <script>

            d3.selectAll("p").style("color", function(d, i){

                var text = this.innerText;

                if (text.indexOf("Error") >= 0){

                    return "red";
                }

                else if (text.indexOf("Warning") >= 0) {
                    
                    return "orange";
                }
            });
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex13 Results.png" alt="Ex13 Results"/>

___




#### 🎓 Events in D3

* **As in all other libraries, D3 also supports built-in events and custom events. We can bind an event listener to any DOM element using `d3.selection.on()` method.**

* **Syntax is as right:**

* **The on() method adds an event listener to all selected DOM elements. The first parameter is an event type as string such as "click", "mouseover" etc. The second parameter is a callback function which will be executed when an event occurs and the third optional parameter capture flag may be specified, which corresponds to the W3C useCapture flag.**


```Ex14.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>

        <style>

            div {
                width: 100px;
                height: 100px;
                margin: 5px;
                background-color: steelblue;
            }
        </style>
    </head>
    
    <body>
        
        <div> </div>

        <script>

            d3.selectAll("div")
              .on("mouseover", function(){

                d3.select(this)
                  .style("background-color", "orange");

                console.log(d3.event);

                console.log(d3.mouse(this));
              })

              .on("mouseout", function(){

                d3.select(this)
                  .style("background-color", "steelblue")
              });
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex14 Results.png" alt="Ex14 Results"/>

___




#### 🎓 Data Binding in D3

* **You will learn how to bind data to DOM elements and create new elements based on your data. D3 includes the following important methods for data binding.**

#### 🎓 data() api

* **D3 is data driven. The data() function is used to join the specified array of data to the selected DOM elements and return the updated selection. D3 works with different types of data like Array, CSV, TSV, JSON, XML etc.**

* **You can pass two types of value to the data() function, an array of values (number or object) or a function of data.**

```Ex15.html

```


#### ➤ Result

&nbsp; <img src="./Images/Ex15 Results.png" alt="Ex15 Results"/>

___




#### 🎓 xxx


```Ex16.html

```


#### ➤ Result

&nbsp; <img src="./Images/Ex16 Results.png" alt="Ex16 Results"/>

___




#### 🎓 xxx


```Ex17.html

```


#### ➤ Result

&nbsp; <img src="./Images/Ex17 Results.png" alt="Ex17 Results"/>

___


#### 🎓 xxx

```Ex18.html

```


#### ➤ Result

&nbsp; <img src="./Images/Ex18 Results.png" alt="Ex18 Results"/>

___





#### 🎓 xxx

```Ex19.html

```


#### ➤ Result

&nbsp; <img src="./Images/Ex19 Results.png" alt="Ex19 Results"/>

___








#### 🎓 xxx

```Ex20.html

```


#### ➤ Result

&nbsp; <img src="./Images/Ex20 Results.png" alt="Ex20 Results"/>

___



