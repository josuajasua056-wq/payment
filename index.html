<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Payment DANA QRIS</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }
        
        .container {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.2);
            width: 100%;
            max-width: 500px;
            padding: 30px;
            text-align: center;
            animation: fadeIn 0.8s ease-out;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .logo {
            width: 100px;
            margin-bottom: 20px;
        }
        
        h1 {
            color: #333;
            margin-bottom: 10px;
            font-weight: 600;
        }
        
        p {
            color: #666;
            margin-bottom: 25px;
            line-height: 1.6;
        }
        
        .qris-container {
            background: white;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            margin: 20px 0;
            transition: transform 0.3s ease;
        }
        
        .qris-container:hover {
            transform: translateY(-5px);
        }
        
        .qris-title {
            font-weight: 500;
            color: #333;
            margin-bottom: 15px;
        }
        
        .qris-code {
            width: 100%;
            max-width: 280px;
            height: auto;
            border-radius: 10px;
            margin: 0 auto;
            display: block;
            border: 1px solid #eee;
        }
        
        .divider {
            height: 1px;
            background: linear-gradient(to right, transparent, #ddd, transparent);
            margin: 25px 0;
        }
        
        .payment-info {
            background: #f8f9fa;
            padding: 15px;
            border-radius: 12px;
            margin: 20px 0;
            text-align: left;
        }
        
        .info-title {
            font-weight: 500;
            color: #444;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
        }
        
        .info-title i {
            margin-right: 10px;
            color: #6a11cb;
        }
        
        .dana-number {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: white;
            padding: 12px 15px;
            border-radius: 8px;
            margin-top: 10px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
        }
        
        .number {
            font-family: monospace;
            font-size: 18px;
            color: #333;
        }
        
        .copy-btn {
            background: #6a11cb;
            color: white;
            border: none;
            padding: 8px 15px;
            border-radius: 6px;
            cursor: pointer;
            transition: background 0.3s;
            display: flex;
            align-items: center;
        }
        
        .copy-btn:hover {
            background: #2575fc;
        }
        
        .copy-btn i {
            margin-right: 5px;
        }
        
        .instructions {
            text-align: left;
            margin: 25px 0;
        }
        
        .instructions ol {
            padding-left: 20px;
            color: #666;
        }
        
        .instructions li {
            margin-bottom: 10px;
            line-height: 1.5;
        }
        
        .note {
            background: #fff8e1;
            padding: 15px;
            border-radius: 10px;
            border-left: 4px solid #ffc107;
            text-align: left;
            margin: 20px 0;
            font-size: 14px;
            color: #666;
        }
        
        .success-message {
            position: fixed;
            top: 20px;
            left: 50%;
            transform: translateX(-50%);
            background: #4caf50;
            color: white;
            padding: 15px 25px;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            z-index: 1000;
            opacity: 0;
            transition: opacity 0.3s;
        }
        
        .success-message.show {
            opacity: 1;
        }
        
        @media (max-width: 600px) {
            .container {
                padding: 20px;
            }
            
            h1 {
                font-size: 24px;
            }
            
            .dana-number {
                flex-direction: column;
                gap: 10px;
            }
            
            .copy-btn {
                width: 100%;
                justify-content: center;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Pembayaran DANA QRIS</h1>
        <p>Scan QR code berikut atau salin nomor DANA untuk melakukan pembayaran</p>
        
        <div class="qris-container">
            <div class="qris-title">QRIS Code Pembayaran</div>
            <img src="https://files.catbox.moe/7yokm2.jpg" alt="QRIS DANA" class="qris-code">
        </div>
        
        <div class="divider"></div>
        
        <div class="payment-info">
            <div class="info-title"><i class="fas fa-wallet"></i> Nomor DANA</div>
            <div class="dana-number">
                <span class="number" id="danaNumber">085714353387</span>
                <button class="copy-btn" id="copyButton"><i class="fas fa-copy"></i> Salin</button>
            </div>
        </div>
        
        <div class="instructions">
            <div class="info-title"><i class="fas fa-info-circle"></i> Cara Pembayaran:</div>
            <ol>
                <li>Buka aplikasi DANA di smartphone Anda</li>
                <li>Tap ikon QR di bagian atas halaman utama</li>
                <li>Scan QR code yang tertera di atas</li>
                <li>Atau transfer manual ke nomor DANA yang tertera</li>
                <li>Masukkan jumlah nominal yang ingin ditransfer</li>
                <li>Konfirmasi dan masukkan PIN DANA Anda</li>
            </ol>
        </div>
        
        <div class="note">
            <strong>Catatan:</strong> Pastikan saldo DANA Anda mencukupi. Pembayaran akan diproses secara instan setelah transfer berhasil.
        </div>
    </div>
    
    <div class="success-message" id="successMessage">Nomor DANA berhasil disalin!</div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const copyButton = document.getElementById('copyButton');
            const danaNumber = document.getElementById('danaNumber');
            const successMessage = document.getElementById('successMessage');
            
            copyButton.addEventListener('click', function() {
                const tempTextArea = document.createElement('textarea');
                tempTextArea.value = danaNumber.textContent;
                document.body.appendChild(tempTextArea);
                tempTextArea.select();
                document.execCommand('copy');
                document.body.removeChild(tempTextArea);
                
                // Tampilkan pesan sukses
                successMessage.classList.add('show');
                
                // Sembunyikan pesan setelah 3 detik
                setTimeout(function() {
                    successMessage.classList.remove('show');
                }, 3000);
            });
            
            // Preload gambar QR code untuk menghindari error
            const qrImage = new Image();
            qrImage.src = "https://files.catbox.moe/7yokm2.jpg";
            
            qrImage.onload = function() {
                console.log("QR code berhasil dimuat");
            };
            
            qrImage.onerror = function() {
                console.log("Error saat memuat QR code");
                document.querySelector('.qris-code').alt = "QR code tidak dapat dimuat. Silakan gunakan nomor DANA secara manual.";
            };
        });
    </script>
</body>
</html>