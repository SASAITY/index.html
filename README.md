# index.html
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Мантра Йога с Адираса Прабху</title>
  <link href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Manrope', sans-serif;
      background: url('https://i.ibb.co/xzNf6cs/mandala-bg.png') no-repeat center center fixed;
      background-size: cover;
      color: white;
      text-align: center;
    }

    .overlay {
      background: rgba(0, 0, 0, 0.7);
      padding: 60px 20px;
      min-height: 100vh;
    }

    h1 {
      font-size: 48px;
      color: #ff9900;
      margin-bottom: 10px;
    }

    h2 {
      font-size: 26px;
      color: #ffcc66;
      margin-top: 0;
    }

    .event-info {
      margin-top: 30px;
      font-size: 18px;
      line-height: 1.6;
    }

    .photo {
      margin-top: 30px;
    }

    .photo img {
      max-width: 280px;
      border-radius: 10px;
      border: 4px solid #ff9900;
    }

    .btn {
      margin-top: 40px;
      background-color: #ff9900;
      color: white;
      padding: 14px 28px;
      border: none;
      border-radius: 30px;
      font-size: 18px;
      cursor: pointer;
      transition: background 0.3s ease;
    }

    .btn:hover {
      background-color: #e07b00;
    }

    .popup {
      display: none;
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: rgba(0, 0, 0, 0.8);
      align-items: center;
      justify-content: center;
      z-index: 999;
    }

    .popup-content {
      background: #fff;
      color: #333;
      padding: 30px;
      border-radius: 12px;
      text-align: center;
      width: 90%;
      max-width: 400px;
    }

    .popup-content a {
      color: #0077cc;
      font-weight: bold;
      text-decoration: none;
      font-size: 18px;
    }

    .popup-content a:hover {
      text-decoration: underline;
    }

    .close {
      margin-top: 20px;
      cursor: pointer;
      color: #ff0000;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <div class="overlay">
    <h1>МАНТРА ЙОГА</h1>
    <h2>с Адираса Прабху</h2>

    <div class="photo">
      <img src="https://i.ibb.co/JpKzNK5/adirasa.jpg" alt="Адираса Прабху">
    </div>

    <div class="event-info">
      <p>📍 Чайковского 82, Батуми</p>
      <p>🗓 25 июня в 17:00</p>
      <p>🌟 Медитативный транс, экстатическое блаженство, сладости и угощения</p>
      <p><strong>Места ограничены — бронируй заранее!</strong></p>
    </div>

    <button class="btn" onclick="openPopup()">Забронировать место</button>
  </div>

  <div class="popup" id="popup">
    <div class="popup-content">
      <p>Напиши нам в Telegram для брони:</p>
      <a href="https://t.me/Aravinda108" target="_blank">@Aravinda108</a>
      <div class="close" onclick="closePopup()">Закрыть</div>
    </div>
  </div>

  <script>
    function openPopup() {
      document.getElementById("popup").style.display = "flex";
    }

    function closePopup() {
      document.getElementById("popup").style.display = "none";
    }
  </script>
</body>
</html>
