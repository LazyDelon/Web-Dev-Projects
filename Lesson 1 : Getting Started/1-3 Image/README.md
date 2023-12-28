# Web Development - Image


## 🎓 Course

|      |	**Course** |	**File** |
| ---- | ---- | ---- |
| **01**	| **Img** | **Ex19.html** |
| **02**	| **Image Size** | **Ex20.html** |
| **03**	| **Image Maps** | **Ex21.html** |




#### 🎓 `<img>`

```Ex19.html
<!DOCTYPE HTML>

<html>

    <head>
    
        <meta charset="utf-8">
        
        <title> Totoro </title>
    </head>
    
    <body>
        
        <h2> 
            &ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;
            &ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;
            
            HTML Image 
        </h2>
        
        <img src="Picture/Totoro_BG.jpg" title="Totoro Image"
             alt="The photo is gone!"  width="500" height="200">
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex19 Results.png" alt="Ex19 Results"/>

___


#### 🎓 Image Size

```Ex20.html
<!DOCTYPE HTML>

<html>

    <head>
    
        <meta charset="utf-8">
        
        <title> Image Maps </title>
        
        <style>
            
            .y {
                outline-color: yellow;
            }
            
            .g {
                outline-color: green;
            }
            
            .b {
                outline-color: blue;
            }
        </style>
    </head>
    
    <body>
    
        <h2> Image Maps </h2>
        
        <p>
            Click on the Phone, the Computer, the cup of Coffee
            to go to a new page and read more about the topic：
        </p>
        
        <img src="Picture/Computer.png" alt="Workplace"
             usemap="#workmap" width="400" height="350">
         
        <map name="workmap">
            
            <area class="y" shape="rect" coords="32, 40, 275, 325" href="Other/Computer.html">
            <area class="g" shape="rect" coords="290, 160, 335, 230" href="Other/Computer.html">
            <area class="b" shape="circle" coords="340, 280, 45" href="Other/Coffee.html">
        </map>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex20 Results.png" alt="Ex20 Results"/>

___


#### 🎓 Image Maps
```Ex21.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Background Image </title>
        
        <style>
            
            body {
                background-size: 250px;
            }
        </style>
    </head>

    <body style="background-image: url(Picture/Totoro.jpg);">
        
        
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex21 Results.png" alt="Ex21 Results"/>

___

