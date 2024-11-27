<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Giáng Sinh Vui Vẻ</title>
    <style>
        body {
            background-color: #f0f8ff;
            font-family: Arial, sans-serif;
            text-align: center;
            color: #2e8b57;
        }
        h1 {
            font-size: 48px;
            color: #d2691e;
            margin-top: 50px;
        }
        .snowflake {
            position: absolute;
            color: white;
            font-size: 24px;
            animation: snow 10s linear infinite;
        }
        @keyframes snow {
            0% { top: -10px; opacity: 1; }
            100% { top: 100%; opacity: 0.6; }
        }
        .tree {
            background-image: url('https://www.freepngimg.com/thumb/christmas_tree/11-2-christmas-tree-png-clipart.png');
            background-size: contain;
            background-repeat: no-repeat;
            height: 400px;
            width: 300px;
            margin: 30px auto;
        }
        .message {
            font-size: 24px;
            margin-top: 20px;
        }
        .footer {
            margin-top: 50px;
            font-size: 16px;
        }
    </style>
</head>
<body>
    <h1>Merry Christmas!</h1>

    <div class="tree"></div>

    <div class="message">
        <p>Chúc bạn một mùa Giáng Sinh an lành và hạnh phúc!</p>
    </div>

    <div class="footer">
        <p>Chúc mừng năm mới 2024!</p>
    </div>

    <!-- Snowflakes animation -->
    <script>
        for (let i = 0; i < 50; i++) {
            let snowflake = document.createElement('div');
            snowflake.className = 'snowflake';
            snowflake.style.left = `${Math.random() * 100}vw`;
            snowflake.style.animationDuration = `${Math.random() * 5 + 5}s`; // Random animation speed
            snowflake.style.animationDelay = `${Math.random() * 5}s`; // Random delay before snowflake falls
            snowflake.innerHTML = '❄';
            document.body.appendChild(snowflake);
        }
    </script>
</body>
</html>
