
# D3.JS Development for Beginners - IMPLEMENTATION II

## 🎓 Course

|      |	**Course** |	**File** |
| ---- | ---- | ---- |
| **01**	| **Setting Attribute Value Dynamically** | **Ex13.html** |
| **02**	| **Events in D3** | **Ex14.html** |
| **03**	| **Data Binding in D3** | **Ex15.html** |
| **04**	| **SVG Transform** | **Ex16.html** |
| **05**	| **SVG Transform for D3** | **Ex17.html** |
| **06**	| **SVG Transform for Pie** | **Ex18.html** |
| **07**	| **Read the dataset from CSV for Pie Chart** | **Ex19.html** |
| **08**	| **Read the dataset from CSV for Bar Chart** | **Ex20.html** |



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

➤  **資料來源：** [**Data Binding in D3**](https://www.tutorialsteacher.com/d3js/data-binding-in-d3js)   

&nbsp; <img src="./Images/Data Binding in D3.png" alt="Differences"/>

```Ex15.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>
    </head>
    
    <body>
        
        <p> </p>
        <p> </p>
        <p> </p>

        <script>

            var MyData = ['John', 'Doe', 'LazyDelon'];

            var p = d3.select("body")
                      .selectAll("p")
                      .data(MyData)
                      .text( function(d, i) {
                        return i + "：" + d;
                    });
        </script>   
    </body>
</html>
```

* **ps .data(myData) - the data() function then binds our data array 'myData' to the selection returned from the previous selection. Since our selection has single p element, the data() function will bind the first value from our data array to the <p> element.**


#### ➤ Result

&nbsp; <img src="./Images/Ex15 Results.png" alt="Ex15 Results"/>

___




#### 🎓 SVG Transform

* **SVG provides options to transform a single SVG shape element or group of SVG elements.
SVG transform supports Translate, Scale, Rotate and Skew.**

```Ex16.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>

        <style>

            svg rect {
                fill: orange;
            }

            svg text {
                fill: white;
                text-anchor: end;
                font: 10px sans-serif;
            }
        </style>
    </head>
    
    <body>
        
        <svg class="chart" width="420" height="120">

            <g transform="translate(0, 0)">
                <rect width="50" height="20"> </rect>
                <text x="40" y="9.5" dy=".35em"> 5 </text>
            </g>

            <g transform="translate(0, 25)">
                <rect width="100" height="20"> </rect>
                <text x="90" y="9.5" dy=".35em"> 10 </text>
            </g>

            <g transform="translate(0, 50)">
                <rect width="120" height="20"> </rect>
                <text x="110" y="9.5" dy=".35em"> 12 </text>
            </g>
        </svg>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex16 Results.png" alt="Ex16 Results"/>

___




#### 🎓 SVG Transform for D3


```Ex17.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>

        <style>

            svg rect {
                fill: orange;
            }

            svg text {
                fill: white;
                text-anchor: end;
                font: 10px sans-serif;
            }
        </style>
    </head>
    
    <body>
        
        <script>

            var data = [5, 10, 12, 15, 8]
            var width = 200, scaleFactor = 10, barHeight = 25;

            var graph = d3.select("body")
                          .append("svg")
                          .attr("width", width)
                          .attr("height", barHeight * data.length);

            var bar = graph.selectAll("g")
                           .data(data)
                           .enter()
                           .append("g")
                           .attr("transform", function(d, i){
                                return "translate(0," + i * barHeight +")";
                           });
            
            bar.append("rect")
               .attr("width", function(d){
                    return d * scaleFactor;
               })
               .attr("height", barHeight - 1)

            bar.append("text")
               .attr("x", function(d){ return (d * scaleFactor); })
               .attr("y", barHeight / 2)
               .attr("dy", ".35em")
               .text( function(d) { return d; });
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex17 Results.png" alt="Ex17 Results"/>

___


#### 🎓 SVG Transform for Pie

* **The <path> element is the most powerful element in the SVG library of basic shapes. It can be used to create lines, curves, arcs, and more. Paths create complex shapes by combining multiple straight lines or curved lines.**

```Ex18.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>
    </head>
    
    <body>

        <svg width="300" height="200"> </svg>

        <script>

            var data = [2, 4, 8, 10];
            var svg = d3.select("svg"),
                width = svg.attr("width"),
                height = svg.attr("height"),
                radius = Math.min(width, height) / 2,
                g = svg.append("g").attr("transform", "translate(" + width / 2 + "," + height / 2 + ")")

            var color = d3.scaleOrdinal(['#4da4da', '#377eb8', '#ff7f00', '#984ea3', '#e41alc'])
            
            // Generate the pie
            var pie =  d3.pie();

            // Generate the arcs 
            var arc = d3.arc()
                        .innerRadius(0)
                        .outerRadius(radius);
            
            // Generate group
            var arcs = g.selectAll("arc")
                        .data(pie(data))
                        .enter()
                        .append("g")
                        .attr("class", "arc")         

            // Draw arc paths
            arcs.append("path")
                .attr("fill", function(d, i) {
                    return color(i);
                })
                .attr("d", arc);
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex18 Results.png" alt="Ex18 Results"/>

___





#### 🎓 Read the dataset from CSV for Pie Chart

```Ex19.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <script src="./d3.v7.min.js"></script>

        <style>

            .arc text {

                text-anchor: middle;
                font: 10px sans-serif;
            }

            .arc path {

                stroke: #fff;
            }

            .title {

                fill: teal;
                font-weight: bold;
            }
        </style>
        
        <script src="https://d3js.org/d3.v4.min.js"></script>
    </head>
    
    <body>

        <svg width="600" height="500"> </svg>

        <script>

            var svg = d3.select("svg"),
                width = svg.attr("width"),
                height = svg.attr("height"),
                radius = Math.min(width, height) / 2;
                
            var g = svg.append("g")
                       .attr("transform", "translate(" + width / 2 + "," + height / 2 + ")")

            var color = d3.scaleOrdinal(['#4daf4a','#377eb8','#ff7f00','#984ea3','#e41a1c']);

            // Generate the pie
            var pie =  d3.pie().value( function(d) {
                return d.percent;
            });

            var path = d3.arc()
                         .outerRadius(radius - 30)
                         .innerRadius(0);

            var label = d3.arc()
                          .outerRadius(radius)
                          .innerRadius(radius - 120);


            d3.csv("browseruse.csv", function(error, data){

                if (error) {
                    throw error;
                }

                var arc = g.selectAll(".arc")
                           .data(pie(data))
                           .enter().append("g")
                           .attr("class", "arc");

                arc.append("path")
                   .attr("d", path)
                   .attr("fill", function(d) { return color(d.data.browser); });
            
                console.log(arc)

                
                arc.append("text")
                   .attr("transform", function(d){
                        return "translate(" + label.centroid(d) + ")";
                   })
                .text(function(d) { return d.data.browser; });
            });


            svg.append("g")
               .attr("transform", "translate(" + (width / 2 - 120) + "," + 20 + ")")
               .append("text")
               .text("Browser use statistics - Jan 2017")
               .attr("class", "title")
            
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex19 Results.png" alt="Ex19 Results"/>

___








#### 🎓 Read the dataset from CSV for Bar Chart

```Ex20.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        <!-- <script src="./d3.v7.min.js"></script> -->

        <style>

            .bar {
                fill: steelblue;
            }

            .highlight {
                fill: orange;
            }
        </style>

        <script src="https://d3js.org/d3.v4.min.js"></script>
    </head>
    
    <body>

        <svg width="600" height="500"> </svg>

        <script>

            var svg = d3.select("svg"),
                margin = 200,
                width = svg.attr("width") - margin,
                height = svg.attr("height") - margin;

            svg.append("text")
               .attr("transform", "translate(100, 0)")
               .attr("x", 50)
               .attr("y", 50)
               .attr("font-size", "24px")
               .text("Foods Stock Price")

            var Scale_X = d3.scaleBand().range([0, width]).padding(0.4);
            var Scale_Y = d3.scaleLinear().range([height, 0]);

            var g = svg.append("g")
                       .attr("transform", "translate(" + 100 + "," + 100 + ")");
        
            
            d3.csv("foodstockprice.csv", function(error, data) {

                if (error) {
                    throw error;
                }

                Scale_X.domain(data.map(function(d) { return d.year; })); 
                Scale_Y.domain([0, d3.max(data, function(d) { return d.value; })]); 

                g.append("g")
                 .attr("transform", "translate(0, " + height + ")")
                 .call(d3.axisBottom(Scale_X))
                 .append("text")
                 .attr("y", height - 250)
                 .attr("x", width - 100)
                 .attr("text-anchor", "end")
                 .attr("stroke", "black")
                 .text("Year");

                        
                g.append("g")
                 .call(d3.axisLeft(Scale_Y).tickFormat(function(d){ return "$" + d; }).ticks(10))
                 .append("text")
                 .attr("transform", "rotate(-90)")
                 .attr("y", 6)
                 .attr("dy", "-5.1em")
                 .attr("text-anchor", "end")
                 .attr("stroke", "black")
                 .text("Stock Price");

                g.selectAll(".bar")
                 .data(data)
                 .enter().append("rect")
                 .attr("class", "bar")
                 .on("mouseover", onMouseOver)
                 .on("mouseout", onMouseOut)
                 .attr("x", function(d) { return Scale_X(d.year); })
                 .attr("y", function(d) { return Scale_Y(d.value); })
                 .attr("width", Scale_X.bandwidth())
                 .transition()
                 .ease(d3.easeLinear)
                 .duration(400)
                 .delay( function(d, i) {
                    return i * 50;
                 })
                 .attr("height", function(d) {
                    return height - Scale_Y(d.value); 
                 });
            });

            //mouseover event handler function 
            function onMouseOver(d, i) {
            
                d3.select(this).attr("class", "highlight");
                d3.select(this)
                    .transition()
                    .duration(400)
                    .attr("width", Scale_X.bandwidth() + 5)
                    .attr("y", function(d) { return Scale_Y(d.value) - 10; })
                    .attr("height", function(d) { return height - Scale_Y(d.value) + 10; });
    
                g.append("text")
                .attr("class", "val")
                .attr("x", function() {
                    return Scale_X(d.year);
                })

                .attr("y", function() {
                    return Scale_Y(d.value) - 15;
                })

                .text( function() {
                    return [ "$" + d.value];
                });
            }
                       
            //mouseout event handler function
            function onMouseOut(d, i) {
                //use the text label class to remove label on mouseout
                d3.select(this).attr("class", "bar");
                d3.select(this)
                    .transition()
                    .duration(400)
                    .attr("width", Scale_X.bandwidth())
                    .attr("y", function(d) { return Scale_Y(d.value); })
                    .attr("height", function(d) { return height - Scale_Y(d.value); });

                d3.selectAll(".val").remove()
            }
        </script>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex20 Results.png" alt="Ex20 Results"/>

___


#### 🎓 Create Bar Chart using D3

**We learned about SVG charts, scales and axes in the previous chapters. Here, we will learn to create SVG bar chart with scales and axes in D3.**

**Let's now take a dataset and create a bar chart visualization. We will plot the share value of a dummy company, foodstockprice Foods, over a period from 2011 to 2016. The following foodstockprice.csv file stores share values:**


#### 📋 foodstockprice.csv

```foodstockprice.csv
year,value
2011,45
2012,47
2013,52
2014,70
2015,75
2016,78
```

**📋 Step 1: Start with creating the SVG and defining the scales for our bar chart as shown below.**

```
<body>

        <svg width="600" height="500"> </svg>

        <script>

            var svg = d3.select("svg"),
                margin = 200,
                width = svg.attr("width") - margin,
                height = svg.attr("height") - margin;

            svg.append("text")
               .attr("transform", "translate(100, 0)")
               .attr("x", 50)
               .attr("y", 50)
               .attr("font-size", "24px")
               .text("Foods Stock Price")

            var Scale_X = d3.scaleBand().range([0, width]).padding(0.4);
            var Scale_Y = d3.scaleLinear().range([height, 0]);

            var g = svg.append("g")
                       .attr("transform", "translate(" + 100 + "," + 100 + ")");
         </script> 
</body>        
```

**📋 Step 2: Let's load our data from the CSV file and add axes to the SVG.**
```
<body>

        <svg width="600" height="500"> </svg>

        <script>

            var svg = d3.select("svg"),
                margin = 200,
                width = svg.attr("width") - margin,
                height = svg.attr("height") - margin;

            svg.append("text")
               .attr("transform", "translate(100, 0)")
               .attr("x", 50)
               .attr("y", 50)
               .attr("font-size", "24px")
               .text("Foods Stock Price")

            var Scale_X = d3.scaleBand().range([0, width]).padding(0.4);
            var Scale_Y = d3.scaleLinear().range([height, 0]);

            var g = svg.append("g")
                       .attr("transform", "translate(" + 100 + "," + 100 + ")");
        
            
            d3.csv("foodstockprice.csv", function(error, data) {

                if (error) {
                    throw error;
                }

                Scale_X.domain(data.map(function(d) { return d.year; })); 
                Scale_Y.domain([0, d3.max(data, function(d) { return d.value; })]); 

                g.append("g")
                 .attr("transform", "translate(0, " + height + ")")
                 .call(d3.axisBottom(Scale_X))
                 .append("text")
                 .attr("y", height - 250)
                 .attr("x", width - 100)
                 .attr("text-anchor", "end")
                 .attr("stroke", "black")
                 .text("Year");

                        
                g.append("g")
                 .call(d3.axisLeft(Scale_Y).tickFormat(function(d){ return "$" + d; }).ticks(10))
                 .append("text")
                 .attr("transform", "rotate(-90)")
                 .attr("y", 6)
                 .attr("dy", "-5.1em")
                 .attr("text-anchor", "end")
                 .attr("stroke", "black")
                 .text("Stock Price");
        </script> 
</body>    
```


**📋 Step 3: Next, we want to create bars corresponding to the data values.**

**Since this is a vertical bar graph, the chart width will be fixed and the bar width will be variable depending on the dataset size. We will calculate the bar width by diving the chart width by the dataset size.**

**Example: Bar Chart in D3**

```
<body>

        <svg width="600" height="500"> </svg>

        <script>

            var svg = d3.select("svg"),
                margin = 200,
                width = svg.attr("width") - margin,
                height = svg.attr("height") - margin;

            svg.append("text")
               .attr("transform", "translate(100, 0)")
               .attr("x", 50)
               .attr("y", 50)
               .attr("font-size", "24px")
               .text("Foods Stock Price")

            var Scale_X = d3.scaleBand().range([0, width]).padding(0.4);
            var Scale_Y = d3.scaleLinear().range([height, 0]);

            var g = svg.append("g")
                       .attr("transform", "translate(" + 100 + "," + 100 + ")");
        
            
            d3.csv("foodstockprice.csv", function(error, data) {

                if (error) {
                    throw error;
                }

                Scale_X.domain(data.map(function(d) { return d.year; })); 
                Scale_Y.domain([0, d3.max(data, function(d) { return d.value; })]); 

                g.append("g")
                 .attr("transform", "translate(0, " + height + ")")
                 .call(d3.axisBottom(Scale_X))
                 .append("text")
                 .attr("y", height - 250)
                 .attr("x", width - 100)
                 .attr("text-anchor", "end")
                 .attr("stroke", "black")
                 .text("Year");

                        
                g.append("g")
                 .call(d3.axisLeft(Scale_Y).tickFormat(function(d){ return "$" + d; }).ticks(10))
                 .append("text")
                 .attr("transform", "rotate(-90)")
                 .attr("y", 6)
                 .attr("dy", "-5.1em")
                 .attr("text-anchor", "end")
                 .attr("stroke", "black")
                 .text("Stock Price");

                g.selectAll(".bar")
                 .data(data)
                 .enter().append("rect")
                 .attr("class", "bar")
                 .on("mouseover", onMouseOver)
                 .on("mouseout", onMouseOut)
                 .attr("x", function(d) { return Scale_X(d.year); })
                 .attr("y", function(d) { return Scale_Y(d.value); })
                 .attr("width", Scale_X.bandwidth())
                 .transition()
                 .ease(d3.easeLinear)
                 .duration(400)
                 .delay( function(d, i) {
                    return i * 50;
                 })
                 .attr("height", function(d) {
                    return height - Scale_Y(d.value); 
                 });
            });
        </script> 
</body>    
```
➤  **資料來源：** [**How do I create a bar chart using D3?**](https://www.quora.com/How-do-I-create-a-bar-chart-using-D3)   
