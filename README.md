<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>منوی کافه</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Vazirmatn:wght@300;400;500;600;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Vazirmatn', sans-serif;
            background: linear-gradient(135deg, #1a1a1a 0%, #2d1810 100%);
            color: #fff;
            min-height: 100vh;
            padding: 40px 20px;
        }
        
        .container {
            max-width: 900px;
            margin: 0 auto;
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(10px);
            border-radius: 30px;
            padding: 50px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.5);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .header {
            text-align: center;
            margin-bottom: 60px;
            padding-bottom: 30px;
            border-bottom: 2px solid rgba(218, 165, 32, 0.3);
        }
        
        .logo {
            font-size: 48px;
            font-weight: 700;
            background: linear-gradient(135deg, #DAA520, #FFD700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 10px;
            letter-spacing: 2px;
        }
        
        .tagline {
            font-size: 16px;
            color: #bbb;
            font-weight: 300;
            letter-spacing: 3px;
        }
        
        .section {
            margin-bottom: 50px;
        }
        
        .section-title {
            font-size: 32px;
            font-weight: 600;
            color: #DAA520;
            margin-bottom: 30px;
            position: relative;
            padding-right: 20px;
        }
        
        .section-title:before {
            content: '';
            position: absolute;
            right: 0;
            top: 50%;
            transform: translateY(-50%);
            width: 6px;
            height: 6px;
            background: #DAA520;
            border-radius: 50%;
        }
        
        .menu-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
            transition: all 0.3s ease;
        }
        
        .menu-item:hover {
            padding-right: 10px;
            border-bottom-color: rgba(218, 165, 32, 0.3);
        }
        
        .item-info {
            flex: 1;
        }
        
        .item-name {
            font-size: 20px;
            font-weight: 500;
            color: #fff;
            margin-bottom: 8px;
        }
        
        .item-description {
            font-size: 14px;
            color: #999;
            font-weight: 300;
        }
        
        .item-price {
            font-size: 22px;
            font-weight: 600;
            color: #DAA520;
            margin-right: 30px;
        }
        
        .price-unit {
            font-size: 14px;
            font-weight: 400;
        }
        
        .divider {
            height: 2px;
            background: linear-gradient(90deg, transparent, rgba(218, 165, 32, 0.3), transparent);
            margin: 40px 0;
        }
        
        @media (max-width: 768px) {
            .container {
                padding: 30px 20px;
            }
            
            .logo {
                font-size: 36px;
            }
            
            .section-title {
                font-size: 26px;
            }
            
            .menu-item {
                flex-direction: column;
                align-items: flex-start;
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
            <div class="logo">☕ CAFÉ ÉLÉGANT</div>
            <div class="tagline">طعم لذت در هر جرعه</div>
        </div>
        
        <div class="section">
            <h2 class="section-title">نوشیدنی‌های گرم</h2>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">اسپرسو</div>
                    <div class="item-description">قهوه تازه دم کرده با دانه‌های برزیلی</div>
                </div>
                <div class="item-price">۴۵,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">کاپوچینو</div>
                    <div class="item-description">اسپرسو، شیر بخار شده و فوم شیر</div>
                </div>
                <div class="item-price">۶۵,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">لاته</div>
                    <div class="item-description">اسپرسو با شیر داغ و لایه‌ای از فوم</div>
                </div>
                <div class="item-price">۷۰,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">موکا</div>
                    <div class="item-description">ترکیب قهوه، شکلات و شیر داغ</div>
                </div>
                <div class="item-price">۷۵,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">هات چاکلت</div>
                    <div class="item-description">شکلات بلژیکی با شیر داغ و خامه</div>
                </div>
                <div class="item-price">۶۸,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">چای ماسالا</div>
                    <div class="item-description">چای سیاه با ادویه‌های هندی و شیر</div>
                </div>
                <div class="item-price">۵۵,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
        </div>
        
        <div class="divider"></div>
        
        <div class="section">
            <h2 class="section-title">نوشیدنی‌های سرد</h2>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">آیس آمریکانو</div>
                    <div class="item-description">اسپرسو با آب یخ و یخ خرد شده</div>
                </div>
                <div class="item-price">۶۰,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">آیس لاته</div>
                    <div class="item-description">اسپرسو، شیر سرد و یخ</div>
                </div>
                <div class="item-price">۷۵,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">فرپوچینو کارامل</div>
                    <div class="item-description">قهوه یخ زده با کارامل و خامه</div>
                </div>
                <div class="item-price">۸۵,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">موهیتو</div>
                    <div class="item-description">نعناع تازه، لیمو، سودا و یخ</div>
                </div>
                <div class="item-price">۶۵,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">اسموتی توت فرنگی</div>
                    <div class="item-description">توت فرنگی تازه، ماست و عسل</div>
                </div>
                <div class="item-price">۷۰,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">لیموناد خانگی</div>
                    <div class="item-description">آب لیمو تازه با نعناع و شکر قندی</div>
                </div>
                <div class="item-price">۵۰,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
            
            <div class="menu-item">
                <div class="item-info">
                    <div class="item-name">شیک شکلاتی</div>
                    <div class="item-description">بستنی وانیلی، شکلات و شیر</div>
                </div>
                <div class="item-price">۸۰,۰۰۰ <span class="price-unit">تومان</span></div>
            </div>
        </div>
    </div>
</body>
</html>
