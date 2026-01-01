# supercoin-app
<!DOCTYPE html>
<html>
<head>
    <title>SuperCoin Miner</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://telegram.org/js/telegram-web-app.js"></script>
    <style>
        body { background: #0e0e0e; color: gold; text-align: center; font-family: 'Arial'; }
        .coin-btn { width: 200px; cursor: pointer; transition: transform 0.1s; }
        .coin-btn:active { transform: scale(0.9); }
        h1 { margin-top: 50px; }
    </style>
</head>
<body>
    <h1>SuperCoin: <span id="balance">0</span></h1>
    <img src="https://i.ibb.co/LzN2V8G/supercoin.png" class="coin-btn" onclick="mine()">
    <script>
        let count = 0;
        function mine() {
            count++;
            document.getElementById('balance').innerText = count;
            window.Telegram.WebApp.HapticFeedback.impactOccurred('medium');
        }
    </script>
</body>
</html>
