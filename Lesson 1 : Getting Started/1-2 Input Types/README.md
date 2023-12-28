# Web Development - Structure


## 🎓 Course

|      |	**Course** |	**File** |
| ---- | ---- | ---- |
| **01**	| **Basic CSS Demo** | **Ex04.html** |
| **02**	| **Basic CSS Demo** | **Ex04.html** |
| **03**	| **Basic CSS Demo** | **Ex04.html** |
| **04**	| **Basic CSS Demo** | **Ex04.html** |
| **05**	| **Basic CSS Demo** | **Ex04.html** |
| **06**	| **Basic CSS Demo** | **Ex04.html** |
| **07**	| **Basic CSS Demo** | **Ex04.html** |
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

&nbsp; <img src="./Images/Ex1 Results.png" alt="Ex1 Results"/>

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

&nbsp; <img src="./Images/Ex2 Results.png" alt="Ex1 Results"/>

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

&nbsp; <img src="./Images/Ex3 Results.png" alt="Ex1 Results"/>

___

