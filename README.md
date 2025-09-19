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
            width: 100%;
            max-width: 500px;
            background: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.2);
            overflow: hidden;
            transition: transform 0.3s ease;
        }

        .container:hover {
            transform: translateY(-5px);
        }

        .header {
            background: linear-gradient(to right, #008ffc, #00c3ff);
            padding: 30px 20px;
            text-align: center;
            color: white;
        }

        .header h1 {
            font-size: 28px;
            margin-bottom: 10px;
            font-weight: 600;
        }

        .header p {
            font-size: 16px;
            opacity: 0.9;
        }

        .content {
            padding: 30px;
        }

        .payment-info {
            text-align: center;
            margin-bottom: 25px;
        }

        .payment-info h2 {
            color: #333;
            margin-bottom: 15px;
            font-size: 22px;
        }

        .qris-container {
            background: white;
            padding: 15px;
            border-radius: 12px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            margin: 20px 0;
            display: inline-block;
        }

        .qris-code {
            width: 250px;
            height: 250px;
            background-image: url('https://files.catbox.moe/7yokm2.jpg');
            background-size: contain;
            background-repeat: no-repeat;
            background-position: center;
            margin: 0 auto;
            border: 1px solid #eee;
            border-radius: 8px;
        }

        .dana-number {
            background: #f8f9fa;
            padding: 15px;
            border-radius: 12px;
            margin: 20px 0;
            text-align: center;
        }

        .dana-number h3 {
            color: #008ffc;
            margin-bottom: 10px;
            font-size: 18px;
        }

        .dana-number p {
            font-size: 22px;
            font-weight: 600;
            color: #333;
            letter-spacing: 1.5px;
        }

        .instructions {
            background: #f0f7ff;
            padding: 20px;
            border-radius: 12px;
            margin-top: 25px;
        }

        .instructions h3 {
            color: #008ffc;
            margin-bottom: 15px;
            font-size: 18px;
        }

        .instructions ol {
            padding-left: 20px;
            color: #555;
        }

        .instructions li {
            margin-bottom: 10px;
            line-height: 1.5;
        }

        .footer {
            text-align: center;
            padding: 20px;
            color: #777;
            font-size: 14px;
            background: #f8f9fa;
        }

        .animation {
            animation: fadeIn 0.8s ease;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @media (max-width: 600px) {
            .container {
                border-radius: 15px;
            }
            
            .header {
                padding: 25px 15px;
            }
            
            .content {
                padding: 20px;
            }
            
            .qris-code {
                width: 200px;
                height: 200px;
            }
        }
    </style>
</head>
<body>
    <div class="container animation">
        <div class="header">
            <h1>PEMBAYARAN DANA QRIS</h1>
            <p>Scan QRIS di bawah untuk melakukan pembayaran</p>
        </div>
        
        <div class="content">
            <div class="payment-info">
                <h2>Bayar dengan DANA</h2>
                
                <div class="qris-container">
                    <div class="qris-code"></div>
                </div>
                
                <div class="dana-number">
                    <h3>Nomor DANA</h3>
                    <p>085714353387</p>
                </div>
            </div>
            
            <div class="instructions">
                <h3>Cara Pembayaran:</h3>
                <ol>
                    <li>Buka aplikasi DANA di ponsel Anda</li>
                    <li>Pilih menu 'Bayar' atau 'Scan'</li>
                    <li>Scan kode QR di atas atau masukkan nomor DANA secara manual</li>
                    <li>Masukkan jumlah pembayaran yang sesuai</li>
                    <li>Konfirmasi dan masukkan PIN DANA Anda</li>
                    <li>Tunggu hingga transaksi selesai</li>
                </ol>
            </div>
        </div>
        
        <div class="footer">
            <p>&copy; 2023 Payment DANA QRIS. Semua hak dilindungi.</p>
        </div>
    </div>
</body>
</html>