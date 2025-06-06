# Ex.08 Design of Interactive Image Gallery
# Date:09/05/2025
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>MUMBAI INDIANS</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #111;
      color: #fff;
    }

    h1 {
      text-align: center;
      margin: 40px 0 10px;
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 20px;
      padding: 20px;
      max-width: 1200px;
      margin: auto;
    }

    .gallery-item {
      position: relative;
      overflow: hidden;
      border-radius: 12px;
      cursor: pointer;
      box-shadow: 0 0 10px rgba(255, 255, 255, 0.1);
    }

    .gallery-item img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      transition: transform 0.4s ease;
    }

    .gallery-item:hover img {
      transform: scale(1.2);
    }

    .caption {
      position: absolute;
      bottom: 0;
      background: rgba(0, 0, 0, 0.6);
      width: 100%;
      padding: 10px;
      text-align: center;
      font-size: 14px;
    }

    .modal {
      display: none;
      position: fixed;
      inset: 0;
      background-color: rgba(0, 0, 0, 0.9);
      justify-content: center;
      align-items: center;
      z-index: 999;
    }

    .modal img {
      max-width: 90%;
      max-height: 90%;
      border: 3px solid white;
      border-radius: 10px;
    }

    .modal .close {
      position: absolute;
      top: 20px;
      right: 30px;
      font-size: 35px;
      color: #fff;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <h1>MUMBAI INDIANS</h1>

  <div class="gallery">
    <div class="gallery-item" onclick="openModal('bumara.webp')">
      <img src="bumara.webp" alt="Great Wall of China">
      <div class="caption">Great Wall of China</div>
    </div>
    <div class="gallery-item" onclick="openModal('deepak.avif')">
      <img src="deepak.avif" alt="deepak">
      <div class="caption">deepak</div>
    </div>
    <div class="gallery-item" onclick="openModal('hardhik pandya.webp')">
      <img src="hardhik pandya.webp" alt="hardhik pandya">
      <div class="caption">hardhik pandya</div>
    </div>
    <div class="gallery-item" onclick="openModal('naman dhir.jpeg')">
      <img src="naman dhir.jpeg" alt="naman dhir">
      <div class="caption">naman dhir</div>
    </div>
    <div class="gallery-item" onclick="openModal('rohit sharma.jpg')">
      <img src="rohit sharma.jpg" alt="rohit sharma">
      <div class="caption">rohit sharma</div>
    </div>
    <div class="gallery-item" onclick="openModal('surya kumar yadhav.webp')">
      <img src="surya kumar yadhav.webp" alt="surya kumar yadhav">
      <div class="caption">surya kumar yadhav</div>
    </div>
    <div class="gallery-item" onclick="openModal('thilak varma.jpg')">
      <img src="thilak varma.jpg" alt="thilak varma">
      <div class="caption">thilak varma</div>
    </div>
  </div>

  <!-- Modal -->
  <div class="modal" id="imageModal">
    <span class="close" onclick="closeModal()">&times;</span>
    <img id="modalImage" src="" alt="">
  </div>
  
  <footer>
    &copy; 2025 designed by NAKSHU[24901864]. All Rights Reserved.
</footer>
  <script>
    function openModal(src) {
      const modal = document.getElementById('imageModal');
      const modalImg = document.getElementById('modalImage');
      modalImg.src = src;
      modal.style.display = 'flex';
    }

    function closeModal() {
      const modal = document.getElementById('imageModal');
      modal.style.display = 'none';
    }
    

  </script>
</body>
</html>
```
# OUTPUT:
![alt text](<Screenshot 2025-05-11 232323.png>)
![alt text](<Screenshot 2025-05-11 232410.png>)
![alt text](<Screenshot 2025-05-11 232424.png>)
![alt text](<Screenshot 2025-05-11 232437.png>)
![alt text](<Screenshot 2025-05-11 232454.png>)
![alt text](<Screenshot 2025-05-11 232623.png>)
![alt text](<Screenshot 2025-05-11 232645.png>)
![alt text](<Screenshot 2025-05-11 232659.png>)
# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
