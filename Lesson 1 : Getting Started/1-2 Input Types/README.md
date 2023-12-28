# Web Development - Input Types


## 🎓 Course

|      |	**Course** |	**File** |
| ---- | ---- | ---- |
| **01**	| **HTML Forms** | **Ex04.html** |
| **02**	| **The select Element** | **Ex05.html** |
| **03**	| **Visible Values** | **Ex06.html** |
| **04**	| **Radio Button** | **Ex07.html** |
| **05**	| **Alert Action** | **Ex08.html** |
| **06**	| **Date type** | **Ex09.html** |
| **07**	| **Range** | **Ex10.html** |
| **08**	| **DataList Element** | **Ex11.html** |
| **09**	| **input + output Element** | **Ex12.html** |
| **10**	| **Attribute：readonly** | **Ex13.html** |
| **11**	| **Attribute：disabled** | **Ex14.html** |
| **12**	| **Attribute：height & width** | **Ex15.html** |
| **13**	| **Attribute：min & max** | **Ex16.html** |
| **14**	| **Attribute：multiple** | **Ex17.html** |
| **15**	| **Attribute：pattern** | **Ex18.html** |




#### 🎓 HTML Forms

```Ex04.html
<!DOCTYPE HTML>

<html>

    <head> 
        
        <meta charset="utf-8">
        
        <title> Form-Data </title>
    </head>
    
    <body>
        
        <h2> HTML Forms </h2>
        
        <form action="/action_page.php">
        
            First Name： <br>
            <input type="text" name="First Name" value="Mickey"> <br>
            
            Last Name： <br>
            <input type="text" name="Last Name" value="Mouse"> <br><br>
            
            <input type="submit" value="Submit">
        </form>
        
        <p>
            If you click the "Submit" Button, 
            the form-data will be sent to a page called "/action_page.php".
        </p>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex04 Results.png" alt="Ex04 Results"/>

___


#### 🎓 The `<select>` Element

```Ex05.html
<!DOCTYPE HTML>

<html>

    <head> 
        
        <meta charset="utf-8">
        
        <title> Select Element </title>
    </head>
    
    <body>
    
        <h2> The select Element </h2>
        
        <form action="/action_page.php">
            
            <select name="cars">
            
                <option value="car1"> BMW   </option>
                <option value="car2"> Audi  </option>
                <option value="car3"> Benz  </option>
                <option value="car4"> Honda </option>
            </select>
            
            <br><br>
            
            <input type="submit" value="Submit">
        </form>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex05 Results.png" alt="Ex05 Results"/>

___


#### 🎓 Visible Values

```Ex06.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Drop-Down List </title>
    </head>

    <body>
        
        <h2> The select Element </h2>
        
        <p> The select element defines a drop-down list： </p>
        
        <form action="/action_page.php">
            
            <select name="cars" size="3">
                
                <option value="car1"> BMW   </option>
                <option value="car2"> Audi  </option>
                <option value="car3"> Benz  </option>
                <option value="car4" selected> Honda </option>
            </select>
            
            <br><br>
            
            <input type="submit" value="Submit">
        </form>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex06 Results.png" alt="Ex06 Results"/>

___


#### 🎓 Radio Button

```Ex07.html
<!DOCTYPE HTML>

<html>
    
    <head>
        
        <meta charset="utf-8">
        
        <title> My HTML5 Experiment </title>
        <link rel="stylesheet" href="Ex07.css">
    </head>
    
    <body>
        
        <h2> HTML Forms </h2>
        
        <form action="/action_page.php">
            
            First Name： <input type="text" name="FirstName" value="Mickey"> <br>
            Last Name：  <input type="text" name="LastName" value="Mouse">   <br>
            Your Student ID： <input type="text" name="ID" value="4080E007"> <br>
            
            <h2> Radio Button </h2>
            
            <input type="radio" name="dept" value="IS department"> IS department <br>
            <input type="radio" name="dept" value="IM department"> IM department <br>
            <input type="radio" name="dept" value="IC department"> IC department <br><br>
            
            <input type="submit" value="Submit">
        </form>
        
        <p>
            If you click the "Submit" Button, the form-data
            will be sent to a page called "/action_page.php".
        </p>
    </body>
</html>
```

```Ex07.css
p {
    color: blue;
}

input {
    color: blue;
    background-color: orange;
}
```
#### ➤ Result

&nbsp; <img src="./Images/Ex07 Results.png" alt="Ex07 Results"/>

___

#### 🎓 Alert Action

```Ex08.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Alert action </title>
    </head>

    <body>
    
        <h2> The Select Element </h2>
        
        <p> The select element defines a drop-down list： </p>
        
        <form action="/action_page.php">
        
            <select name="cars" size="3">
                
                <option value="car1"> BMW   </option>
                <option value="car2"> Audi  </option>
                <option value="car3"> Benz  </option>
                <option value="car4"> Honda </option>
                <option value="car5"> Mazda </option>
            </select>
            
            <br><br>
            
            <input type="button" onclick="alert('Hello HTML5!')" value="Click Me!">
        </form>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex08 Results.png" alt="Ex08 Results"/>

___

#### 🎓 Date type 

```Ex09.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Date Type </title>
    </head> 
    
    <body>
        
        <h2> The Select Element </h2>
        
        <p> The select element defines a drop-down list： </p>
        
        <form action="/action_page.php">
        
            <select name="cars" size="3">
            
                <option value="car1"> BMW   </option>
                <option value="car2"> Audi  </option>
                <option value="car3"> Benz  </option>
                <option value="car4"> Honda </option>
                <option value="car5"> Mazda </option>
            </select>
            
            <br><br>
            
            <h2> Date Field </h2>
            
            <input type="date" name="bday">
            <input type="button" onclick="alert('Hello HTML5!')" value="Click Me!">
        </form>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex09 Results.png" alt="Ex09 Results"/>

___

#### 🎓 Range

```Ex10.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Range </title>
    </head> 
    
    <body>
        
        <h2> The Select Element </h2>
        
        <p> The select element defines a drop-down list： </p>
        
        <form action="/action_page.php">
        
            <select name="cars" size="3">
            
                <option value="car1"> BMW   </option>
                <option value="car2"> Audi  </option>
                <option value="car3"> Benz  </option>
                <option value="car4"> Honda </option>
                <option value="car5"> Mazda </option>
            </select>
            
            <br><br>
            
            <h2> Range Field </h2>
            
            <input type="range" name="points" min="0" max="100"> <br>
            <input type="submit" value="Submit">
        </form>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex10 Results.png" alt="Ex10 Results"/>

___

#### 🎓 `<DataList>` Element

```Ex11.html
<!DOCTYPE HTML>

<html>
    
    <head>
        
        <meta charset="utf-8">
        
        <title> DataList Element </title>
    </head>

    <body>
        
        <h2> The DataList Element </h2>
        
        <p>
            The datalist element specifies a list of pre-defined options 
            for an input element：
        </p>
        
        <form action="/action_page.php">
            
            <input list="browsers" name="browser">
            
            <datalist id="browsers">
                
                <option value="Opera">
                <option value="Chrome">
                <option value="Safari">
                <option value="Firefox">
                <option value="Internet Explorer">
            </datalist>
            
            <br><br>
            
            <input type="submit">
        </form>
        
        <p> <b>Note</b> The datalist tag is not supported in Safari or IE9. </p>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex11 Results.png" alt="Ex11 Results"/>

___

#### 🎓 `<input>` + `<output>` Element

```Ex12.html
<!DOCTYPE HTML>

<html>

    <head> 
        
        <meta charset="utf-8">
        
        <title> input + output </title>
    </head>
    
    <body>
        
        <h2> The Output Element </h2>
        
        <p>
            The output element represents the result of a calculation.
        </p>
        
        <form action="/action_page.php"
              oninput="y.value = parseInt(a.value) + parseInt(b.value)">

            0 <input type="range" id="a" name="a" value="50" oninput="myFunction()"> 100 
            
            <br><br> ➜ <nobr id="range"> </nobr> &ensp;
            
            + &ensp; <input type="number" id="b" value="50"> &ensp; =
            
            <output name="y" for="range b"> </output> <br>
        </form>
        
        <script>
            function myFunction() {

                var x = document.getElementById("a").value;
                document.getElementById("range").innerHTML = x;
            }
        </script> 
        
      
        <p> <strong>Note</strong> The output element. </p>
    </body>
    
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex12 Results.png" alt="Ex12 Results"/>

___

#### 🎓 Attribute：readonly

```Ex13.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Attribute：readonly </title>
    </head>

    <body>
        
        <h2> The readonly Attribute </h2>
        
        <p>
            The readonly attribute specifies that the
            input filed is read only (cannot be changed)：
        </p>
        
        <form action="/action_page.php">
        
            First Name： <br>
            <input type="text" name="FirstName" value="John" readonly> <br>
            
            Last Name： <br>
            <input type="text" name="LastName"> <br><br>
            
            <input type="submit" value="Submit">
        </form>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex13 Results.png" alt="Ex13 Results"/>

___

#### 🎓 Attribute：disabled

```Ex14.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Attribute：disabled </title>
    </head>

    <body>
        
        <h2> The disabled Attribute </h2>
        
        <p>
            The disabled attribute specifies that the input filed is disabled：
        </p>
        
        <form action="/action_page.php">
        
            First Name： <br>
            <input type="text" name="FirstName" value="John" disabled> <br>
            
            Last Name： <br>
            <input type="text" name="LastName"> <br><br>
            
            <input type="submit" value="Submit">
        </form>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex14 Results.png" alt="Ex14 Results"/>

___

#### 🎓 Attribute：height & width

```Ex15.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Attribute：height & width </title>
    </head>
    
    <body>
        
        <h2> The height and width Attributes </h2>
        
        <p>
            The height and width attribute specify the
            height and width of an input type="image" element.
        </p>
        
        <form action="/action_page.php">
            
            First Name： <br>
            <input type="text" name="FirstName"> <br><br>
            
            Last Name：  <br>
            <input type="text" name="LastName"> <br>
            
            <input type="image" src="Picture/submit.png" alt="Submit" width="100" height="90">
        </form>
        
        <p>
            <b> Note： </b>
            
            The input type="image" sends the X and Y 
            coordinates of the click that activated the image button.
        </p>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex15 Results.png" alt="Ex15 Results"/>

___

#### 🎓 Attribute：min & max

```Ex16.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Attributes：min & max </title>
    </head>
    
    <body>
        
        <h2> The min and max Attributes </h2>
        
        <p>
            The min and max attribute specify the 
            minuimum and maximum values for an input element.
        </p>
    
        <form action="/action_page.php">
            
            Enter a date before 1980-01-01：
            <input type="date" name="bday" max="1979-12-31"> 
            
            &ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;
            
            Enter a date after 2000-01-01：
            <input type="date" name="bday" min="2000-01-02"> 
            
            <br><br><br><br><br><br><br><br><br><br>
            <br><br><br><br><br><br><br><br><br><br>
            
            Quantity (Between 1 to 5)：
            <input type="number" name="Quantity" min="1" max="5">
            
            <input type="submit">
        </form>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex16 Results.png" alt="Ex16 Results"/>

___

#### 🎓 Attribute：multiple

```Ex17.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Attribute：multiple </title>
    </head>

    <body>
        
        <h2> The multiple Attributes </h2>
        
        <p>
            The multiple attribute specifies that the 
            user is allowed to enter more than one value in the input element.
        </p>
        
        <form action="/action_page.php">
            
            Select Images：<input type="file" name="img" multiple>
            
            <input type="submit">
        </form>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex17 Results.png" alt="Ex17 Results"/>

___

#### 🎓 Attribute：pattern

```Ex18.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Attribute：pattern </title>
    </head>
    
    <body>
        
        <h2> The pattern Attributes </h2>
        
        <p>
            The pattern attribute specifies a regular expression
            that the input element's value is checked against.
        </p>
        
        <form action="/action_page.php"> 
            
            Country Code： 
            <input type="text" name="Country_Code" pattern="[A-Za-z]{3}"
                   title="Three letter country code">
            
            <input type="submit">
        </form>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex18 Results.png" alt="Ex18 Results"/>

___
