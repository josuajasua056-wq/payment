<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Toko Barang Game - HD Quality</title>
    <style>
        /* Reset dan base styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
            color: #fff;
            min-height: 100vh;
            padding: 20px;
            overflow-x: hidden;
        }
        
        /* Container utama */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        /* Header */
        header {
            text-align: center;
            margin-bottom: 40px;
            animation: fadeIn 1s ease-out;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            background: linear-gradient(to right, #ff7e5f, #feb47b);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
        }
        
        /* Grid barang */
        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 25px;
            margin-bottom: 40px;
        }
        
        /* Kartu produk */
        .product-card {
            background: rgba(255, 255, 255, 0.05);
            border-radius: 15px;
            overflow: hidden;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.4s ease;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
            animation: slideUp 0.5s ease-out;
        }
        
        .product-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.3);
            border-color: rgba(255, 255, 255, 0.2);
        }
        
        .product-header {
            padding: 20px;
            text-align: center;
            background: rgba(0, 0, 0, 0.2);
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .product-name {
            font-size: 1.5rem;
            font-weight: 600;
            margin-bottom: 5px;
        }
        
        .product-body {
            padding: 20px;
        }
        
        .product-price {
            font-size: 1.2rem;
            color: #4ecca3;
            margin-bottom: 20px;
            text-align: center;
            display: none;
            animation: fadeIn 0.5s ease-out;
        }
        
        .btn-show-price {
            display: block;
            width: 100%;
            padding: 12px;
            background: linear-gradient(to right, #ff7e5f, #feb47b);
            color: white;
            border: none;
            border-radius: 8px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
        }
        
        .btn-show-price:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.3);
        }
        
        .btn-show-price:active {
            transform: translateY(0);
        }
        
        /* Animasi */
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        @keyframes slideUp {
            from { 
                opacity: 0;
                transform: translateY(30px);
            }
            to { 
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        /* Responsif */
        @media (max-width: 768px) {
            .products-grid {
                grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
                gap: 20px;
            }
            
            h1 {
                font-size: 2rem;
            }
        }
        
        /* Efek smooth scroll */
        html {
            scroll-behavior: smooth;
        }
        
        /* Efek kilap pada kartu */
        .product-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.1), transparent);
            transition: 0.5s;
        }
        
        .product-card:hover::before {
            left: 100%;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Katalog Barang Game</h1>
            <p>Kualitas HD • Harga Terjangkau • Transaksi Aman</p>
        </header>
        
        <div class="products-grid">
            <!-- Jasteb -->
            <div class="product-card">
                <div class="product-header">
                    <h3 class="product-name">Jasteb</h3>
                </div>
                <div class="product-body">
                    <p class="product-price" id="jasteb-price">
                        1k = 20res<br>
                        2k = 70res<br>
                        3k = 90res<br>
                        4k = 150res<br>
                        5k = 250res
                    </p>
                    <button class="btn-show-price" onclick="togglePrice('jasteb-price', this)">Lihat Harga</button>
                </div>
            </div>
            
            <!-- Murlog -->
            <div class="product-card">
                <div class="product-header">
                    <h3 class="product-name">Murlog</h3>
                </div>
                <div class="product-body">
                    <p class="product-price" id="murlog-price">
                        1k + Full Tutor = ?res
                    </p>
                    <button class="btn-show-price" onclick="togglePrice('murlog-price', this)">Lihat Harga</button>
                </div>
            </div>
            
            <!-- Mursun -->
            <div class="product-card">
                <div class="product-header">
                    <h3 class="product-name">Mursun</h3>
                </div>
                <div class="product-body">
                    <p class="product-price" id="mursun-price">
                        1k + Full Tutor = ?res
                    </p>
                    <button class="btn-show-price" onclick="togglePrice('mursun-price', this)">Lihat Harga</button>
                </div>
            </div>
            
            <!-- SC Bug Dreadt Invictus -->
            <div class="product-card">
                <div class="product-header">
                    <h3 class="product-name">SC Bug Dreadt Invictus</h3>
                </div>
                <div class="product-body">
                    <p class="product-price" id="scbug-price">
                        Harga: 10k
                    </p>
                    <button class="btn-show-price" onclick="togglePrice('scbug-price', this)">Lihat Harga</button>
                </div>
            </div>
            
            <!-- Mod The Spike -->
            <div class="product-card">
                <div class="product-header">
                    <h3 class="product-name">Mod The Spike</h3>
                </div>
                <div class="product-body">
                    <p class="product-price" id="modspike-price">
                        Harga: 5k
                    </p>
                    <button class="btn-show-price" onclick="togglePrice('modspike-price', this)">Lihat Harga</button>
                </div>
            </div>
            
            <!-- Crate Web Payment -->
            <div class="product-card">
                <div class="product-header">
                    <h3 class="product-name">Crate Web Payment</h3>
                </div>
                <div class="product-body">
                    <p class="product-price" id="crateweb-price">
                        Harga: 3k
                    </p>
                    <button class="btn-show-price" onclick="togglePrice('crateweb-price', this)">Lihat Harga</button>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Fungsi untuk menampilkan/sembunyikan harga
        function togglePrice(priceId, button) {
            const priceElement = document.getElementById(priceId);
            
            if (priceElement.style.display === 'block') {
                priceElement.style.display = 'none';
                button.textContent = 'Lihat Harga';
            } else {
                // Sembunyikan semua harga terlebih dahulu
                document.querySelectorAll('.product-price').forEach(price => {
                    price.style.display = 'none';
                });
                
                // Ubah teks semua button kembali ke "Lihat Harga"
                document.querySelectorAll('.btn-show-price').forEach(btn => {
                    btn.textContent = 'Lihat Harga';
                });
                
                // Tampilkan harga yang dipilih
                priceElement.style.display = 'block';
                button.textContent = 'Tutup';
            }
        }
        
        // Animasi untuk kartu produk
        document.addEventListener('DOMContentLoaded', function() {
            const productCards = document.querySelectorAll('.product-card');
            
            productCards.forEach((card, index) => {
                // Delay munculnya animasi untuk setiap kartu
                card.style.animationDelay = `${index * 0.1}s`;
            });
        });
    </script>
</body>
</html>