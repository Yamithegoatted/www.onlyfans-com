<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>OnlyFans</title>
  <style>
    body {
      background-color: white;
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
      font-family: Arial, sans-serif;
    }
    #loading {
      font-size: 2em;
      color: #0d0d0d;
    }
    #jumpscare {
      display: none;
      position: absolute;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      background: black;
      justify-content: center;
      align-items: center;
      z-index: 9999;
    }
    #jumpscare img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  </style>
</head>
<body>
  <div id="loading">Loading OnlyFans...</div>
  <div id="jumpscare">
    <img src="https://example.com/scary-image.jpg" alt="Jumpscare">
    <audio autoplay>
      <source src="https://example.com/scream.mp3" type="audio/mpeg">
    </audio>
  </div>

  <script>
    setTimeout(() => {
      document.getElementById('loading').style.display = 'none';
      document.getElementById('jumpscare').style.display = 'flex';
    }, 3000); // 3 seconds delay
  </script>
</body>
</html>
