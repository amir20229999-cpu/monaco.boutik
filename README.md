<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>موناکو | بوتیک لباس لوکس</title>
    <meta name="description" content="بوتیک موناکو - ارائه کننده لباس‌های لوکس و شیک با بهترین کیفیت و قیمت">
    <meta name="keywords" content="لباس لوکس, فروشگاه پوشاک, مد روز, پیراهن مردانه, پیراهن زنانه">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* Reset و تنظیمات پیشرفته */
        :root {
            --primary: #e74c3c;
            --primary-dark: #c0392b;
            --primary-light: #ff7675;
            --secondary: #2c3e50;
            --secondary-light: #34495e;
            --accent: #f39c12;
            --accent-light: #f1c40f;
            --light: #f8f9fa;
            --dark: #2d3436;
            --gray: #636e72;
            --gray-light: #dfe6e9;
            --success: #00b894;
            --danger: #d63031;
            --warning: #fdcb6e;
            --info: #0984e3;
            --gold: #ffd700;
            --silver: #bdc3c7;
            --whatsapp: #25D366;
            --telegram: #0088cc;
            --border-radius-sm: 8px;
            --border-radius: 16px;
            --border-radius-lg: 24px;
            --shadow-sm: 0 2px 8px rgba(0,0,0,0.06);
            --shadow: 0 8px 30px rgba(0,0,0,0.12);
            --shadow-lg: 0 20px 60px rgba(0,0,0,0.16);
            --transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.1);
            --gradient-primary: linear-gradient(135deg, #e74c3c 0%, #c0392b 100%);
            --gradient-gold: linear-gradient(135deg, #ffd700 0%, #f39c12 100%);
            --gradient-dark: linear-gradient(135deg, #2c3e50 0%, #1a252f 100%);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            -webkit-tap-highlight-color: transparent;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Vazirmatn', Roboto, Oxygen, Ubuntu, sans-serif;
            background: linear-gradient(135deg, #f5f7fa 0%, #e4e8f0 100%);
            color: var(--dark);
            line-height: 1.7;
            overflow-x: hidden;
            min-height: 100vh;
        }

        h1, h2, h3, h4, h5, h6 {
            font-weight: 700;
            line-height: 1.3;
            margin-bottom: 1rem;
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* سیستم موسیقی */
        .music-player {
            position: fixed;
            bottom: 30px;
            left: 30px;
            z-index: 10000;
            background: rgba(255, 255, 255, 0.98);
            backdrop-filter: blur(20px);
            border-radius: 50px;
            padding: 12px 20px;
            box-shadow: var(--shadow-lg);
            display: flex;
            align-items: center;
            gap: 15px;
            border: 1px solid rgba(255, 255, 255, 0.3);
        }

        .music-btn {
            width: 56px;
            height: 56px;
            border-radius: 50%;
            background: var(--gradient-primary);
            border: none;
            color: white;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.4rem;
            transition: var(--transition);
            box-shadow: 0 4px 15px rgba(231, 76, 60, 0.3);
        }

        .music-btn:hover {
            transform: translateY(-3px) scale(1.05);
            box-shadow: 0 8px 25px rgba(231, 76, 60, 0.4);
        }

        .music-btn.playing {
            background: var(--gradient-gold);
        }

        .volume-control {
            display: flex;
            align-items: center;
            gap: 10px;
            width: 180px;
        }

        .volume-slider {
            flex: 1;
            height: 6px;
            -webkit-appearance: none;
            background: linear-gradient(90deg, var(--primary) 0%, #ddd 0%);
            border-radius: 3px;
            outline: none;
        }

        .volume-slider::-webkit-slider-thumb {
            -webkit-appearance: none;
            width: 20px;
            height: 20px;
            border-radius: 50%;
            background: white;
            border: 3px solid var(--primary);
            cursor: pointer;
            box-shadow: 0 2px 10px rgba(0,0,0,0.2);
        }

        .now-playing {
            font-size: 0.9rem;
            color: var(--gray);
            font-weight: 500;
            white-space: nowrap;
        }

        /* هدر */
        header {
            background: linear-gradient(135deg, rgba(44, 62, 80, 0.95) 0%, rgba(231, 76, 60, 0.9) 100%);
            padding: 1rem 0;
            position: sticky;
            top: 0;
            z-index: 9999;
            box-shadow: var(--shadow);
            backdrop-filter: blur(10px);
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 2rem;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 12px;
            text-decoration: none;
        }

        .logo-icon {
            width: 50px;
            height: 50px;
            background: var(--gradient-gold);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.8rem;
            color: var(--secondary);
            box-shadow: 0 4px 15px rgba(255, 215, 0, 0.3);
        }

        .logo-text {
            display: flex;
            flex-direction: column;
        }

        .logo-text h1 {
            font-size: 1.8rem;
            color: white;
            margin: 0;
            letter-spacing: 1px;
        }

        .logo-text span {
            font-size: 0.9rem;
            color: rgba(255, 255, 255, 0.8);
            font-weight: 300;
        }

        .nav-menu {
            display: flex;
            list-style: none;
            gap: 2.5rem;
            align-items: center;
        }

        .nav-item {
            position: relative;
        }

        .nav-link {
            color: white;
            text-decoration: none;
            font-weight: 500;
            font-size: 1.05rem;
            padding: 0.5rem 0;
            transition: var(--transition);
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .nav-link:hover {
            color: var(--accent-light);
        }

        .auth-buttons {
            display: flex;
            gap: 1rem;
        }

        /* دکمه‌ها */
        .btn {
            padding: 12px 28px;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            font-weight: 600;
            font-size: 1rem;
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            transition: var(--transition);
            position: relative;
            overflow: hidden;
        }

        .btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.2), transparent);
            transition: 0.5s;
        }

        .btn:hover::before {
            left: 100%;
        }

        .btn-primary {
            background: var(--gradient-primary);
            color: white;
            box-shadow: 0 6px 20px rgba(231, 76, 60, 0.3);
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 12px 30px rgba(231, 76, 60, 0.4);
        }

        .btn-secondary {
            background: rgba(255, 255, 255, 0.15);
            color: white;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .btn-secondary:hover {
            background: rgba(255, 255, 255, 0.25);
            transform: translateY(-3px);
        }

        .btn-gold {
            background: var(--gradient-gold);
            color: var(--dark);
            font-weight: 700;
            box-shadow: 0 6px 20px rgba(255, 215, 0, 0.3);
        }

        .btn-gold:hover {
            transform: translateY(-3px) scale(1.05);
            box-shadow: 0 12px 30px rgba(255, 215, 0, 0.4);
        }

        .btn-whatsapp {
            background: linear-gradient(135deg, var(--whatsapp), #128C7E);
            color: white;
        }

        .btn-telegram {
            background: linear-gradient(135deg, var(--telegram), #006699);
            color: white;
        }

        /* Hero Section */
        .hero {
            position: relative;
            padding: 120px 0;
            background: linear-gradient(rgba(44, 62, 80, 0.85), rgba(231, 76, 60, 0.75)), 
                        url('https://images.unsplash.com/photo-1441986300917-64674bd600d8?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            overflow: hidden;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
            position: relative;
            z-index: 2;
        }

        .hero h1 {
            font-size: 4rem;
            margin-bottom: 1.5rem;
            text-shadow: 2px 2px 10px rgba(0,0,0,0.3);
        }

        .hero p {
            font-size: 1.3rem;
            margin-bottom: 2.5rem;
            opacity: 0.9;
            line-height: 1.8;
        }

        /* Features */
        .features {
            padding: 100px 0;
            background: white;
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }

        .feature-card {
            background: white;
            padding: 40px 30px;
            border-radius: var(--border-radius);
            text-align: center;
            box-shadow: var(--shadow);
            transition: var(--transition);
            position: relative;
            overflow: hidden;
        }

        .feature-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 4px;
            background: var(--gradient-primary);
        }

        .feature-card:hover {
            transform: translateY(-10px);
            box-shadow: var(--shadow-lg);
        }

        .feature-icon {
            width: 80px;
            height: 80px;
            background: linear-gradient(135deg, #f8f9fa, #e9ecef);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 25px;
            font-size: 2.5rem;
            color: var(--primary);
            transition: var(--transition);
        }

        .feature-card:hover .feature-icon {
            background: var(--gradient-primary);
            color: white;
            transform: rotateY(360deg);
        }

        .feature-card h3 {
            font-size: 1.4rem;
            margin-bottom: 15px;
            color: var(--secondary);
        }

        .feature-card p {
            color: var(--gray);
            line-height: 1.7;
        }

        /* Products Section */
        .products-section {
            padding: 100px 0;
            background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
        }

        .section-header {
            text-align: center;
            margin-bottom: 60px;
        }

        .section-header h2 {
            font-size: 3rem;
            color: var(--secondary);
            margin-bottom: 20px;
            position: relative;
            display: inline-block;
        }

        .section-header h2::after {
            content: '';
            position: absolute;
            bottom: -15px;
            right: 50%;
            transform: translateX(50%);
            width: 80px;
            height: 4px;
            background: var(--gradient-primary);
            border-radius: 2px;
        }

        .section-header p {
            font-size: 1.2rem;
            color: var(--gray);
            max-width: 600px;
            margin: 30px auto 0;
            line-height: 1.8;
        }

        /* Product Grid */
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }

        .product-card {
            background: white;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition);
            position: relative;
        }

        .product-card:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: var(--shadow-lg);
        }

        .product-image-container {
            position: relative;
            width: 100%;
            height: 300px;
            overflow: hidden;
        }

        .product-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }

        .product-card:hover .product-image {
            transform: scale(1.1);
        }

        .product-badge {
            position: absolute;
            top: 20px;
            left: 20px;
            background: var(--gradient-primary);
            color: white;
            padding: 8px 20px;
            border-radius: 50px;
            font-size: 0.85rem;
            font-weight: 600;
            letter-spacing: 1px;
            z-index: 2;
            box-shadow: 0 4px 15px rgba(231, 76, 60, 0.3);
        }

        .product-badge.sale {
            background: var(--gradient-gold);
        }

        .product-badge.new {
            background: linear-gradient(135deg, var(--success), #00a085);
        }

        .product-info {
            padding: 30px;
        }

        .product-title {
            font-size: 1.4rem;
            color: var(--secondary);
            margin-bottom: 15px;
            line-height: 1.4;
        }

        .product-description {
            color: var(--gray);
            margin-bottom: 20px;
            line-height: 1.6;
        }

        .price-container {
            display: flex;
            align-items: center;
            gap: 15px;
            margin-bottom: 25px;
            flex-wrap: wrap;
        }

        .current-price {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary);
        }

        .original-price {
            font-size: 1.2rem;
            color: var(--gray);
            text-decoration: line-through;
        }

        .discount-percentage {
            background: var(--success);
            color: white;
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 600;
        }

        .product-colors {
            display: flex;
            gap: 10px;
            margin-bottom: 25px;
        }

        .color-option {
            width: 30px;
            height: 30px;
            border-radius: 50%;
            border: 2px solid white;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
            cursor: pointer;
            transition: var(--transition);
        }

        .color-option:hover {
            transform: scale(1.1);
        }

        .product-actions {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 12px;
        }

        /* Message Section */
        .message-section {
            background: linear-gradient(135deg, #e8f5e9, #c8e6c9);
            padding: 60px;
            border-radius: var(--border-radius);
            margin: 60px 0;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .message-section h3 {
            font-size: 2.2rem;
            color: #2d3436;
            margin-bottom: 20px;
        }

        .message-section p {
            font-size: 1.1rem;
            color: #636e72;
            max-width: 700px;
            margin: 0 auto 30px;
            line-height: 1.8;
        }

        /* Admin Panel */
        .admin-panel {
            background: white;
            padding: 50px;
            border-radius: var(--border-radius-lg);
            margin: 60px 0;
            box-shadow: var(--shadow-lg);
            border: 1px solid rgba(0,0,0,0.05);
            display: none;
        }

        .admin-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 40px;
            padding-bottom: 25px;
            border-bottom: 2px solid var(--gray-light);
        }

        .admin-header h2 {
            font-size: 2.5rem;
            color: var(--secondary);
            display: flex;
            align-items: center;
            gap: 15px;
        }

        /* مودال‌ها */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            z-index: 10001;
            overflow-y: auto;
            padding: 20px;
            backdrop-filter: blur(10px);
        }

        .modal-content {
            background: white;
            border-radius: var(--border-radius-lg);
            width: 100%;
            max-width: 600px;
            margin: 50px auto;
            position: relative;
            box-shadow: var(--shadow-lg);
        }

        .modal-header {
            padding: 30px 40px 20px;
            border-bottom: 1px solid var(--gray-light);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .modal-header h2 {
            font-size: 2rem;
            color: var(--secondary);
            margin: 0;
        }

        .close-btn {
            background: none;
            border: none;
            font-size: 2rem;
            color: var(--gray);
            cursor: pointer;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: var(--transition);
        }

        .close-btn:hover {
            background: var(--gray-light);
            color: var(--dark);
        }

        .modal-body {
            padding: 30px 40px;
            max-height: 70vh;
            overflow-y: auto;
        }

        /* فرم‌ها */
        .form-group {
            margin-bottom: 25px;
        }

        .form-label {
            display: block;
            margin-bottom: 10px;
            font-weight: 600;
            color: var(--secondary);
            font-size: 1rem;
        }

        .form-control {
            width: 100%;
            padding: 15px 20px;
            border: 2px solid var(--gray-light);
            border-radius: var(--border-radius-sm);
            font-size: 1rem;
            font-family: inherit;
            transition: var(--transition);
            background: white;
        }

        .form-control:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 3px rgba(231, 76, 60, 0.1);
        }

        .file-upload {
            border: 2px dashed var(--gray-light);
            border-radius: var(--border-radius);
            padding: 40px;
            text-align: center;
            cursor: pointer;
            transition: var(--transition);
        }

        .file-upload:hover {
            border-color: var(--primary);
            background: rgba(231, 76, 60, 0.02);
        }

        .file-upload i {
            font-size: 3rem;
            color: var(--primary);
            margin-bottom: 20px;
        }

        /* Footer */
        footer {
            background: var(--gradient-dark);
            color: white;
            padding: 80px 0 30px;
            position: relative;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 60px;
        }

        .footer-section h3 {
            font-size: 1.4rem;
            margin-bottom: 25px;
            color: white;
            position: relative;
            padding-bottom: 15px;
        }

        .footer-section h3::after {
            content: '';
            position: absolute;
            bottom: 0;
            right: 0;
            width: 50px;
            height: 2px;
            background: var(--accent-light);
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 12px;
        }

        .footer-links a {
            color: rgba(255, 255, 255, 0.8);
            text-decoration: none;
            transition: var(--transition);
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .footer-links a:hover {
            color: var(--accent-light);
            padding-right: 10px;
        }

        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }

        .social-link {
            width: 45px;
            height: 45px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-decoration: none;
            transition: var(--transition);
        }

        .social-link:hover {
            background: var(--primary);
            transform: translateY(-3px);
        }

        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: rgba(255, 255, 255, 0.7);
            font-size: 0.9rem;
        }

        /* Responsive Design */
        @media (max-width: 1200px) {
            .hero h1 {
                font-size: 3.5rem;
            }
            
            .section-header h2 {
                font-size: 2.5rem;
            }
        }

        @media (max-width: 992px) {
            .nav-menu {
                display: none;
            }
            
            .hero h1 {
                font-size: 3rem;
            }
            
            .product-grid {
                grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            }
        }

        @media (max-width: 768px) {
            .hero {
                padding: 80px 0;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .hero p {
                font-size: 1.1rem;
            }
            
            .features-grid {
                grid-template-columns: 1fr;
            }
            
            .product-grid {
                grid-template-columns: 1fr;
            }
            
            .music-player {
                bottom: 20px;
                left: 20px;
                right: 20px;
                flex-direction: column;
                align-items: stretch;
                padding: 15px;
            }
            
            .volume-control {
                width: 100%;
            }
            
            .modal-content {
                margin: 20px auto;
            }
        }

        @media (max-width: 576px) {
            .navbar {
                padding: 0 1rem;
            }
            
            .logo-text h1 {
                font-size: 1.5rem;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
            
            .btn {
                padding: 10px 20px;
                font-size: 0.9rem;
            }
            
            .section-header h2 {
                font-size: 2rem;
            }
        }

        /* Scrollbar */
        ::-webkit-scrollbar {
            width: 10px;
        }

        ::-webkit-scrollbar-track {
            background: #f1f1f1;
        }

        ::-webkit-scrollbar-thumb {
            background: linear-gradient(180deg, var(--primary), var(--primary-dark));
            border-radius: 5px;
        }

        ::-webkit-scrollbar-thumb:hover {
            background: linear-gradient(180deg, var(--primary-dark), var(--secondary));
        }
    </style>
</head>
<body>
    <!-- Music Player -->
    <div class="music-player">
        <button class="music-btn" id="musicToggle">
            <i class="fas fa-music"></i>
        </button>
        <div class="volume-control" id="volumeControl">
            <i class="fas fa-volume-up"></i>
            <input type="range" class="volume-slider" id="volumeSlider" min="0" max="1" step="0.1" value="0.3">
        </div>
        <div class="now-playing" id="nowPlaying">
            موسیقی آرامش‌بخش
        </div>
    </div>

    <!-- Header -->
    <header>
        <nav class="navbar container">
            <a href="#" class="logo">
                <div class="logo-icon">
                    <i class="fas fa-crown"></i>
                </div>
                <div class="logo-text">
                    <h1>موناکو</h1>
                    <span>بوتیک لباس لوکس</span>
                </div>
            </a>
            
            <ul class="nav-menu">
                <li class="nav-item"><a href="#" class="nav-link"><i class="fas fa-home"></i> خانه</a></li>
                <li class="nav-item"><a href="#products" class="nav-link"><i class="fas fa-tshirt"></i> محصولات</a></li>
                <li class="nav-item"><a href="#" class="nav-link"><i class="fas fa-info-circle"></i> درباره ما</a></li>
                <li class="nav-item"><a href="#" class="nav-link"><i class="fas fa-phone"></i> تماس</a></li>
            </ul>
            
            <div class="auth-buttons">
                <button class="btn btn-secondary" onclick="openLogin()">
                    <i class="fas fa-sign-in-alt"></i>
                    ورود
                </button>
                <button class="btn btn-primary" onclick="openRegister()">
                    <i class="fas fa-user-plus"></i>
                    ثبت‌نام
                </button>
                <button class="btn btn-secondary" id="adminBtn" style="display: none;" onclick="toggleAdminPanel()">
                    <i class="fas fa-cog"></i>
                    پنل مدیریت
                </button>
                <button class="btn btn-primary" id="logoutBtn" style="display: none;" onclick="logout()">
                    <i class="fas fa-sign-out-alt"></i>
                    خروج
                </button>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <div class="hero-content">
                <h1>تجربه‌ای لوکس از دنیای مد</h1>
                <p>در بوتیک موناکو، زیبایی و کیفیت در هم می‌آمیزد. با انتخاب‌های بی‌نظیر ما، استایلی منحصر به فرد برای خود خلق کنید.</p>
                <div class="hero-cta">
                    <button class="btn btn-gold" onclick="showBuyGuide()">
                        <i class="fas fa-shopping-bag"></i>
                        شروع خرید اکنون
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- Features -->
    <section class="features">
        <div class="container">
            <div class="section-header">
                <h2>چرا موناکو را انتخاب کنید؟</h2>
                <p>ما تعهد داریم بهترین تجربه خرید را برای شما فراهم کنیم</p>
            </div>
            
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-award"></i>
                    </div>
                    <h3>کیفیت درجه یک</h3>
                    <p>استفاده از بهترین پارچه‌ها و دوخت حرفه‌ای برای محصولاتی با ماندگاری بالا</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-shipping-fast"></i>
                    </div>
                    <h3>تحویل سریع</h3>
                    <p>ارسال رایگان برای خریدهای بالای 500 هزار تومان و تحویل در کمترین زمان</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-headset"></i>
                    </div>
                    <h3>پشتیبانی ۲۴/۷</h3>
                    <p>تیم پشتیبانی ما همیشه آماده پاسخگویی به سوالات و راهنمایی شماست</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <h3>ضمانت بازگشت</h3>
                    <p>در صورت عدم رضایت، تا ۷ روز امکان بازگشت کالا با شرایط خاص وجود دارد</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Products Section -->
    <section class="products-section" id="products">
        <div class="container">
            <div class="section-header">
                <h2>محصولات منتخب</h2>
                <p>برترین و شیک‌ترین لباس‌های مجموعه موناکو که توسط متخصصان مد انتخاب شده‌اند</p>
            </div>

            <!-- راهنمای خرید -->
            <div class="message-section">
                <h3><i class="fas fa-comment-dots"></i> برای خرید محصولات با ما در ارتباط باشید</h3>
                <p>کارشناسان فروش ما آماده راهنمایی و پاسخگویی به سوالات شما هستند. برای دریافت مشاوره رایگان و ثبت سفارش، از طریق واتس‌اپ یا تلگرام با ما در ارتباط باشید.</p>
                <div class="social-buttons">
                    <button class="btn btn-whatsapp" onclick="sendWhatsAppMessage()">
                        <i class="fab fa-whatsapp"></i>
                        واتس‌اپ
                    </button>
                    <button class="btn btn-telegram" onclick="sendTelegramMessage()">
                        <i class="fab fa-telegram"></i>
                        تلگرام
                    </button>
                    <button class="btn btn-gold" onclick="showContactInfo()">
                        <i class="fas fa-phone"></i>
                        اطلاعات تماس
                    </button>
                </div>
            </div>

            <!-- Grid محصولات -->
            <div class="product-grid" id="productGrid">
                <!-- محصولات اینجا نمایش داده می‌شوند -->
            </div>
        </div>
    </section>

    <!-- Admin Panel -->
    <div class="admin-panel container" id="adminPanel">
        <div class="admin-header">
            <h2><i class="fas fa-crown"></i> پنل مدیریت</h2>
            <div>
                <button class="btn btn-primary" onclick="openAddProduct()">
                    <i class="fas fa-plus-circle"></i>
                    افزودن محصول جدید
                </button>
                <button class="btn btn-secondary" onclick="exportProducts()" style="margin-right: 15px;">
                    <i class="fas fa-download"></i>
                    خروجی محصولات
                </button>
            </div>
        </div>

        <!-- محصولات ادمین -->
        <div id="adminProductGrid"></div>
    </div>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>درباره موناکو</h3>
                    <p>بوتیک موناکو با بیش از یک دهه تجربه در صنعت مد و پوشاک، متعهد به ارائه بهترین کیفیت و جدیدترین استایل‌ها به مشتریان خود است.</p>
                    <div class="social-links">
                        <a href="#" class="social-link"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="social-link"><i class="fab fa-telegram"></i></a>
                        <a href="#" class="social-link"><i class="fab fa-whatsapp"></i></a>
                    </div>
                </div>
                
                <div class="footer-section">
                    <h3>لینک‌های سریع</h3>
                    <ul class="footer-links">
                        <li><a href="#"><i class="fas fa-chevron-left"></i> خانه</a></li>
                        <li><a href="#products"><i class="fas fa-chevron-left"></i> محصولات</a></li>
                        <li><a href="#"><i class="fas fa-chevron-left"></i> درباره ما</a></li>
                        <li><a href="#"><i class="fas fa-chevron-left"></i> تماس با ما</a></li>
                        <li><a href="#"><i class="fas fa-chevron-left"></i> حریم خصوصی</a></li>
                    </ul>
                </div>
                
                <div class="footer-section">
                    <h3>تماس با ما</h3>
                    <ul class="footer-links">
                        <li><a href="#"><i class="fas fa-map-marker-alt"></i> تهران، خیابان ولیعصر</a></li>
                        <li><a href="tel:+989129573096"><i class="fas fa-phone"></i> ۰۹۱۲۹۵۷۳۰۹۶</a></li>
                        <li><a href="mailto:info@monaco.com"><i class="fas fa-envelope"></i> info@monaco.com</a></li>
                        <li><a href="#"><i class="fas fa-clock"></i> ساعت کار: ۹ صبح تا ۹ شب</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="copyright">
                <p>© ۱۴۰۳ بوتیک موناکو. تمامی حقوق محفوظ است.</p>
            </div>
        </div>
    </footer>

    <!-- مودال‌ها -->
    <div class="modal" id="loginModal">
        <div class="modal-content">
            <div class="modal-header">
                <h2><i class="fas fa-sign-in-alt"></i> ورود به حساب کاربری</h2>
                <button class="close-btn" onclick="closeModals()">×</button>
            </div>
            <div class="modal-body">
                <form id="loginForm" class="modal-form">
                    <div class="form-group">
                        <label class="form-label">آدرس ایمیل</label>
                        <input type="email" id="loginEmail" class="form-control" required placeholder="example@email.com">
                    </div>
                    <div class="form-group">
                        <label class="form-label">رمز عبور</label>
                        <input type="password" id="loginPassword" class="form-control" required placeholder="رمز عبور خود را وارد کنید">
                    </div>
                    <button type="submit" class="btn btn-primary" style="width: 100%; padding: 15px;">
                        <i class="fas fa-sign-in-alt"></i>
                        ورود به حساب
                    </button>
                </form>
            </div>
        </div>
    </div>

    <div class="modal" id="registerModal">
        <div class="modal-content">
            <div class="modal-header">
                <h2><i class="fas fa-user-plus"></i> ایجاد حساب جدید</h2>
                <button class="close-btn" onclick="closeModals()">×</button>
            </div>
            <div class="modal-body">
                <form id="registerForm" class="modal-form">
                    <div class="form-group">
                        <label class="form-label">نام کامل</label>
                        <input type="text" id="registerName" class="form-control" required placeholder="نام و نام خانوادگی">
                    </div>
                    <div class="form-group">
                        <label class="form-label">آدرس ایمیل</label>
                        <input type="email" id="registerEmail" class="form-control" required placeholder="example@email.com">
                    </div>
                    <div class="form-group">
                        <label class="form-label">رمز عبور</label>
                        <input type="password" id="registerPassword" class="form-control" required placeholder="حداقل ۶ کاراکتر">
                    </div>
                    <button type="submit" class="btn btn-primary" style="width: 100%; padding: 15px;">
                        <i class="fas fa-user-plus"></i>
                        ایجاد حساب
                    </button>
                </form>
            </div>
        </div>
    </div>

    <div class="modal" id="addProductModal">
        <div class="modal-content">
            <div class="modal-header">
                <h2><i class="fas fa-plus-circle"></i> افزودن محصول جدید</h2>
                <button class="close-btn" onclick="closeModals()">×</button>
            </div>
            <div class="modal-body">
                <form id="addProductForm" class="modal-form">
                    <div class="form-group">
                        <label class="form-label">نام محصول</label>
                        <input type="text" id="productName" class="form-control" required placeholder="نام کامل محصول">
                    </div>
                    
                    <div class="form-group">
                        <label class="form-label">قیمت (تومان)</label>
                        <input type="number" id="productPrice" class="form-control" required placeholder="مثال: 250000" min="1000">
                    </div>
                    
                    <!-- آپلود عکس -->
                    <div class="form-group">
                        <label class="form-label">عکس‌های محصول</label>
                        <div class="file-upload" id="uploadArea">
                            <i class="fas fa-cloud-upload-alt"></i>
                            <p>عکس‌ها را اینجا بکشید یا کلیک کنید</p>
                            <p style="font-size: 0.9rem; color: var(--gray); margin-top: 0.5rem;">
                                می‌توانید چند عکس آپلود کنید
                            </p>
                            <input type="file" id="imageUpload" multiple accept="image/*" style="display: none;">
                        </div>
                        <div class="uploaded-images" id="uploadedImages" style="display: grid; grid-template-columns: repeat(auto-fill, minmax(100px, 1fr)); gap: 10px; margin-top: 1rem;"></div>
                    </div>
                    
                    <!-- انتخاب رنگ -->
                    <div class="form-group">
                        <label class="form-label">رنگ‌های محصول</label>
                        <div style="display: flex; gap: 0.5rem; margin-bottom: 1rem;">
                            <input type="text" id="colorInput" class="form-control" placeholder="نام رنگ (مثال: مشکی)" style="flex: 1;">
                            <input type="color" id="colorPicker" value="#000000" style="width: 60px;">
                            <button type="button" class="btn btn-primary" onclick="addColor()" style="padding: 10px 20px;">
                                <i class="fas fa-plus"></i>
                            </button>
                        </div>
                        <div id="selectedColors" style="display: flex; flex-wrap: wrap; gap: 0.5rem; margin-top: 1rem;"></div>
                    </div>
                    
                    <div class="form-group">
                        <label class="form-label">سایزهای موجود</label>
                        <input type="text" id="productSize" class="form-control" placeholder="با کاما جدا کنید، مثال: S, M, L, XL">
                    </div>
                    
                    <div class="form-group">
                        <label class="form-label">توضیحات محصول</label>
                        <textarea id="productDescription" class="form-control" placeholder="توضیحات کامل محصول" rows="4"></textarea>
                    </div>
                    
                    <button type="submit" class="btn btn-primary" style="width: 100%; padding: 15px;">
                        <i class="fas fa-plus-circle"></i>
                        افزودن محصول
                    </button>
                </form>
            </div>
        </div>
    </div>

    <div class="modal" id="discountModal">
        <div class="modal-content">
            <div class="modal-header">
                <h2><i class="fas fa-percentage"></i> مدیریت تخفیف</h2>
                <button class="close-btn" onclick="closeModals()">×</button>
            </div>
            <div class="modal-body">
                <div id="discountFormContainer"></div>
            </div>
        </div>
    </div>

    <script>
        // ========== متغیرهای اصلی ==========
        let users = JSON.parse(localStorage.getItem('monaco_users')) || [];
        let products = JSON.parse(localStorage.getItem('monaco_products')) || [];
        let currentUser = JSON.parse(localStorage.getItem('current_user'));
        let currentProductImages = [];
        let currentImageIndex = 0;
        let uploadedImages = [];
        let selectedColors = [];

        // ========== سیستم موسیقی ==========
        const backgroundMusic = new Audio('https://assets.mixkit.co/music/preview/mixkit-sunny-happy-joyful-312.mp3');
        backgroundMusic.loop = true;
        backgroundMusic.volume = 0.3;
        let isMusicPlaying = false;

        document.addEventListener('DOMContentLoaded', function() {
            const musicToggle = document.getElementById('musicToggle');
            const volumeControl = document.getElementById('volumeControl');
            const volumeSlider = document.getElementById('volumeSlider');
            
            // رویداد کلیک برای پخش/توقف موسیقی
            musicToggle.addEventListener('click', function(e) {
                e.stopPropagation();
                toggleMusic();
            });
            
            // کنترل صدا
            volumeSlider.addEventListener('input', function(e) {
                backgroundMusic.volume = e.target.value;
            });
            
            // نمایش/مخفی کردن کنترل صدا
            musicToggle.addEventListener('mouseenter', function() {
                volumeControl.style.opacity = '1';
                volumeControl.style.width = '180px';
            });
            
            volumeControl.addEventListener('mouseleave', function(e) {
                if (!e.relatedTarget || !e.relatedTarget.closest('.music-player')) {
                    volumeControl.style.opacity = '0';
                    volumeControl.style.width = '0';
                }
            });
        });

        function toggleMusic() {
            const musicToggle = document.getElementById('musicToggle');
            
            if (isMusicPlaying) {
                backgroundMusic.pause();
                musicToggle.classList.remove('playing');
                musicToggle.innerHTML = '<i class="fas fa-music"></i>';
                isMusicPlaying = false;
            } else {
                backgroundMusic.play().then(() => {
                    isMusicPlaying = true;
                    musicToggle.classList.add('playing');
                    musicToggle.innerHTML = '<i class="fas fa-pause"></i>';
                }).catch(error => {
                    console.log('خطا در پخش موسیقی:', error);
                    // درخواست اجازه از کاربر
                    if (confirm('برای پخش موسیقی نیاز به اجازه شماست. آیا اجازه می‌دهید؟')) {
                        document.body.addEventListener('click', function playOnClick() {
                            backgroundMusic.play().then(() => {
                                isMusicPlaying = true;
                                musicToggle.classList.add('playing');
                                musicToggle.innerHTML = '<i class="fas fa-pause"></i>';
                            });
                            document.body.removeEventListener('click', playOnClick);
                        }, { once: true });
                    }
                });
            }
        }

        // ========== توابع عمومی ==========
        function openLogin() {
            document.getElementById('loginModal').style.display = 'block';
            document.body.style.overflow = 'hidden';
        }

        function openRegister() {
            document.getElementById('registerModal').style.display = 'block';
            document.body.style.overflow = 'hidden';
        }

        function openAddProduct() {
            // ریست فرم
            uploadedImages = [];
            selectedColors = [];
            document.getElementById('addProductForm').reset();
            document.getElementById('uploadedImages').innerHTML = '';
            document.getElementById('selectedColors').innerHTML = '';
            
            document.getElementById('addProductModal').style.display = 'block';
            document.body.style.overflow = 'hidden';
            
            // فعال کردن آپلود عکس
            setupImageUpload();
        }

        function closeModals() {
            const modals = document.querySelectorAll('.modal');
            modals.forEach(modal => {
                modal.style.display = 'none';
            });
            document.body.style.overflow = 'auto';
        }

        function toggleAdminPanel() {
            const panel = document.getElementById('adminPanel');
            panel.style.display = panel.style.display === 'block' ? 'none' : 'block';
            if (panel.style.display === 'block') {
                displayProducts();
            }
        }

        // ========== سیستم آپلود عکس ==========
        function setupImageUpload() {
            const uploadArea = document.getElementById('uploadArea');
            const imageUpload = document.getElementById('imageUpload');
            const uploadedImagesContainer = document.getElementById('uploadedImages');
            
            // اجازه انتخاب چند فایل
            imageUpload.setAttribute('multiple', 'multiple');
            
            // کلیک روی آپلود اریا
            uploadArea.addEventListener('click', () => {
                imageUpload.click();
            });
            
            // Drag and Drop
            uploadArea.addEventListener('dragover', (e) => {
                e.preventDefault();
                uploadArea.style.borderColor = 'var(--success)';
                uploadArea.style.background = '#e8f5e9';
            });
            
            uploadArea.addEventListener('dragleave', () => {
                uploadArea.style.borderColor = 'var(--gray-light)';
                uploadArea.style.background = 'rgba(231, 76, 60, 0.02)';
            });
            
            uploadArea.addEventListener('drop', (e) => {
                e.preventDefault();
                uploadArea.style.borderColor = 'var(--gray-light)';
                uploadArea.style.background = 'rgba(231, 76, 60, 0.02)';
                const files = Array.from(e.dataTransfer.files);
                handleImageFiles(files);
            });
            
            // انتخاب فایل
            imageUpload.addEventListener('change', (e) => {
                const files = Array.from(e.target.files);
                handleImageFiles(files);
            });
            
            function handleImageFiles(files) {
                files.forEach(file => {
                    if (!file.type.startsWith('image/')) {
                        alert('فقط فایل‌های تصویری مجاز هستند');
                        return;
                    }
                    
                    const reader = new FileReader();
                    reader.onload = function(e) {
                        const imageData = e.target.result;
                        uploadedImages.push(imageData);
                        displayUploadedImages();
                    };
                    reader.readAsDataURL(file);
                });
            }
            
            function displayUploadedImages() {
                uploadedImagesContainer.innerHTML = '';
                uploadedImages.forEach((imageData, index) => {
                    const imgDiv = document.createElement('div');
                    imgDiv.style.position = 'relative';
                    imgDiv.style.width = '100px';
                    imgDiv.style.height = '100px';
                    imgDiv.style.borderRadius = '8px';
                    imgDiv.style.overflow = 'hidden';
                    imgDiv.style.border = '2px solid #eee';
                    imgDiv.innerHTML = `
                        <img src="${imageData}" alt="تصویر ${index + 1}" style="width: 100%; height: 100%; object-fit: cover;">
                        <button onclick="removeImage(${index})" style="position: absolute; top: 5px; left: 5px; background: rgba(220, 53, 69, 0.9); color: white; border: none; border-radius: 50%; width: 24px; height: 24px; cursor: pointer; display: flex; align-items: center; justify-content: center; font-size: 0.8rem;">
                            <i class="fas fa-times"></i>
                        </button>
                    `;
                    uploadedImagesContainer.appendChild(imgDiv);
                });
            }
        }

        function removeImage(index) {
            uploadedImages.splice(index, 1);
            const uploadedImagesContainer = document.getElementById('uploadedImages');
            uploadedImagesContainer.innerHTML = '';
            uploadedImages.forEach((imageData, i) => {
                const imgDiv = document.createElement('div');
                imgDiv.style.position = 'relative';
                imgDiv.style.width = '100px';
                imgDiv.style.height = '100px';
                imgDiv.style.borderRadius = '8px';
                imgDiv.style.overflow = 'hidden';
                imgDiv.style.border = '2px solid #eee';
                imgDiv.innerHTML = `
                    <img src="${imageData}" alt="تصویر ${i + 1}" style="width: 100%; height: 100%; object-fit: cover;">
                    <button onclick="removeImage(${i})" style="position: absolute; top: 5px; left: 5px; background: rgba(220, 53, 69, 0.9); color: white; border: none; border-radius: 50%; width: 24px; height: 24px; cursor: pointer; display: flex; align-items: center; justify-content: center; font-size: 0.8rem;">
                        <i class="fas fa-times"></i>
                    </button>
                `;
                uploadedImagesContainer.appendChild(imgDiv);
            });
        }

        // ========== سیستم انتخاب رنگ ==========
        function addColor() {
            const colorName = document.getElementById('colorInput').value.trim();
            const colorValue = document.getElementById('colorPicker').value;
            
            if (!colorName) {
                alert('لطفاً نام رنگ را وارد کنید');
                return;
            }
            
            // بررسی تکراری نبودن رنگ
            if (selectedColors.some(color => color.name === colorName || color.value === colorValue)) {
                alert('این رنگ قبلاً اضافه شده است');
                return;
            }
            
            selectedColors.push({
                name: colorName,
                value: colorValue
            });
            
            displaySelectedColors();
            
            // ریست فیلدها
            document.getElementById('colorInput').value = '';
            document.getElementById('colorPicker').value = '#000000';
        }

        function displaySelectedColors() {
            const container = document.getElementById('selectedColors');
            container.innerHTML = '';
            
            selectedColors.forEach((color, index) => {
                const colorItem = document.createElement('div');
                colorItem.style.display = 'flex';
                colorItem.style.alignItems = 'center';
                colorItem.style.gap = '0.5rem';
                colorItem.style.background = '#f8f9fa';
                colorItem.style.padding = '0.3rem 0.8rem';
                colorItem.style.borderRadius = '20px';
                colorItem.style.fontSize = '0.9rem';
                colorItem.innerHTML = `
                    <div style="width: 20px; height: 20px; border-radius: 50%; background-color: ${color.value}; border: 2px solid #fff; box-shadow: 0 2px 4px rgba(0,0,0,0.1);"></div>
                    <span>${color.name}</span>
                    <button onclick="removeColor(${index})" style="background: none; border: none; color: var(--danger); cursor: pointer; font-size: 0.8rem; padding: 0 0.3rem;">
                        <i class="fas fa-times"></i>
                    </button>
                `;
                container.appendChild(colorItem);
            });
        }

        function removeColor(index) {
            selectedColors.splice(index, 1);
            displaySelectedColors();
        }

        // ========== سیستم تماس ==========
        function sendWhatsAppMessage() {
            const phoneNumber = "989129573096";
            const message = "سلام! 👋\nمی‌خواهم از بوتیک موناکو خرید کنم.\nلطفاً راهنمایی ام کنید.";
            const url = `https://wa.me/${phoneNumber}?text=${encodeURIComponent(message)}`;
            window.open(url, '_blank');
        }

        function sendTelegramMessage() {
            const phoneNumber = "989129573096";
            const message = "سلام! 👋\nمی‌خواهم از بوتیک موناکو خرید کنم.\nلطفاً راهنمایی ام کنید.";
            const url = `https://t.me/+${phoneNumber}?text=${encodeURIComponent(message)}`;
            window.open(url, '_blank');
        }

        function showBuyGuide() {
            alert("🛍️ راهنمای خرید از بوتیک موناکو:\n\n" +
                  "1️⃣ محصول مورد نظر خود را انتخاب کنید\n" +
                  "2️⃣ روی دکمه 'واتس‌اپ' یا 'تلگرام' کلیک کنید\n" +
                  "3️⃣ پیام پیش‌فرض را ارسال کنید\n" +
                  "4️⃣ کارشناسان ما با شما تماس خواهند گرفت\n\n" +
                  "📞 شماره تماس: ۰۹۱۲۹۵۷۳۰۹۶\n" +
                  "💬 واتس‌اپ: همین شماره\n" +
                  "📱 تلگرام: همین شماره");
        }

        function showContactInfo() {
            alert("📞 اطلاعات تماس بوتیک موناکو:\n\n" +
                  "شماره تماس: ۰۹۱۲۹۵۷۳۰۹۶\n" +
                  "واتس‌اپ: همین شماره\n" +
                  "تلگرام: همین شماره\n\n" +
                  "ساعات پاسخگویی:\n" +
                  "📅 همه روزه\n" +
                  "⏰ ۹ صبح تا ۹ شب");
        }

        // ========== سیستم همگام‌سازی ==========
        function exportProducts() {
            if (!currentUser || !currentUser.isAdmin) {
                alert("❌ فقط مدیر سیستم می‌تواند از محصولات خروجی بگیرد!");
                return;
            }
            
            if (products.length === 0) {
                alert("❌ محصولی برای خروجی گرفتن وجود ندارد!");
                return;
            }
            
            try {
                const dataStr = JSON.stringify(products, null, 2);
                const dataBlob = new Blob([dataStr], {type: 'application/json'});
                const link = document.createElement('a');
                link.href = URL.createObjectURL(dataBlob);
                link.download = 'monaco_products.json';
                document.body.appendChild(link);
                link.click();
                document.body.removeChild(link);
                URL.revokeObjectURL(link.href);
                
                alert('✅ فایل محصولات با موفقیت دانلود شد!');
            } catch (error) {
                console.error('خطا در خروجی گرفتن:', error);
                alert('❌ خطا در خروجی گرفتن از محصولات!');
            }
        }

        // ========== سیستم تخفیف دستی ==========
        function openDiscountModal(productId) {
            const product = products.find(p => p.id === productId);
            if (!product) return;

            const container = document.getElementById('discountFormContainer');
            container.innerHTML = `
                <h3 style="margin-bottom: 1rem; color: var(--secondary);">${product.name}</h3>
                <div style="margin-bottom: 1.5rem; padding: 1rem; background: #f8f9fa; border-radius: 10px;">
                    <div style="display: flex; justify-content: space-between; margin-bottom: 0.5rem;">
                        <span>قیمت اصلی:</span>
                        <span style="font-weight: bold;">${product.price.toLocaleString()} تومان</span>
                    </div>
                    ${product.discount?.hasDiscount ? `
                    <div style="display: flex; justify-content: space-between; color: var(--success);">
                        <span>قیمت با تخفیف:</span>
                        <span style="font-weight: bold;">${product.discount.discountedPrice.toLocaleString()} تومان</span>
                    </div>
                    ` : ''}
                </div>
                
                <form id="discountForm" class="modal-form">
                    <div class="form-group">
                        <label class="form-label">آیا تخفیف دارد؟</label>
                        <select id="hasDiscount" class="form-control">
                            <option value="false" ${!product.discount?.hasDiscount ? 'selected' : ''}>خیر</option>
                            <option value="true" ${product.discount?.hasDiscount ? 'selected' : ''}>بله</option>
                        </select>
                    </div>
                    
                    <div id="discountFields" style="${!product.discount?.hasDiscount ? 'display: none;' : ''} margin-top: 1rem;">
                        <div class="form-group">
                            <label class="form-label">دلیل تخفیف</label>
                            <input type="text" id="discountReason" class="form-control" value="${product.discount?.reason || ''}" placeholder="مثال: شگفت‌انگیز، فصلی، ویژه، حراج">
                        </div>
                        <div class="form-group">
                            <label class="form-label">قیمت پس از تخفیف (تومان)</label>
                            <input type="number" id="discountedPrice" class="form-control" value="${product.discount?.discountedPrice || product.price}" min="1000" max="${product.price}" placeholder="${product.price}">
                            <small style="color: #666; display: block; margin-top: 0.3rem;">
                                قیمت باید کمتر از ${product.price.toLocaleString()} تومان باشد
                            </small>
                        </div>
                    </div>
                    
                    <div style="display: flex; gap: 0.5rem; margin-top: 1.5rem;">
                        <button type="button" class="btn btn-success" style="flex: 1;" onclick="saveDiscount(${productId})">
                            <i class="fas fa-save"></i> ذخیره
                        </button>
                        <button type="button" class="btn btn-secondary" style="flex: 1;" onclick="closeModals()">
                            <i class="fas fa-times"></i> انصراف
                        </button>
                    </div>
                </form>
            `;

            document.getElementById('hasDiscount').addEventListener('change', function() {
                const discountFields = document.getElementById('discountFields');
                discountFields.style.display = this.value === 'true' ? 'block' : 'none';
            });

            document.getElementById('discountModal').style.display = 'block';
            document.body.style.overflow = 'hidden';
        }

        function saveDiscount(productId) {
            const product = products.find(p => p.id === productId);
            if (!product) return;

            const hasDiscount = document.getElementById('hasDiscount').value === 'true';
            
            if (hasDiscount) {
                const reason = document.getElementById('discountReason').value.trim();
                const discountedPrice = parseInt(document.getElementById('discountedPrice').value);
                
                if (!reason) {
                    alert("❌ لطفاً دلیل تخفیف را وارد کنید");
                    return;
                }
                
                if (!discountedPrice || discountedPrice <= 0) {
                    alert("❌ لطفاً قیمت پس از تخفیف را وارد کنید");
                    return;
                }
                
                if (discountedPrice >= product.price) {
                    alert(`❌ قیمت پس از تخفیف باید کمتر از ${product.price.toLocaleString()} تومان باشد`);
                    return;
                }

                product.discount = {
                    hasDiscount: true,
                    reason: reason,
                    discountedPrice: discountedPrice
                };
            } else {
                product.discount = {
                    hasDiscount: false,
                    reason: "",
                    discountedPrice: 0
                };
            }

            localStorage.setItem('monaco_products', JSON.stringify(products));
            displayProducts();
            closeModals();
            alert("✅ تخفیف با موفقیت ذخیره شد!");
        }

        // ========== سیستم نمایش محصولات ==========
        function displayProducts() {
            const productGrid = document.getElementById('productGrid');
            const adminProductGrid = document.getElementById('adminProductGrid');
            
            if (products.length === 0) {
                productGrid.innerHTML = `
                    <div style="text-align: center; padding: 3rem 1rem; grid-column: 1 / -1;">
                        <i class="fas fa-tshirt" style="font-size: 4rem; color: #ddd; margin-bottom: 1rem;"></i>
                        <h3 style="color: var(--secondary);">هنوز محصولی وجود ندارد</h3>
                        <p style="color: var(--gray); margin-top: 0.5rem;">برای افزودن محصول وارد پنل مدیریت شوید</p>
                    </div>
                `;
                
                adminProductGrid.innerHTML = `
                    <div style="text-align: center; padding: 3rem 1rem;">
                        <i class="fas fa-box-open" style="font-size: 4rem; color: #ddd; margin-bottom: 1rem;"></i>
                        <h3 style="color: var(--secondary);">محصولی برای مدیریت وجود ندارد</h3>
                        <p style="color: var(--gray); margin-top: 0.5rem;">برای شروع، اولین محصول خود را اضافه کنید</p>
                    </div>
                `;
                return;
            }
            
            // نمایش برای کاربران عادی
            productGrid.innerHTML = '';
            products.forEach(product => {
                const productCard = document.createElement('div');
                productCard.className = 'product-card';
                
                let priceHTML = '';
                if (product.discount?.hasDiscount && product.discount.discountedPrice > 0) {
                    const discountPercent = Math.round((1 - product.discount.discountedPrice / product.price) * 100);
                    priceHTML = `
                        <div class="price-container">
                            <div class="current-price">${product.discount.discountedPrice.toLocaleString()} تومان</div>
                            <div class="original-price">${product.price.toLocaleString()} تومان</div>
                            <div class="discount-percentage">${discountPercent}% تخفیف</div>
                        </div>
                    `;
                } else {
                    priceHTML = `
                        <div class="price-container">
                            <div class="current-price">${product.price.toLocaleString()} تومان</div>
                        </div>
                    `;
                }
                
                productCard.innerHTML = `
                    ${product.discount?.hasDiscount ? '<div class="product-badge sale">تخفیف ویژه</div>' : '<div class="product-badge new">جدید</div>'}
                    <div class="product-image-container">
                        <img src="${product.images?.[0] || 'https://via.placeholder.com/400x300/eee/666?text=محصول+موناکو'}" 
                             alt="${product.name}" class="product-image">
                    </div>
                    <div class="product-info">
                        <h3 class="product-title">${product.name}</h3>
                        <p class="product-description">${product.description || 'محصولی شیک و با کیفیت از مجموعه موناکو'}</p>
                        ${priceHTML}
                        ${product.colors && product.colors.length > 0 ? `
                        <div class="product-colors">
                            ${product.colors.map(color => `
                                <div class="color-option" style="background-color: ${color.value || color};" title="${color.name || color}"></div>
                            `).join('')}
                        </div>
                        ` : ''}
                        <div class="product-actions">
                            <button class="btn btn-primary" onclick="showProductDetails(${product.id})">
                                <i class="fas fa-eye"></i> مشاهده
                            </button>
                            <button class="btn btn-whatsapp" onclick="event.stopPropagation(); sendWhatsAppMessage()">
                                <i class="fab fa-whatsapp"></i> خرید
                            </button>
                        </div>
                    </div>
                `;
                productGrid.appendChild(productCard);
            });
            
            // نمایش برای ادمین
            adminProductGrid.innerHTML = '<h3 style="margin-bottom: 1rem; color: var(--secondary);">محصولات برای مدیریت:</h3>';
            const adminGrid = document.createElement('div');
            adminGrid.className = 'product-grid';
            adminProductGrid.appendChild(adminGrid);
            
            products.forEach(product => {
                const productCard = document.createElement('div');
                productCard.className = 'product-card';
                
                let priceHTML = '';
                if (product.discount?.hasDiscount && product.discount.discountedPrice > 0) {
                    priceHTML = `
                        <div class="price-container">
                            <div class="current-price">${product.discount.discountedPrice.toLocaleString()} تومان</div>
                            <div class="original-price">${product.price.toLocaleString()} تومان</div>
                            <small style="color: var(--success); font-weight: 600;">${product.discount.reason}</small>
                        </div>
                    `;
                } else {
                    priceHTML = `
                        <div class="price-container">
                            <div class="current-price">${product.price.toLocaleString()} تومان</div>
                        </div>
                    `;
                }
                
                productCard.innerHTML = `
                    <div class="product-image-container">
                        <img src="${product.images?.[0] || 'https://via.placeholder.com/400x300'}" 
                             alt="${product.name}" class="product-image">
                    </div>
                    <div class="product-info">
                        <h3 class="product-title">${product.name}</h3>
                        ${priceHTML}
                        <div class="product-actions">
                            <button class="btn btn-primary" onclick="showProductDetails(${product.id})">
                                <i class="fas fa-eye"></i> مشاهده
                            </button>
                            <button class="btn btn-warning" onclick="openDiscountModal(${product.id})">
                                <i class="fas fa-percentage"></i> تخفیف
                            </button>
                            <button class="btn btn-danger" onclick="deleteProduct(${product.id})">
                                <i class="fas fa-trash"></i> حذف
                            </button>
                        </div>
                    </div>
                `;
                adminGrid.appendChild(productCard);
            });
        }

        // ========== فرم افزودن محصول ==========
        document.getElementById('addProductForm').addEventListener('submit', function(event) {
            event.preventDefault();
            
            const name = document.getElementById('productName').value.trim();
            const price = parseInt(document.getElementById('productPrice').value);
            const size = document.getElementById('productSize').value.trim();
            const description = document.getElementById('productDescription').value.trim();
            
            if (!name || !price) {
                alert("❌ لطفاً نام و قیمت محصول را وارد کنید");
                return;
            }
            
            if (uploadedImages.length === 0) {
                alert("❌ لطفاً حداقل یک عکس برای محصول آپلود کنید");
                return;
            }
            
            const newProduct = {
                id: Date.now(),
                name: name,
                price: price,
                images: uploadedImages,
                colors: selectedColors,
                size: size,
                description: description,
                discount: {
                    hasDiscount: false,
                    reason: "",
                    discountedPrice: 0
                }
            };
            
            products.push(newProduct);
            localStorage.setItem('monaco_products', JSON.stringify(products));
            
            displayProducts();
            alert("✅ محصول با موفقیت اضافه شد!");
            closeModals();
            
            // ریست فرم
            uploadedImages = [];
            selectedColors = [];
            document.getElementById('addProductForm').reset();
            document.getElementById('uploadedImages').innerHTML = '';
            document.getElementById('selectedColors').innerHTML = '';
        });

        // ========== سیستم نمایش جزئیات محصول ==========
        function showProductDetails(productId) {
            const product = products.find(p => p.id === productId);
            if (!product) return;

            alert(`📋 جزئیات محصول:\n\n` +
                  `🏷️ نام: ${product.name}\n` +
                  `💰 قیمت: ${product.price.toLocaleString()} تومان\n` +
                  (product.discount?.hasDiscount ? 
                  `🎯 قیمت با تخفیف: ${product.discount.discountedPrice.toLocaleString()} تومان\n` +
                  `📝 دلیل تخفیف: ${product.discount.reason}\n` : '') +
                  (product.size ? `📏 سایزهای موجود: ${product.size}\n` : '') +
                  (product.description ? `📖 توضیحات: ${product.description}\n` : '') +
                  `\nبرای خرید این محصول از دکمه‌های واتس‌اپ یا تلگرام استفاده کنید.`);
        }

        // ========== مدیریت محصولات ==========
        function deleteProduct(productId) {
            if (confirm('آیا از حذف این محصول اطمینان دارید؟')) {
                products = products.filter(product => product.id !== productId);
                localStorage.setItem('monaco_products', JSON.stringify(products));
                displayProducts();
                alert("✅ محصول با موفقیت حذف شد!");
            }
        }

        // ========== سیستم کاربران ==========
        document.getElementById('loginForm').addEventListener('submit', function(event) {
            event.preventDefault();
            const email = document.getElementById('loginEmail').value.trim();
            const password = document.getElementById('loginPassword').value;
            
            // مدیر سیستم
            if (email === "admin_shaian@gmail.com" && password === "shaian_112233") {
                currentUser = { name: 'مدیر سیستم', email: email, isAdmin: true };
                localStorage.setItem('current_user', JSON.stringify(currentUser));
                updateUI();
                displayProducts();
                alert("👑 خوش آمدید مدیر!");
                closeModals();
                return;
            }
            
            // کاربر عادی
            const user = users.find(u => u.email === email && u.password === password);
            if (user) {
                currentUser = user;
                localStorage.setItem('current_user', JSON.stringify(currentUser));
                updateUI();
                displayProducts();
                alert(`🎉 خوش آمدید ${user.name}!`);
                closeModals();
            } else {
                alert("❌ ایمیل یا رمز عبور اشتباه است!");
            }
        });

        document.getElementById('registerForm').addEventListener('submit', function(event) {
            event.preventDefault();
            const name = document.getElementById('registerName').value.trim();
            const email = document.getElementById('registerEmail').value.trim();
            const password = document.getElementById('registerPassword').value;
            
            if (users.find(u => u.email === email)) {
                alert("❌ این ایمیل قبلاً ثبت‌نام شده است!");
                return;
            }
            
            if (password.length < 6) {
                alert("❌ رمز عبور باید حداقل ۶ کاراکتر باشد!");
                return;
            }
            
            const newUser = { id: Date.now(), name, email, password };
            users.push(newUser);
            localStorage.setItem('monaco_users', JSON.stringify(users));
            
            currentUser = newUser;
            localStorage.setItem('current_user', JSON.stringify(currentUser));
            updateUI();
            
            alert(`✅ ثبت‌نام موفقیت آمیز!\nخوش آمدید ${name}`);
            closeModals();
        });

        function logout() {
            currentUser = null;
            localStorage.removeItem('current_user');
            updateUI();
            displayProducts();
            alert("👋 با موفقیت خارج شدید!");
        }

        function updateUI() {
            const loginBtn = document.querySelector('.btn-secondary[onclick="openLogin()"]');
            const registerBtn = document.querySelector('.btn-primary[onclick="openRegister()"]');
            const adminBtn = document.getElementById('adminBtn');
            const logoutBtn = document.getElementById('logoutBtn');
            const adminPanel = document.getElementById('adminPanel');

            if (currentUser) {
                loginBtn.style.display = 'none';
                registerBtn.style.display = 'none';
                logoutBtn.style.display = 'block';
                
                if (currentUser.isAdmin) {
                    adminBtn.style.display = 'block';
                    adminPanel.style.display = 'block';
                } else {
                    adminBtn.style.display = 'none';
                    adminPanel.style.display = 'none';
                }
            } else {
                loginBtn.style.display = 'block';
                registerBtn.style.display = 'block';
                adminBtn.style.display = 'none';
                logoutBtn.style.display = 'none';
                adminPanel.style.display = 'none';
            }
        }

        // ========== مدیریت رخدادها ==========
        window.onclick = function(event) {
            const modals = document.querySelectorAll('.modal');
            modals.forEach(modal => {
                if (event.target === modal) {
                    modal.style.display = 'none';
                    document.body.style.overflow = 'auto';
                }
            });
        };

        // ========== راه‌اندازی اولیه ==========
        document.addEventListener('DOMContentLoaded', function() {
            updateUI();
            displayProducts();
        });
    </script>
</body>
</html>
