# Design a Website for Server Side Processing

## AIM:
To design a website to perform mathematical calculations in server side.

## DESIGN STEPS:

### Step 1:

Fork and clone the git repository.

### Step 2:

Create area.html in templates and type the required programs.

### Step 3:

Make changes in views.py , urls.py .

### Step 4:

Make migratons if you have any.

### Step 5:

Run the server.

### Step 6:

Publish the website in the given URL.

## PROGRAM :

```python
<!DOCTYPE html>
<html lang="en">
    <head>
        <style type="text/css">
        body{
            background-color: orange;
        }
        .color1{
            background-color: yellowgreen;
        }
        .color2{
            background-color: teal;
        }
        .color3{
            background-color: #FF0037;
        }
        #calculation{
            width:750px;
            height:300px;
            margin-left: auto;
            margin-right: auto;
            margin-top: 200px;
            margin-bottom: auto;
            border-width: 5px;
            border-color: yellow;
            border-style: groove;
        }
        .block{
            text-align:center;
            width:375px;
            height:40px;
            margin-top: auto;
            margin-bottom: auto;
            margin-left: auto;
            margin-right: auto;
            background-color: palegoldenrod;
        }
        </style>

    </head>
    <body>
        <div id="calculation" class="color2" align="center">
        <h1>Area of a rectangle</h1>
        <form method="POST" action="/area/">
            {%csrf_token%}
            <div class="block">
            <label for="length">Length</label>
            <input type="text" name="length" id="length" value="{{ length }}"/>
            </div>
            <div class="block">
            <label for="breadth">Breadth</label>
            <input type="text" name="breadth" id="breadth" value="{{ breadth }}"/>
            </div>
        
            <div class="block">
            <input type="submit" value="Calculate area"/>
           </div>
           <div class="block">
            <label for="area">Area</label>
            <input type="text" name="area" id="area" value="{{ area }}"/>
            </div>
        </form>
        </div>
    </body>
</html>
```
## OUTPUT:



### Home Page:
![server](https://user-images.githubusercontent.com/118541549/212706899-b24e402a-90dc-4605-b2a7-b2d4b40000b9.jpeg)


## Result:
Thus the website is created.
