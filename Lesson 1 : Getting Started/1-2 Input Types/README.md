# Web Development - Structure


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
| **08**	| **Basic CSS Demo** | **Ex04.html** |
| **09**	| **Basic CSS Demo** | **Ex04.html** |
| **10**	| **Basic CSS Demo** | **Ex04.html** |
| **11**	| **Basic CSS Demo** | **Ex04.html** |
| **12**	| **Basic CSS Demo** | **Ex04.html** |




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

#### 🎓 xxxx

```Ex11.html

```
#### ➤ Result

&nbsp; <img src="./Images/Ex11 Results.png" alt="Ex11 Results"/>

___

#### 🎓 xxxx

```Ex12.html

```
#### ➤ Result

&nbsp; <img src="./Images/Ex12 Results.png" alt="Ex12 Results"/>

___

#### 🎓 xxxx

```Ex13.html

```
#### ➤ Result

&nbsp; <img src="./Images/Ex13 Results.png" alt="Ex13 Results"/>

___

#### 🎓 xxxx

```Ex14.html

```
#### ➤ Result

&nbsp; <img src="./Images/Ex14 Results.png" alt="Ex14 Results"/>

___

#### 🎓 xxxx

```Ex15.html

```
#### ➤ Result

&nbsp; <img src="./Images/Ex15 Results.png" alt="Ex15 Results"/>

___

#### 🎓 xxxx

```Ex16.html

```
#### ➤ Result

&nbsp; <img src="./Images/Ex16 Results.png" alt="Ex16 Results"/>

___

#### 🎓 xxxx

```Ex17.html

```
#### ➤ Result

&nbsp; <img src="./Images/Ex17 Results.png" alt="Ex17 Results"/>

___

#### 🎓 xxxx

```Ex18.html

```
#### ➤ Result

&nbsp; <img src="./Images/Ex18 Results.png" alt="Ex18 Results"/>

___
