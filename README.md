# Ex.05 Design a Website for Server Side Processing
## Date:02/04/2024

## AIM:
To design a website to find surface area of a Right Cylinder in server side.

## FORMULA:
Surface Area = 2Πrh + 2Πr<sup>2</sup>
<br>r --> Radius of Right Cylinder
<br>h --> Height of Right Cylinder

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create python programs for views and urls to perform server side processing.

### Step 5:
Create a HTML file to implement form based input and output.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<html>
<head>
<meta charset='utf-8'>
<meta http-equiv='X-UA-Compatible' content='IE=edge'>
<title>Surface area of Right Cylinder</title>
<meta name='viewport' content='width=device-width, initial-scale=1'>
<style type="text/css">
body {
    background-color: palevioletred;
}
.edge {
    width: 100%; /* Set width to 100% */
    display: flex;
    justify-content: center; /* Center the content horizontally */
    align-items: center; /* Center the content vertically */
    height: 100vh; /* Set height to 100% of the viewport height */
}
.box {
    border: Thick dashed pink;
    width: 500px;
    min-height: 300px;
    font-size: 20px;
    background-color: pink;
    padding: 20px; /* Add padding for better appearance */
}
.formelt {
    color: black;
    text-align: center;
    margin-top: 7px;
    margin-bottom: 6px;
}
h1 {
    color: black;
    text-align: center;
    padding-top: 20px;
}
</style>
</head>
<body>
<div class="edge">
    <div class="box">
        <h1>Surface area of Right Cylinder</h1>
        <form method="POST">
            {% csrf_token %}
            <div class="formelt">
                Radius : <input type="text" name="Radius" value="{{ r }}"></input>(in m)<br/>
            </div>
            <div class="formelt">
                Height : <input type="text" name="height" value="{{ h }}"></input>(in m)<br/>
            </div>
            <div class="formelt">
                <input type="submit" value="Calculate"></input><br/>
            </div>
            <div class="formelt">
                Area : <input type="text" name="area" value="{{ area }}"></input>m<sup>2</sup><br/>
            </div>
        </form>
    </div>
</div>
</body>
</html>
```
## SERVER SIDE PROCESSING:
![alt text](code1.png)

## HOMEPAGE:
![alt text](server.png)

## RESULT:
The program for performing server side processing is completed successfully.
