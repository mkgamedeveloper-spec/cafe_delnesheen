
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
   
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Vazirmatn:wght@300;400;500;600;700;800&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Vazirmatn', sans-serif;
            background: linear-gradient(135deg, #FFD93D 0%, #FF6B9D 50%, #C2FFD9 100%);
            min-height: 100vh;
            padding: 40px 20px;
            animation: gradientShift 10s ease infinite;
            background-size: 200% 200%;
        }
        
        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        .container {
            max-width: 900px;
            margin: 0 auto;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(15px);
            border-radius: 40px;
            padding: 50px;
            box-shadow: 0 30px 80px rgba(0, 0, 0, 0.2);
            border: 3px solid rgba(255, 255, 255, 0.8);
        }
        
        .header {
            text-align: center;
            margin-bottom: 50px;
            padding-bottom: 30px;
            border-bottom: 3px dashed #FF6B9D;
            position: relative;
        }
        
        .coffee-icon {
            font-size: 60px;
            animation: bounce 2s ease-in-out infinite;
            display: inline-block;
            margin-bottom: 10px;
        }
        
        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-15px); }
        }
        
        .logo {
            font-size: 56px;
            font-weight: 800;
            background: linear-gradient(135deg, #FF6B9D, #FFA500, #FF6B9D);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 10px;
            letter-spacing: 1px;
            animation: colorShift 3s ease infinite;
        }
        
        @keyframes colorShift {
            0%, 100% { filter: hue-rotate(0deg); }
            50% { filter: hue-rotate(20deg); }
        }
        
        .tagline {
            font-size: 18px;
            color: #666;
            font-weight: 400;
            letter-spacing: 2px;
        }
        
        .section {
            margin-bottom: 45px;
        }
        
        .section-header {
            background: linear-gradient(135deg, #FF6B9D, #FFA500);
            padding: 20px 30px;
            border-radius: 20px;
            margin-bottom: 25px;
            box-shadow: 0 8px 20px rgba(255, 107, 157, 0.3);
            transform: rotate(-1deg);
            transition: transform 0.3s ease;
        }
        
        .section-header:hover {
            transform: rotate(0deg) scale(1.02);
        }
        
        .section-title {
            font-size: 32px;
            font-weight: 700;
            color: white;
            text-align: center;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
        }
        
        .menu-item {
            background: linear-gradient(135deg, #FFF9E6 0%, #FFE6F0 100%);
            padding: 25px;
            margin-bottom: 15px;
            border-radius: 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            transition: all 0.3s ease;
            border: 2px solid transparent;
            position: relative;
            overflow: hidden;
        }
        
        .menu-item:before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.5), transparent);
            transition: left 0.5s ease;
        }
        
        .menu-item:hover {
            transform: translateX(-5px) scale(1.02);
            border-color: #FF6B9D;
            box-shadow: 0 10px 30px rgba(255, 107, 157, 0.3);
        }
        
        .menu-item:hover:before {
            left: 100%;
        }
        
        .item-info {
            flex: 1;
        }
        
        .item-name {
            font-size: 22px;
            font-weight: 600;
            color: #333;
            margin-bottom: 8px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .item-emoji {
            font-size: 26px;
        }
        
        .item-description {
            font-size: 15px;
            color: #666;
            font-weight: 400;
        }
        
        .item-price {
            font-size: 26px;
            font-weight: 700;
            background: linear-gradient(135deg, #FF6B9D, #FFA500);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-right: 20px;
            min-width: 120px;
            text-align: left;
        }
        
        .price-unit {
            font-size: 14px;
            font-weight: 500;
        }
        
        .decorative-line {
            height: 30px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 30px 0;
            gap: 15px;
            font-size: 24px;
        }
        
        .footer {
            text-align: center;
            margin-top: 40px;
            padding-top: 30px;
            border-top: 3px dashed #FF6B9D;
            color: #666;
            font-size: 16px;
        }
        
        @media (max-width: 768px) {
            .container {
                padding: 30px 20px;
            }
            
            .logo {
                font-size: 42px;
            }
            
            .section-title {
                font-size: 26px;
            }
            
            .menu-item {
                flex-direction: column;
                align-items: flex-start;
                padding: 20px;
            }
            
            .item-price {
                margin-right: 0;
                margin-top: 10px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="coffee-icon">☕</div>
            <div class="logo">کافه دلنشین</div>
            <div class="tagline">جایی برای لبخند و لذت</div>
        </div>
        
        <div class="section">
            <div class="section-header">
                <h2 class="section-title">🔥 نوشیدنی‌های گرم</h2>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">
                        <span class="item-emoji">☕</span>
                        اسپرسو
                    </div>
                    <div class="item-description">قهوه تلخ و خوشمزه با دانه‌های تازه</div>
                </div>
                <div class="item-price">۴۵,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">
                        <span class="item-emoji">☕</span>
                        کاپوچینو
                    </div>
                    <div class="item-description">اسپرسو با شیر گرم و فوم خامه‌ای</div>
                </div>
                <div class="item-price">۶۵,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">
                        <span class="item-emoji">🥛</span>
                        لاته
                    </div>
                    <div class="item-description">قهوه ملایم با شیر داغ</div>
                </div>
                <div class="item-price">۷۰,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">
                        <span class="item-emoji">🍫</span>
                        موکا
                    </div>
                    <div class="item-description">قهوه با شکلات و شیر خوشمزه</div>
                </div>
                <div class="item-price">۷۵,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">
                        <span class="item-emoji">🍫</span>
                        هات چاکلت
                    </div>
                    <div class="item-description">شکلات داغ با خامه و مارشمالو</div>
                </div>
                <div class="item-price">۶۸,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">
                        <span class="item-emoji">🍵</span>
                        چای ماسالا
                    </div>
                    <div class="item-description">چای معطر با ادویه و شیر</div>
                </div>
                <div class="item-price">۵۵,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
        </div>
        
        <div class="decorative-line">
            <span>🌸</span>
            <span>☀️</span>
            <span>🌈</span>
            <span>⭐</span>
        </div>
        
        <div class="section">
            <div class="section-header">
                <h2 class="section-title">❄️ نوشیدنی‌های سرد</h2>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">
                        <span class="item-emoji">🧊</span>
                        آیس آمریکانو
                    </div>
                    <div class="item-description">قهوه سرد با یخ خرد شده</div>
                </div>
                <div class="item-price">۶۰,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">
                        <span class="item-emoji">🥤</span>
                        آیس لاته
                    </div>
                    <div class="item-description">قهوه با شیر سرد و یخ</div>
                </div>
                <div class="item-price">۷۵,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">
                        <span class="item-emoji">🍮</span>
                        فرپوچینو کارامل
                    </div>
                    <div class="item-description">نوشیدنی یخ زده با کارامل و خامه</div>
                </div>
                <div class="item-price">۸۵,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">
                        <span class="item-emoji">🌿</span>
                        موهیتو
                    </div>
                    <div class="item-description">نعناع تازه، لیمو و سودا</div>
                </div>
                <div class="item-price">۶۵,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">
                        <span class="item-emoji">🍓</span>
                        اسموتی توت فرنگی
                    </div>
                    <div class="item-description">توت فرنگی تازه با ماست و عسل</div>
                </div>
                <div class="item-price">۷۰,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">
                        <span class="item-emoji">🍋</span>
                        لیموناد خانگی
                    </div>
                    <div class="item-description">آب لیمو تازه با نعناع</div>
                </div>
                <div class="item-price">۵۰,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">
                        <span class="item-emoji">🍦</span>
                        شیک شکلاتی
                    </div>
                    <div class="item-description">بستنی با شکلات و شیر</div>
                </div>
                <div class="item-price">۸۰,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
        </div>
        
        <div class="footer">
            💝 با عشق در کافه دلنشین آماده شده 💝
        </div>
    </div>
</body>
</html>
