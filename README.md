<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> social links</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <!-- فونت‌های فارسی از گوگل فونت -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Vazirmatn:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        /* استفاده از فونت فارسی */
        body {
            font-family: 'Vazirmatn', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #000;
            color: #fff;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 20px;
            line-height: 1.6;
        }
        
        .container {
            width: 100%;
            max-width: 500px;
            text-align: center;
        }
        
        .title {
            margin-bottom: 30px;
        }
        
        h1 {
            font-size: 28px;
            margin-bottom: 10px;
            font-weight: 700;
        }
        
        p {
            font-size: 16px;
            opacity: 0.9;
            margin-bottom: 30px;
            font-weight: 400;
            color: #ccc;
        }
        
        .links {
            display: flex;
            flex-direction: column;
            gap: 15px;
            margin-bottom: 30px;
        }
        
        .link {
            background-color: rgba(255, 255, 255, 0.05);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 12px;
            padding: 15px 20px;
            text-decoration: none;
            color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            font-weight: 500;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
            position: relative;
            overflow: hidden;
        }
        
        .link::before {
            content: '';
            position: absolute;
            top: 0;
            right: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, rgba(255,255,255,0.1), transparent);
            opacity: 0;
            transition: opacity 0.4s ease;
        }
        
        .link:hover {
            transform: translateY(-5px);
            background-color: rgba(255, 255, 255, 0.15);
            box-shadow: 
                0 12px 30px rgba(255, 255, 255, 0.2),
                0 6px 20px rgba(255, 255, 255, 0.15);
            border-color: rgba(255, 255, 255, 0.4);
        }
        
        .link:hover::before {
            opacity: 1;
        }
        
        .link-content {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 100%;
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }
        
        .link-icon {
            font-size: 24px;
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .custom-icon {
            width: 24px;
            height: 24px;
            fill: white;
        }
        
        .link-text {
            opacity: 0;
            transform: translateX(20px);
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            white-space: nowrap;
            margin-right: 10px;
            position: absolute;
            right: 50%;
            transform: translateX(20px) translateX(50%);
        }
        
        .link:hover .link-icon {
            transform: translateX(40px);
        }
        
        .link:hover .link-text {
            opacity: 1;
            transform: translateX(0) translateX(50%);
        }
        
        .instagram {
            background: linear-gradient(45deg, rgba(240, 148, 51, 0.2), rgba(230, 104, 60, 0.2), rgba(220, 39, 67, 0.2), rgba(204, 35, 102, 0.2), rgba(188, 24, 136, 0.2));
        }
        
        .instagram:hover {
            background: linear-gradient(45deg, rgba(240, 148, 51, 0.4), rgba(230, 104, 60, 0.4), rgba(220, 39, 67, 0.4), rgba(204, 35, 102, 0.4), rgba(188, 24, 136, 0.4));
        }
        
        .telegram {
            background-color: rgba(0, 136, 204, 0.2);
        }
        
        .telegram:hover {
            background-color: rgba(0, 136, 204, 0.4);
        }
        
        .eitaa {
            background-color: rgba(255, 165, 0, 0.2);
        }
        
        .eitaa:hover {
            background-color: rgba(255, 165, 0, 0.4);
        }
        
        footer {
            margin-top: 30px;
            font-size: 14px;
            opacity: 0.7;
            font-weight: 300;
            color: #999;
        }
        
        @media (max-width: 480px) {
            .container {
                padding: 0 15px;
            }
            
            h1 {
                font-size: 24px;
            }
            
            .link {
                padding: 12px 15px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="title">
            <h1>از طریق لینک های زیر با ما در ارتباط باشید</h1>
        </div>
        
        <div class="links">
            <a href="https://instagram.com/yourusername" class="link instagram" target="_blank">
                <div class="link-content">
                    <div class="link-icon">
                        <i class="fab fa-instagram"></i>
                    </div>
                    <div class="link-text">اینستاگرام</div>
                </div>
            </a>
            
            <a href="https://t.me/yourusername" class="link telegram" target="_blank">
                <div class="link-content">
                    <div class="link-icon">
                        <i class="fab fa-telegram"></i>
                    </div>
                    <div class="link-text">تلگرام</div>
                </div>
            </a>
            
            <a href="https://eitaa.com/yourusername" class="link eitaa" target="_blank">
                <div class="link-content">
                    <div class="link-icon">
                        <svg class="custom-icon" viewBox="0 0 24 24" role="img" xmlns="http://www.w3.org/2000/svg">
                            <path d="M5.968 23.942a6.624 6.624 0 0 1-2.332-.83c-1.62-.929-2.829-2.593-3.217-4.426-.151-.717-.17-1.623-.15-7.207C.288 5.47.274 5.78.56 4.79c.142-.493.537-1.34.823-1.767C2.438 1.453 3.99.445 5.913.08c.384-.073.94-.08 6.056-.08 6.251 0 6.045-.009 7.066.314a6.807 6.807 0 0 1 4.314 4.184c.33.937.346 1.087.369 3.555l.02 2.23-.391.268c-.558.381-1.29 1.06-2.316 2.15-1.182 1.256-2.376 2.42-2.982 2.907-1.309 1.051-2.508 1.651-3.726 1.864-.634.11-1.682.067-2.302-.095-.553-.144-.517-.168-.726.464a6.355 6.355 0 0 0-.318 1.546l-.031.407-.146-.03c-1.215-.241-2.419-1.285-2.884-2.5a3.583 3.583 0 0 1-.26-1.219l-.016-.34-.309-.284c-.644-.59-1.063-1.312-1.195-2.061-.212-1.193.34-2.542 1.538-3.756 1.264-1.283 3.127-2.29 4.953-2.68.658-.14 1.818-.177 2.403-.075 1.138.198 2.067.773 2.645 1.639.182.271.195.311.177.555a.812.812 0 0 1-.183.493c-.465.651-1.848 1.348-3.336 1.68-2.625.585-4.294-.142-4.033-1.759.026-.163.04-.304.031-.313-.032-.032-.293.104-.575.3-.479.334-.903.984-1.05 1.607-.036.156-.05.406-.034.65.02.331.053.454.192.736.092.186.275.45.408.589l.24.251-.096.122a4.845 4.845 0 0 0-.677 1.217 3.635 3.635 0 0 0-.105 1.815c.103.461.421 1.095.739 1.468.242.285.797.764.886.764.024 0 .044-.048.044-.106.001-.23.184-.973.326-1.327.423-1.058 1.351-1.96 2.82-2.74.245-.13.952-.47 1.572-.757 1.36-.63 2.103-1.015 2.511-1.305 1.176-.833 1.903-2.065 2.14-3.625.086-.57.086-1.634 0-2.207-.368-2.438-2.195-4.096-4.818-4.37-2.925-.307-6.648 1.953-8.942 5.427-1.116 1.69-1.87 3.565-2.187 5.443-.123.728-.169 2.08-.093 2.75.193 1.704.822 3.078 1.903 4.156a6.531 6.531 0 0 0 1.87 1.313c2.368 1.13 4.99 1.155 7.295.071.996-.469 1.974-1.196 3.023-2.25 1.02-1.025 1.71-1.88 3.592-4.458 1.04-1.423 1.864-2.368 2.272-2.605l.15-.086-.019 3.091c-.018 2.993-.022 3.107-.123 3.561-.6 2.678-2.54 4.636-5.195 5.242l-.468.107-5.775.01c-4.734.008-5.85-.002-6.19-.056z"/>
                        </svg>
                    </div>
                    <div class="link-text">ایتا</div>
                </div>
            </a>
        </div>
    </div>
</body>
</html>
