# Ex.08 Design of Interactive Image Gallery
## Date:09/10/2025

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :

```
an.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> My Gallery</title>
    <link rel="stylesheet" href="hlo.css">
</head>
<body>
    <header style="text-align: center; background-color: #333; color: white; padding: 1rem 0;">
        <h1>My Gallery</h1>
    </header>
    <div style="white-space: nowrap; overflow-x: auto; padding: 1rem;">
        <div style="display: inline-block; margin-right: 10px;" onclick="openModal(this)">
            <img src="1000097967.jpg" style="height: 400px;">
        </div>
        <div style="display: inline-block; margin-right: 10px;" onclick="openModal(this)">
            <img src="dhoni.jpg" style="height: 400px;">
        </div>
        <div style="display: inline-block; margin-right: 10px;" onclick="openModal(this)">
            <img src="hardik.jpg" style="height: 400px;">
        </div>
        <div style="display: inline-block;" onclick="openModal(this)">
            <img src="kohli.jpg" style="height: 400px;">
        </div>
        <div style="display: inline-block;" onclick="openModal(this)">
            <img src="rohit.jpg" style="height: 400px;">
        </div>
    </div>
    <div id="modal" style="display: none; position: fixed; z-index: 1; left: 0; top: 0; width: 100%; height: 100%; background-color: rgba(0,0,0,0.9);">
        <span style="position: absolute; top: 15px; right: 35px; color: white; font-size: 40px; font-weight: bold; cursor: pointer;" onclick="closeModal()">&times;</span>
        <img id="modalImage" style="display: block; margin: 5% auto; max-width: 80%; height:800px;">
    </div>
    <div class="box">
        <h2>Designed By</h2>
        <h1>YASHVANDAN K | 25017523</h1>
    </div>
    <script>
        function openModal(element) {
            var modal = document.getElementById("modal");
            var modalImg = document.getElementById("modalImage");
            modal.style.display = "block";
            modalImg.src = element.querySelector("img").src;
        }
        function closeModal() {
            document.getElementById("modal").style.display = "none";
        }
    </script>
</body>
</html>

hlo.css
*{
    margin: 0;
    border:0;
}
body{
    background: linear-gradient(135deg, #00c6ff, #2a5298, #00c6ff);
    background-size: 400% 400%;
    text-align: center;
}

.box{
    position:absolute;
    color:rgb(111, 24, 75);
    left:80%;
    top:600px;
    border-radius: 10%;
    border: solid 4px black;
    padding:30px;
}
.yash{
    display: inline-block; 
    margin-right: 10px;
}

```

## OUTPUT:
![alt text](<Screenshot 2025-10-18 084132.png>)
![alt text](<Screenshot 2025-10-07 175222.png>)
![alt text](<Screenshot 2025-10-07 175242.png>)
![alt text](<Screenshot 2025-10-07 175257.png>)
![alt text](<Screenshot 2025-10-07 175344.png>)
![alt text](<Screenshot 2025-10-07 175400.png>)


## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
