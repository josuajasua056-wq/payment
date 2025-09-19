<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pembayaran QRIS DANA</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #ff0000, #ffffff);
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
    }
    .card {
      background: #fff;
      padding: 25px;
      border-radius: 15px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.2);
      text-align: center;
      max-width: 360px;
      width: 100%;
    }
    h2 {
      color: #e60000;
      margin-bottom: 15px;
    }
    img {
      width: 250px;
      border-radius: 10px;
      margin-bottom: 15px;
    }
    .dana-box {
      background: #f8f8f8;
      padding: 10px;
      border-radius: 8px;
      font-size: 18px;
      font-weight: bold;
      color: #333;
      margin-bottom: 10px;
    }
    button {
      background: #e60000;
      color: white;
      border: none;
      padding: 10px 20px;
      border-radius: 8px;
      cursor: pointer;
      font-size: 16px;
    }
    button:hover {
      background: #b30000;
    }
  </style>
</head>
<body>
  <div class="card">
    <h2>Pembayaran QRIS DANA</h2>
    <!-- QRIS base64 -->
    <img src="data:image/png;base64,
    iVBORw0KGgoAAAANSUhEUgAAA... (disingkat karena panjang) ..." 
    alt="QRIS DANA">
    
    <div class="dana-box">
      Nomor DANA: 085714353387
    </div>
    <button onclick="copyDana()">Copy Nomor DANA</button>
  </div>

  <script>
    function copyDana() {
      navigator.clipboard.writeText("085714353387").then(() => {
        alert("Nomor DANA berhasil disalin!");
      });
    }
  </script>
</body>
</html>