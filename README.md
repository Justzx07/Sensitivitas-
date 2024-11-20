<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Aimlock V5 Panel</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background: linear-gradient(135deg, #f0f4ff, #dfe8fc);
    }
    .container {
      width: 300px;
      padding: 20px;
      background: #fff;
      border-radius: 15px;
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
      text-align: center;
    }
    .container h1 {
      font-size: 24px;
      margin: 0;
      color: #333;
    }
    .container p {
      font-size: 14px;
      color: #888;
      margin-bottom: 20px;
    }
    .toggle-group {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 15px;
      padding: 10px;
      border-radius: 10px;
      background: #f8f9fc;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }
    .toggle-group label {
      display: flex;
      align-items: center;
      font-size: 14px;
      color: #555;
      gap: 10px;
    }
    .toggle-group label i {
      font-size: 18px;
      color: #888;
    }
    .toggle-switch {
      position: relative;
      width: 40px;
      height: 20px;
      background: #ccc;
      border-radius: 10px;
      cursor: pointer;
      transition: background 0.3s;
    }
    .toggle-switch::before {
      content: '';
      position: absolute;
      width: 16px;
      height: 16px;
      background: #fff;
      border-radius: 50%;
      top: 2px;
      left: 2px;
      transition: transform 0.3s;
    }
    .toggle-switch.active {
      background: #4caf50;
    }
    .toggle-switch.active::before {
      transform: translateX(20px);
    }
    .footer {
      margin-top: 20px;
      font-size: 12px;
      color: #aaa;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>AIMLOCK V5</h1>
    <p>PANEL FREEFIRE</p>

    <div class="toggle-group">
      <label>
        <i>📄</i>
        EASY DRAG
      </label>
      <div class="toggle-switch" onclick="toggleSwitch(this)"></div>
    </div>

    <div class="toggle-group">
      <label>
        <i>🎯</i>
        STABILIZER
      </label>
      <div class="toggle-switch active" onclick="toggleSwitch(this)"></div>
    </div>

    <div class="toggle-group">
      <label>
        <i>🚀</i>
        LOCK FPS
      </label>
      <div class="toggle-switch" onclick="toggleSwitch(this)"></div>
    </div>

    <div class="footer">BY: @JUST HAMZ</div>
  </div>

  <script>
    function toggleSwitch(element) {
      element.classList.toggle('active');
    }
  </script>
</body>
</html>
