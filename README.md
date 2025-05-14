# Ex.08 Design of Interactive Image Gallery
## DATE:14/05/2025

## AIM
  To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS

## Step 1:

Clone the github repository and create Django admin interface

## Step 2:

Change settings.py file to allow request from all hosts.

## Step 3:

Use CSS for positioning and styling.

## Step 4:

Write JavaScript program for implementing interactivit

## Step 5:

Validate the HTML and CSS code

## Step 6:

Publish the website in the given URL.

## PROGRAM
image.html
```
<html>
<head>
    <title>Interactive Image Gallery</title>
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Anton&family=Bebas+Neue&family=Edu+AU+VIC+WA+NT+Arrows:wght@400..700&family=Josefin+Sans:ital,wght@0,100..700;1,100..700&family=Montserrat:ital,wght@0,100..900;1,100..900&family=Raleway:ital,wght@0,100..900;1,100..900&family=Shadows+Into+Light&display=swap" rel="stylesheet">
</head>
<body>
    <div class="first">
    <h1 class="heading">
        Kollywood Actors Image Gallery
    </h1>
    </div>
    <div>
        <center>
        <img src="kamal.jpg" class="img">
        <h3>Kamal Haasan</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="Rajnikanth.webp" class="img">
        <h3>Rajnikanth</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="vijayactor.webp" class="img">
        <h3>Vijay</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="ajith.webp" class="img">
        <h3>Ajith Kumar</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="surya.webp" class="img">
        <h3>Surya</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="vikram.webp" class="img">
        <h3>Vikram</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="simbu.webp" class="img">
        <h3>Silambarasan</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="dhanush.jpg" class="img">
        <h3>dhanush</h3>
        </center>
    </div>
    <div>
        <center>
            <img src="karthi.jpg" class="img">
        <h3>Karthi</h3>
        </center>
    </div>
    <div class="action">
        <img src="" alt="" class="action-image">
        <button class="btn">X</button>
    </div>
    <footer>
        Designed and Developed by Karthikeyan &reg;
    </footer>
    <script>
        const action = document.querySelector('.action');
        const actionImage = document.querySelector('.action-image');
        const closeButton = document.querySelector('.btn');
        const images = document.querySelectorAll('.img');

        images.forEach((image) => {
            image.addEventListener('click', () => {
                actionImage.src = image.src;
                action.classList.add('visible'); 
            });
        });

        closeButton.addEventListener('click', () => {
            action.classList.remove('visible'); 
        });

       action.addEventListener('click', (e) => {
            if (e.target === action) {
                action.classList.remove('visible'); 
            }
        });
    </script>
</body>
</html>
```
style.css
```
.heading{
    text-align: center;
    font-size: 30px;
    font-family: Montserrat;
    color: rgb(248, 14, 14);

}
.first {
    background-image: linear-gradient(to left,#eeaeca,);
    color:red;
    height:80px;
    width: 1461px;
    padding: 25px;
}
div{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    display: inline-block;
    margin: 25px;

}
div img{
    width: 420px;
    height: 350px;
    border:2px solid;
    border-radius: 13px;
    box-shadow: 4px 7px 7px 0px;
    margin:10px;
    transition: 400ms;

}
.img:hover {
    transform: scale(1.05); 
}

.action {
    position: fixed;
    top: 0;
    left: 0;
    width: 100vw;
    height: 100vh;
    background-color: rgba(0, 0, 0, 0.8);
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 1000;
    visibility: hidden;
    opacity: 0;
    transition: opacity 0.3s ease;
}

.action.visible {
    
    visibility: visible;
    opacity: 1;
}

.action-image {
    max-width: 90%;
    max-height: 90%;
    border-radius: 10px;
}

.btn {
    position: absolute;
    top: 10px;
    right: 10px;
    padding: 10px 20px;
    font-size: 16px;
    color: #fff;
    background: rgba(0, 0, 0, 0.5);
    border: none;
    cursor: pointer;
    border-radius: 5px;
    transition: background 0.2s ease;
}

.btn:hover {
    background: rgba(255, 255, 255, 0.2);
}
body{
    background-image:url(bg.jpg)

}
footer{
    height:55px;
    width: 1600px;background-color: rgb(90, 42, 42);
    text-align: center;
    padding-top: 30px;
    font-size: large;
    font-family: Montserrat;
    color:white ;    
}

```

## OUTPUT
![alt text](<Screenshot 2025-05-14 225645.png>)
![alt text](<Screenshot 2025-05-14 225654.png>)
![alt text](<Screenshot 2025-05-14 225702.png>)
![alt text](<Screenshot 2025-05-14 225712.png>)
## RESULT
  The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
