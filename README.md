# Ex04 Places Around Me
## Date: 25/09/2024

## AIM
To develop a website to display details about the places around my house.

## DESIGN STEPS

### STEP 1
Create a Django admin interface.

### STEP 2
Download your city map from Google.

### STEP 3
Using ```<map>``` tag name the map.

### STEP 4
Create clickable regions in the image using ```<area>``` tag.

### STEP 5
Write HTML programs for all the regions identified.

### STEP 6
Execute the programs and publish them.

## Program
```
<!DOCTYPE html>
<html lang="en">

<head>
    {% load static %}
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body {
            margin: 0;
        }
    </style>
</head>
<body>
    <img src="{%static 'images/map.png' %}" width="800px" usemap="#map" onmousemove="coordinate(event)">
    <map name="map">
        <area shape="rect" coords="424,206,452,226" href="https://madrascoffeehouse.com/" title="MADRAS COFFEE HOUSE">
        <area shape="rect" coords="488,324,512,340" href="https://www.coffeeshastra.com/" title="COFFEE SHASTRA">
        <area shape="rect" coords="428,327,451,347" href="https://coffeeculture.co.in/" title="COFFEE CULTURE">
        <area shape="rect" coords="626,347,650,366" href="https://www.starbucks.in/dashboard" title="STARBUCKS">
        <area shape="rect" coords="368,24,396,42" href="https://www.agscinemas.com/" title="AGS CINEMAS">
    </map>
    <br>
    x-coordinate <input type="text" id="x"><br><br>
    y-coordinate <input type="text" id="y"><br>

    <script>
        function coordinate(event) {
            let x = event.clientX;
            let y = event.clientY;
            document.getElementById("x").value = x;
            document.getElementById("y").value = y;
        }
    </script>
</body>

</html>
```


## OUTPUT
![03 1](https://github.com/user-attachments/assets/733c8f2c-e2b3-472f-94c5-2e0252e57665)
![03 2](https://github.com/user-attachments/assets/1a3eb797-f931-4b15-b756-951404865710)
![03 3](https://github.com/user-attachments/assets/ba36d0bb-7205-410d-bfdd-cfed15779d85)
![03 4](https://github.com/user-attachments/assets/e7e2e04d-cb4a-40ce-b19f-808196e4d0e4)
![03 5](https://github.com/user-attachments/assets/e364e58a-ba88-4ad4-ae33-12c2a53e819c)






## RESULT
The program for implementing image maps using HTML is executed successfully.
