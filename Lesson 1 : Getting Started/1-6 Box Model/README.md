# Web Development - Box Model

## 🎓 Course

|      |	**Course** |	**File** |
| ---- | ---- | ---- |
| **01**	| **CSS margins** | **Ex35.html** |
| **02**	| **CSS Fonts** | **Ex36.html** |
| **03**	| **Show layout without float** | **Ex37.html** |
| **04**	| **Show layout with float** | **Ex38.html** |
| **05**	| **Practise & Answers** | **Ex39.html** |



#### 🎓 CSS margins

* **All the margin properties can have the following values:**

&nbsp; &nbsp; ➤ &nbsp;  **auto - the browser calculates the margin**

&nbsp; &nbsp; ➤ &nbsp;  **Length - specifies a margin in px, pt, cm, etc.**

&nbsp; &nbsp; ➤ &nbsp;  **% - specifies a margin in % of the width of the containing element.**

&nbsp; &nbsp; ➤ &nbsp;  **inherit - specifies that the margin should be inherited from the parent element.**


```Ex35.html
<!DOCTYPE HTML>

<html>

    <head>

        <meta charset="utf-8">

        <title> CSS Margins </title>

        <style>

            div {
                margin-top:  100px;
                margin-left: 80px;
                margin-right: 150px;
                margin-bottom: 100px;

                border: 1px solid black;
                background-color: lightblue ;
            }
        </style>
    </head>

    <body>

        <h2> HTML Is Dept </h2>

        <div>
            This div element has 
            a top margin of 100px.
            a right margin of 150px.
            a bottom margin of 100px.
            and a left margin of 80px.
        </div>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex35 Results.png" alt="Ex35 Results"/>

___

#### 🎓 CSS Fonts

* **Font Family: The font family of a text is 
   set with the fontfamily property.**

* **The font-family property should hold several 
   font names as a “fallback” system. 
   If the browser does not support the first font, 
   it tries the next font, and so on.**

* **Note: If the name of a font family is more 
  than one word, it must be in quotation marks, 
  like: "Times New Roman".**

* **More than one font family is specified in 
  a commaseparated list：**


```Ex36.html
<!DOCTYPE HTML>

<html>

    <head>

        <meta charset="utf-8">

        <title> CSS Fonts </title>

        <style>

            h2.serif {
                font-family: 'Times New Roman', Times, serif;
            }

            ul.sansserif {
                font-family: Arial, Helvetica, sans-serif;
            }
        </style>
    </head>

    <body>

        <h2 class="serif"> Unordered List with Circle Bullets </h2>
        
        <ul style="list-style-type: lower-alpha;" class="sansserif">
            
            <li> Tea    </li>
            <li> Milk   </li>
            <li> Coffee </li>
        </ul>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex36 Results.png" alt="Ex36 Results"/>

___

#### 🎓 Show layout without float

```Ex37.html
<!DOCTYPE HTML>

<html>

    <head>

        <meta charset="utf-8">

        <title> Show layout without float </title>
        
        <style>

            #side {
                text-align: center;
                background-color: lightblue;
            }

            #main {
                text-align: center;
                background-color: lightgreen;
            }

            #header {
                text-align: center;
                background-color: lightgray;
            }

            #footer {
                text-align: center;
                background-color: yellow;
            }
        </style>
    </head>

    <body>

        <div id="header"> Header ID </div>
        <div id="side">   Side ID   </div>
        <div id="main">   Main ID   </div>
        <div id="footer"> Footer ID </div>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex37 Results.png" alt="Ex37 Results"/>

___

#### 🎓 Show layout with float

```Ex38.html
<!DOCTYPE HTML>

<html>

    <head>

        <meta charset="utf-8">

        <title> Show layout without float </title>
        
        <style>

            #side {
                float: left;
                width: 100px;
                background-color: lightblue;
            }

            #main {
                float: left;
                width: 100px;
                background-color: lightgreen;
            }

            #header {
                float: left;
                width: 100px;
                background-color: lightgray;
            }

            #footer {
                float: left;
                width: 100px;
                background-color: yellow;
            }
        </style>
    </head>

    <body>

        <div id="header"> Header ID </div>
        <div id="side">   Side ID   </div>
        <div id="main">   Main ID   </div>
        <div id="footer"> Footer ID </div>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex38 Results.png" alt="Ex38 Results"/>

___

#### 🎓 Practise & Answers

```Ex39.html
<!DOCTYPE HTML>

<html>

    <head>

        <meta charset="utf-8">

        <title> Exercise / Answer </title>
        
        <style>

            #side {
                float: left;
                width: 100px;
                height: 20px;
                background-color: lightblue;
            }

            #main {
                float: left;
                width: 100px;
                height: 20px;
                background-color: lightgreen;
            }

            #header {
                float: inherit;
                width: 500px;
                height:100px;
                background-color: lightcoral;
            }

            #footer {
                float: inherit;
                width: 500px;
                height:100px;
                background-color: lightgray;
            }
        </style>
    </head>

    <body>

        <div id="header"> Header ID </div>
        <div id="side">   Side ID   </div>
        <div id="main">   Main ID   </div>
        <div id="footer"> Footer ID </div>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex39 Results.png" alt="Ex39 Results"/>

___

