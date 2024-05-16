# Ex04 Places Around Me
## Date: 16-05-24

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

## CODE
<!DOCTYPE html>
<html lang="en">
<head>
</head>
<script>
    function coord(event) {
        let x=event.clientX;
        let y=event.clientY;
        document.getElementById("txt1").value=x;
        document.getElementById("txt2").value=y;
    }
</script>
<body>
    <img src="ex-04.png" width="1000px" usemap="#MapNew" onmousemove="coord(event)">
    <MAP name="MapNew">
        <AREA shape="RECT" coords="599,606,620,374" href="https://www.madhaengineeringcollege.com/" Title="madha engineering college" >
        <AREA shape="RECT" coords="612,298,617,296" href="https://saintthomascollege.com/" Title="st thomas college of engineering" >
        <AREA shape="RECT" coords="600,376,609,375" href="https://npsbcet.edu.in/" Title="new  shri bhavani college" >
    </MAP> <br>
    X coord:<input type="text" name="" id="txt1"> <br>
    Y coord:<input type="text" name="" id="txt2"> 

</body>
</html>


## OUTPUT
![alt text](<ex -04 output.png>)






## RESULT
The program for implementing image maps using HTML is executed successfully.
