
# Web Development - Structure


## 🎓 Course

|      |	**Course** |	**File** |
| ---- | ---- | ---- |
| **01**	| **Selection by Tag** | **Ex03.html** |
| **02**	| **Selection by Class name** | **Ex04.html** |
| **03**	| **Chain syntax: append().text()** | **Ex05.html** |
| **04**	| **B attr() Method** | **Ex06.html** |
| **05**	| **C style() Method** | **Ex07.html** |
| **06**	| **enter()、update() and exit()** | **Ex08.html** |
| **07**	| **Review: Drawing a line and shapes** | **Ex09.html** |
| **08**	| **SVG Using D3.js to do the same thing** | **Ex10.html** |
| **09**	| **Rectangle Using D3.js** | **Ex11.html** |
| **10**	| **Circle Using D3.js** | **Ex12.html** |




#### 🎓 Selection by Tag

**You can select HTML elements using its TAG. The following syntax is used to select the “div” tag elements**



```Ex03.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>
    </head>
    
    <body>
        <div> Hello World ! </div>

        <script>

            alert(d3.select("div").text());
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex03 Results.png" alt="Ex03 Results"/>

___




#### 🎓 Selection by Class name

**HTML elements styled using CSS classes can be selected by using
the following syntax.**



```Ex04.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>
    </head>
    
    <body>
        <div class="myclass">
            Kun Shan University !
        </div>

        <script>

            alert(d3.select(".myclass").text());
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex04 Results.png" alt="Ex04 Results"/>

___


#### 🎓 Selection by ID

**Every element in a HTML page should have a unique ID. We can use this unique ID of an element to access 
it using the select() method as specified below.**


```Selection by ID 
<body>
    <div class="hello">
        Hello World !
    </div>

    <script>

        alert(d3.select("#hello").text());
    </script>
</body>
```




#### 🎓 Chain syntax: append().text()

```Ex05.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>
    </head>
    
    <body>
        <div class="myclass">
            Kun Shan University !
        </div>

        <script>

            d3.select("div.myclass").append("span").text("from D3.js");
        </script>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex05 Results.png" alt="Ex05 Results"/>

___




#### 🎓 B attr() Method

**The attr() method is used to add or update the attribute of the selected elements.**

```Ex06.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>
    </head>
    
    <body>
        <div class="myclass">
            Spider Man !
        </div>

        <script>

            d3.select("div.myclass").attr("style", "color: blue");
        </script>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex06 Results.png" alt="Ex06 Results"/>

___




#### 🎓 C style() Method

**The style() method is used to set the style property of the selected elements.**

```Ex07.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>
    </head>
    
    <body>
        <h2 id="myclass"> Wang </h2>
        <h2 class="myclass"> KSU </h2>
        <div class="myclass"> IE Dept </div>

        <script>

            d3.selectAll(".myclass").attr("style", "color: blue");
            d3.selectAll("#myclass").style("color", "red");
        </script>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex07 Results.png" alt="Ex07 Results"/>

___


#### 🎓 enter()、update() and exit()

```Ex08.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>
    </head>
    
    <body>
        <ul id="list">
            <li></li>
            <li></li>
        </ul>

        <input type="button" name="Remove" value="Remove Fourth Value"
               onclick="javascript:remove()"/>

        <script>

            d3.select("#list").selectAll("li")
              .data([10, 20, 30, 25, 15])
              .text( function(N) {
                return "This is pre-existing element and the value is" + N;
              })
              .enter()
              .append("li")
              .text( function(N) {
                return "This is dynamically created element and the value is" + N;
              })

            function remove() {
                d3.selectAll("li")
                  .data([10, 20, 30, 15])
                  .exit()
                  .remove()
            }
        </script>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex08 Results.png" alt="Ex08 Results"/>

___





#### 🎓 Review: Drawing a line and shapes

```Ex09.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>
    </head>
    
    <body>

        <div id="svgcontainer">

            <svg width = "300" height = "300">

                <line x1 = "100" y1 = "100"
                        x2 = "200" y2 = "200"
                        style = "stroke:rgb(255, 0, 0); 
                                stroke-width:2"/>
            </svg>
        </div>

        <p></p>
        <p></p>

    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex09 Results.png" alt="Ex09 Results"/>

___








#### 🎓 SVG Using D3.js to do the same thing 

```Ex10.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>
    </head>
    
    <body>

        <div id="svgcontainer"></div>

        <script language = "javascript">

            var width = 300;
            var height = 300;
            var svg = d3.select("#svgcontainer")
                        .append("svg")
                        .attr("width", width)
                        .attr("height", height);

                svg.append("line")
                   .attr("x1", 100)
                   .attr("y1", 100)
                   .attr("x2", 200)
                   .attr("y2", 200)
                   .style("stroke", "Rgb(255, 0, 0)")
                   .style("stroke-width", 2);
        </script>

    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex10 Results.png" alt="Ex10 Results"/>

___



#### 🎓 Rectangle Using D3.js

```Ex11.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>
    </head>
    
    <body>

        <div id="svgcontainer"></div>

        <script language = "javascript">

            var width = 300;
            var height = 300;
            var svg = d3.select("#svgcontainer")
                        .append("svg")
                        .attr("width", width)
                        .attr("height", height);

                svg.append("rect")
                   .attr("x", 20)
                   .attr("y", 20)
                   .attr("width", 200)
                   .attr("height", 100)
                   .attr("fill", "green");
        </script>

    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex11 Results.png" alt="Ex11 Results"/>

___







#### 🎓 Circle Using D3.js

```Ex12.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>
    </head>
    
    <body>

        <div id="svgcontainer"></div>

        <script language = "javascript">

            var width = 300;
            var height = 300;
            var svg = d3.select("#svgcontainer")
                        .append("svg")
                        .attr("width", width)
                        .attr("height", height);

                svg.append("circle")
                   .attr("cx", 200)
                   .attr("cy", 100)
                   .attr("r", 80)
                   .attr("fill", "green");
        </script>

    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex12 Results.png" alt="Ex12 Results"/>

___
