# Web Development - Form


## 🎓 Course

|      |	**Course** |	**File** |
| ---- | ---- | ---- |
| **01**	| **table** | **Ex22.html** |
| **02**	| **Adding a Border - 1** | **Ex23.html** |
| **03**	| **Adding a Border - 2** | **Ex24.html** |
| **04**	| **Adding a Border - 3** | **Ex25.html** |
| **05**	| **Adding a Border - 4** | **Ex26.html** |
| **06**	| **Adding a Caption** | **Ex27.html** |
| **07**	| **Use table name & background color** | **Ex28.html** |
| **08**	| **Different colors** | **Ex29.html** |


#### 🎓 `<table>`

```Ex22.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Basic HTML table </title>
        
        <style>
            
            table {
                width: 100%; 
                color: brown; 
                font-size: 20px;
                font-weight: bold;
            }
            
            .title {
                color: black; 
                font-size: 25px;
                font-weight: bold;
            }
        </style>
    </head>
    
    <body>
    
        <table>
        
            <tr class="title">
                
                <th> First Name </th>
                <th> Last  Name </th>
                <th> Age </th>
            </tr>
            
            <tr>
                
                <td> Jill  </td>
                <td> Smith </td>
                <td> 50    </td>
            </tr>
            
            <tr>
                
                <td> Eva     </td>
                <td> Jackson </td>
                <td> 94      </td>
            </tr>
            
            <tr>
                
                <td> John </td>
                <td> Doe  </td>
                <td> 50   </td>
            </tr>
        </table>
    </body>
</html>
```


#### ➤ Result

&nbsp; <img src="./Images/Ex22 Results.png" alt="Ex22 Results"/>

___


#### 🎓 Adding a Border - 1

```Ex23.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Basic HTML table </title>
        
        <style>
            
            td {
                border: 1px solid black;
            }
            
            th, table {
                border: 5px solid black;
            } 
            
            table {
                width: 100%; 
                color: brown; 
                font-size: 20px;
                font-weight: bold;
            }
            
            .title {
                color: black; 
                font-size: 25px;
                font-weight: bold;
            }
        </style>
    </head>
    
    <body>
    
        <table>
        
            <tr class="title">
                
                <th> First Name </th>
                <th> Last  Name </th>
                <th> Age </th>
            </tr>
            
            <tr>
                
                <td> Jill  </td>
                <td> Smith </td>
                <td> 50    </td>
            </tr>
            
            <tr>
                
                <td> Eva     </td>
                <td> Jackson </td>
                <td> 94      </td>
            </tr>
            
            <tr>
                
                <td> John </td>
                <td> Doe  </td>
                <td> 50   </td>
            </tr>
        </table>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex23 Results.png" alt="Ex23 Results"/>

___


#### 🎓 Adding a Border - 2

```Ex24.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Basic HTML table </title>
        
        <style>
            
            td, th {
                text-align: right;
            }
            
            td, th, table {
                border: 1px solid black;
                border-collapse: collapse ;
            } 
            
            table {
                width: 100%; 
                color: brown; 
                font-size: 20px;
                font-weight: bold;
            }
            
            .title {
                color: black; 
                font-size: 25px;
                font-weight: bold;
            }
        </style>
    </head>
    
    <body>
    
        <table>
        
            <tr class="title">
                
                <th> First Name </th>
                <th> Last  Name </th>
                <th> Age </th>
            </tr>
            
            <tr>
                
                <td> Jill  </td>
                <td> Smith </td>
                <td> 50    </td>
            </tr>
            
            <tr>
                
                <td> Eva     </td>
                <td> Jackson </td>
                <td> 94      </td>
            </tr>
            
            <tr>
                
                <td> John </td>
                <td> Doe  </td>
                <td> 50   </td>
            </tr>
        </table>
    </body>
</html>
```
#### ➤ Result

&nbsp; <img src="./Images/Ex24 Results.png" alt="Ex24 Results"/>

___


#### 🎓 Adding a Border - 3

```Ex25.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Basic HTML table </title>
        
        <style>
            
            td, th {
                text-align: center;
            }
            
            td, th, table {
                border: 1px solid black;
                border-collapse: collapse ;
            } 
            
            table {
                width: 100%; 
                color: brown; 
                font-size: 20px;
                font-weight: bold;
            }
            
            .title {
                color: black; 
                font-size: 25px;
                font-weight: bold;
            }
        </style>
    </head>
    
    <body>
    
        <table>
        
            <tr class="title">
                
                <th> First Name </th>
                <th colspan="2"> Last  Name / Age </th>
            </tr>
            
            <tr>
                
                <td> Jill  </td>
                <td> Smith </td>
                <td> 50    </td>
            </tr>
            
            <tr>
                
                <td> Eva     </td>
                <td> Jackson </td>
                <td> 94      </td>
            </tr>
            
            <tr>
                
                <td> John </td>
                <td> Doe  </td>
                <td> 50   </td>
            </tr>
        </table>
    </body>
</html> 
```
#### ➤ Result

&nbsp; <img src="./Images/Ex25 Results.png" alt="Ex25 Results"/>

___


#### 🎓 Adding a Border - 4
```Ex26.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Basic HTML table </title>
        
        <style>
            
            td, th {
                text-align: center;
            }
            
            td, th, table {
                border: 1px solid black;
                border-collapse: collapse ;
            } 
            
            table {
                width: 100%; 
                color: brown; 
                font-size: 20px;
                font-weight: bold;
            }
            
            .title {
                color: black; 
                font-size: 25px;
                font-weight: bold;
            }
        </style>
    </head>
    
    <body>
    
        <table>
        
            <tr class="title">
                
                <th> First Name </th>
                <th colspan="2"> Last  Name / Age </th>
            </tr>
            
            <tr>
                
                <td> Jill  </td>
                <td> Smith </td>
                <td> 50    </td>
            </tr>
            
            <tr>
                
                <td rowspan="2"> Eva     </td>
                <td> Jackson </td>
                <td> 94      </td>
            </tr>
            
            <tr>
                
                <td> Doe  </td>
                <td> 50   </td>
            </tr>
        </table>
    </body>
</html> 
```
#### ➤ Result

&nbsp; <img src="./Images/Ex26 Results.png" alt="Ex26 Results"/>

___


#### 🎓 Adding a Caption
```Ex27.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Basic HTML table </title>
        
        <style>
            
            td, th {
                text-align: center;
            }
            
            td, th, table {
                border: 1px solid black;
                border-collapse: collapse ;
            } 
            
            table {
                width: 100%; 
                color: brown; 
                font-size: 20px;
                font-weight: bold;
            }
            
            .title {
                color: black; 
                font-size: 25px;
                font-weight: bold;
            }
        </style>
    </head>
    
    <body>
    
        <table>

            <caption> My Friends </caption>
        
            <tr class="title">
                
                <th> First Name </th>
                <th colspan="2"> Last  Name / Age </th>
            </tr>
            
            <tr>
                
                <td> Jill  </td>
                <td> Smith </td>
                <td> 50    </td>
            </tr>
            
            <tr>
                
                <td> Eva     </td>
                <td> Jackson </td>
                <td> 94      </td>
            </tr>
            
            <tr>
                
                <td> John </td>
                <td> Doe  </td>
                <td> 50   </td>
            </tr>
        </table>
    </body>
</html> 
```
#### ➤ Result

&nbsp; <img src="./Images/Ex27 Results.png" alt="Ex27 Results"/>

___


#### 🎓 Use table name & background color

```Ex28.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Basic HTML table </title>
        
        <style>
            
            td, th {
                text-align: center;
            }
            
            td, th, table {
                border: 1px solid black;
                border-collapse: collapse ;
            } 
            
            table {
                width: 100%; 
                color: brown; 
                font-size: 20px;
                font-weight: bold;
                background-color: lightblue;
            }
            
            .title {
                color: black; 
                font-size: 25px;
                font-weight: bold;
            }
        </style>
    </head>
    
    <body>
    
        <table>

            <caption> My Friends </caption>
        
            <tr class="title">
                
                <th> First Name </th>
                <th colspan="2"> Last  Name / Age </th>
            </tr>
            
            <tr>
                
                <td> Jill  </td>
                <td> Smith </td>
                <td> 50    </td>
            </tr>
            
            <tr>
                
                <td> Eva     </td>
                <td> Jackson </td>
                <td> 94      </td>
            </tr>
            
            <tr>
                
                <td> John </td>
                <td> Doe  </td>
                <td> 50   </td>
            </tr>
        </table>
    </body>
</html> 
```
#### ➤ Result

&nbsp; <img src="./Images/Ex28 Results.png" alt="Ex28 Results"/>

___



#### 🎓 Different colors
```Ex29.html
<!DOCTYPE HTML>

<html>

    <head>
        
        <meta charset="utf-8">
        
        <title> Basic HTML table </title>
        
        <style>
            
            td, th {
                text-align: center;
            }
            
            td, th, table {
                border: 1px solid black;
                border-collapse: collapse ;
            } 
            
            table {
                width: 100%; 
                color: brown; 
                font-size: 20px;
                font-weight: bold;
            }
            
            .title {
                color: black; 
                font-size: 25px;
                font-weight: bold;
                background-color: lightblue;
            }
        </style>
    </head>
    
    <body>
    
        <table>

            <caption> My Friends </caption>
        
            <tr class="title">
                
                <th> First Name </th>
                <th colspan="2"> Last  Name / Age </th>
            </tr>
            
            <tr style="background-color: yellow;">
                
                <td> Jill  </td>
                <td> Smith </td>
                <td> 50    </td>
            </tr>
            
            <tr style="background-color: yellow;">
                
                <td> Eva     </td>
                <td> Jackson </td>
                <td> 94      </td>
            </tr>
            
            <tr style="background-color: yellow;">
                
                <td> John </td>
                <td> Doe  </td>
                <td> 50   </td>
            </tr>
        </table>
    </body>
</html> 
```
#### ➤ Result

&nbsp; <img src="./Images/Ex29 Results.png" alt="Ex29 Results"/>

___
