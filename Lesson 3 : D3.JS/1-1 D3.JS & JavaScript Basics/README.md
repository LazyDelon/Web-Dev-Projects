# D3.JS Development for Beginners - D3.JS & JavaScript Basics


## 🎓 Course

|      |	**Course** |	**File** |
| ---- | ---- | ---- |
| **01**	| **Download D3.js library** | **Ex01.html** |
| **02**	| **First JavaScript Example** | **Ex02.html** |




#### 🎓 Download D3.js library

```Ex01.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
        
        <!-- Load D3.JS -->
        <script src="./d3.v7.js"></script>
        <script src="./d3.v7.min.js"></script>
        <script src="./plotly-2.27.1.min.js"></script>
    </head>
    
    <body>
        
        <div id="mydiv"></div>
    </body>
</html>

<script>

    var data = [{
        values: [4, 5, 2],
        labels: ['台北', '台中', '台南'],
        type: 'pie'
    }];

    var frame = {
        width: 500,
        height: 500
    };
    Plotly.newPlot('mydiv', data, frame)
</script>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex01 Results.png" alt="Ex01 Results"/>

___


#### 🎓 First JavaScript Example

```Ex02.html
<!DOCTYPE HTML>

<html>
    <head>
        
        <meta charset="utf-8">
    </head>
    
    <body>
        
        <h2> My First JavaScript </h2>

        <button type="button" onclick="document.getElementById('demo').innerHTML = Date()">
            Click me to Display Date and Time.
        </button>

        <p id="demo"></p>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex02 Results.png" alt="Ex02 Results"/>

___
