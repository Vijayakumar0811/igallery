# Ex.08 Design of Interactive Image Gallery
## Date:19-05-2025

NAME: VIJAYAKUMAR S

REG NO:212224040359

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
gallery.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vijay Movie Poster Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #222;
            color: white;
        }
        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
        }
        .gallery img {
            width: 200px;
            height: 300px;
            cursor: pointer;
            border: 2px solid white;
            transition: 0.3s;
        }
        .gallery img:hover {
            transform: scale(1.1);
        }
        .popup {
            display: none;
            position: fixed;
            top: 0; left: 0;
            width: 100%; height: 100%;
            background: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
        }
        .popup img {
            width: 400px;
            height: auto;
        }
        .popup span {
            position: absolute;
            top: 10px; right: 20px;
            font-size: 30px;
            cursor: pointer;
            color: white;
        }
    </style>
</head>
<body>
    <h1>Vijay Movie Poster Gallery</h1>
    <div class="gallery">
        <img src="Screenshot 2025-05-13 111155.png" alt="JANA NAYAGAN" onclick="openPopup(this.src)">
        <img src="Screenshot 2025-05-13 111456.png" alt="THE GOAT" onclick="openPopup(this.src)">
        <img src="Screenshot 2025-05-13 111655.png" alt="Leo" onclick="openPopup(this.src)">
        <img src="Screenshot 2025-05-14 132117.png" alt="Beast" onclick="openPopup(this.src)">
        <img src="Screenshot 2025-05-14 132632.png" alt="Mersal" onclick="openPopup(this.src)">
        <img src="Screenshot 2025-05-14 133200.png" alt="Jilla" onclick="openPopup(this.src)">
        <img src="IMG_20250514_133513.jpg" alt="Theri" onclick="openPopup(this.src)">
        <img src="Screenshot 2025-05-14 132339.png" alt="Kaththi" onclick="openPopup(this.src)">
        <img src="Screenshot 2025-05-14 133722.png" alt="Thalaivaa" onclick="openPopup(this.src)">
        <img src="Screenshot 2025-05-13 112946.png" alt="Master" onclick="openPopup(this.src)">
    </div>

    <div class="popup" id="popup">
        <span onclick="closePopup()">×</span>
        <img id="popupImg" src="">
    </div>

    <script>
        function openPopup(src) {
            document.getElementById('popupImg').src = src;
            document.getElementById('popup').style.display = 'flex';
        }
        function closePopup() {
            document.getElementById('popup').style.display = 'none';
        }
    </script>
</body>
</html>

```
## OUTPUT:
![image](https://github.com/user-attachments/assets/7cd71146-4eee-453e-9eac-d15c13307408)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
