# Web Development - Extra


## 🎓 Course

|      |	**Course** |	**File** |
| ---- | ---- | ---- |
| **01**	| **The css settings in way 2** | **Ex30.html** |
| **02**	| **The element Selector** | **Ex31.html** |
| **03**	| **The id Selector** | **Ex32.html** |
| **04**	| **The class Selector** | **Ex33.html** |
| **05**	| **Grouping Selectors** | **Ex34.html** |



#### 🎓 The css settings in way 2

```Ex30.html
<!DOCTYPE HTML>

<html>

    <head> 

        <meta charset="utf-8">
        
        <title> The css settings in way 2 </title>
        
        <style>

            h2 {
                color: white;
            }

            p {
                font-size: 20px;
                font-family: Verdana;
            }

            body {
                text-align: center;
                background-color: lightblue;
            }
        </style>
    </head>

    <body>

        <h2> !'M COFFEE </h2>

        <img src="./Picture/Coffee.jpg" title="The view is ......"
             alt="The photo is gone!"   width="500px" height="333px">
        
        <p> The prices in the coffee is to be determinted. </p>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex30 Results.png" alt="Ex30 Results"/>

___


#### 🎓 The element Selector


```Ex31.html
<!DOCTYPE HTML>

<html>

    <head>

        <meta charset="utf-8">

        <title> The element Selector </title>
        
        <style>

            p {
                color: blueviolet;
                font-size: 20px;
                font-weight: bold;
                text-align: center;
            }
        </style>
    </head>

    <body>

        <p> Every paragraph will be affected by the style. </p>
        
        <p id="paral"> Me too ! </p>
        <p> And Me ! </p>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex31 Results.png" alt="Ex31 Results"/>

___


#### 🎓 The id Selector
```Ex32.html
<!DOCTYPE HTML>

<html>

    <head>

        <meta charset="utf-8">

        <title> The id Selector </title>

        <style>

            p {
                font-size: 20px;
                font-weight: bold;
            }
            
            #paral {
                color: blueviolet;
                font-size: 20px;
                font-weight: bold;
                text-align: center;
            }
        </style>
    </head>

    <body>

        <p id="paral"> Hello World ! </p>

        <p> This paragraph is not affected by the style. </p>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex32 Results.png" alt="Ex32 Results"/>

___



#### 🎓 The class Selector
```Ex33.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">

        <title> The class Selector </title>

        <style>

            .center {
                color: blueviolet;
                text-align: center;
            }
        </style>
    </head>

    <body>

        <h1 class="center"> Red and center-aligned heading. </h1>
        
        <p class="center"> Red and center-aligned paragraph. </p>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex33 Results.png" alt="Ex33 Results"/>

___


#### 🎓 Grouping Selectors
```Ex34.html
<!DOCTYPE HTML>

<html>

    <head>

        <meta charset="utf-8">

        <title> Grouping Selectors </title>

        <style>

            p, h1, h2 {
                color: purple;
                text-align: center;
            }
        </style>
    </head>

    <body>

        <h1> Hello World ! </h1>
        <h2> Smaller heading ! </h2>
        <p> This is a paragraph. </p>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex34 Results.png" alt="Ex34 Results"/>

___

