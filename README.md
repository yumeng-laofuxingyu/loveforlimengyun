<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>给宝贝老婆的表白</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Microsoft YaHei', sans-serif;
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%);
            color: #fff;
            line-height: 1.6;
            overflow-x: hidden;
            min-height: 100vh;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }
        
        .container {
            max-width: 500px;
            width: 100%;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            padding: 30px;
            text-align: center;
            position: relative;
            overflow: hidden;
            margin: 20px 0;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .stars {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
        }
        
        .star {
            position: absolute;
            background-color: white;
            border-radius: 50%;
            animation: twinkle 5s infinite;
        }
        
        @keyframes twinkle {
            0%, 100% { opacity: 0.2; }
            50% { opacity: 1; }
        }
        
        h1 {
            font-size: 28px;
            margin-bottom: 20px;
            color: #ff9a9e;
            text-shadow: 0 0 10px rgba(255, 154, 158, 0.5);
        }
        
        .name {
            color: #ff9a9e;
            font-weight: bold;
            font-size: 32px;
            margin: 10px 0;
            text-shadow: 0 0 10px rgba(255, 154, 158, 0.5);
        }
        
        .message {
            font-size: 18px;
            margin: 20px 0;
            text-align: left;
            padding: 0 10px;
            line-height: 1.8;
            min-height: 60px;
        }
        
        .love-letter {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 20px;
            margin: 20px 0;
            text-align: left;
            border-left: 4px solid #ff9a9e;
        }
        
        .btn {
            background: linear-gradient(to right, #ff9a9e, #fad0c4);
            color: #333;
            border: none;
            padding: 12px 30px;
            font-size: 18px;
            border-radius: 50px;
            cursor: pointer;
            margin: 20px 0;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            transition: all 0.3s ease;
            font-weight: bold;
        }
        
        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
        }
        
        .hearts-container {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 15px;
            margin: 20px 0;
        }
        
        .heart {
            width: 40px;
            height: 40px;
            background-color: #ff4d79;
            transform: rotate(45deg);
            position: relative;
            animation: heartbeat 1.5s infinite;
        }
        
        .heart:before, .heart:after {
            content: '';
            width: 40px;
            height: 40px;
            background-color: #ff4d79;
            border-radius: 50%;
            position: absolute;
        }
        
        .heart:before {
            top: -20px;
            left: 0;
        }
        
        .heart:after {
            top: 0;
            left: -20px;
        }
        
        @keyframes heartbeat {
            0%, 100% { transform: rotate(45deg) scale(1); }
            50% { transform: rotate(45deg) scale(1.1); }
        }
        
        .footer {
            margin-top: 20px;
            font-size: 14px;
            color: rgba(255, 255, 255, 0.7);
        }
        
        .hidden {
            opacity: 0;
            transform: translateY(20px);
            transition: all 0.8s ease;
        }
        
        .show {
            opacity: 1;
            transform: translateY(0);
        }
        
        .floating-hearts {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            pointer-events: none;
        }
        
        .floating-heart {
            position: absolute;
            font-size: 24px;
            color: #ff9a9e;
            opacity: 0;
            animation: floatUp 5s linear forwards;
        }
        
        @keyframes floatUp {
            0% {
                transform: translateY(100px) rotate(0deg);
                opacity: 1;
            }
            100% {
                transform: translateY(-100px) rotate(360deg);
                opacity: 0;
            }
        }
        
        .photo-frame {
            width: 150px;
            height: 150px;
            margin: 20px auto;
            border-radius: 50%;
            background: linear-gradient(45deg, #ff9a9e, #fad0c4, #a1c4fd);
            padding: 5px;
            animation: rotate 10s linear infinite;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .photo {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.2);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 40px;
            color: white;
        }
        
        @keyframes rotate {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        .music-note {
            position: absolute;
            font-size: 20px;
            color: #ff9a9e;
            opacity: 0;
            animation: musicFloat 3s linear infinite;
        }
        
        @keyframes musicFloat {
            0% {
                transform: translateY(0) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                transform: translateY(-100px) rotate(360deg);
                opacity: 0;
            }
        }
        
        .typing {
            border-right: 2px solid #ff9a9e;
            animation: blink 0.7s infinite;
        }
        
        @keyframes blink {
            0%, 100% { border-color: transparent; }
            50% { border-color: #ff9a9e; }
        }
    </style>
</head>
<body>
    <div class="stars" id="stars"></div>
    <div class="floating-hearts" id="floatingHearts"></div>
    
    <div class="container">
        <h1>亲爱的 <span class="name">宝贝老婆</span></h1>
        
        <div class="photo-frame">
            <div class="photo">
                <i class="fas fa-heart"></i>
            </div>
        </div>
        
        <div class="message" id="message1"></div>
        
        <div class="love-letter hidden" id="message2">
            遇见你是我这辈子最幸运的事<br><br>
            你的笑容是我每天的动力<br><br>
            喜欢和你在一起的每一帧每一秒<br><br>
            你说我的套路都是你玩过的<br><br>
	          那么这个呢？<br><br>
            希望给你独一无二的，老婆
        </div>
        
        <div class="hearts-container">
            <div class="heart"></div>
            <div class="heart"></div>
            <div class="heart"></div>
        </div>
        
        <div class="message hidden" id="message3"></div>
        
        <button class="btn hidden" id="confessBtn">点击看看我想说什么啊 ❤️</button>
        
        <div class="footer hidden" id="footer">
            永远爱你的老公 · 给李梦云小朋友专门做的哦
        </div>
    </div>

    <script>
        // 创建星空背景
        function createStars() {
            const starsContainer = document.getElementById('stars');
            for (let i = 0; i < 100; i++) {
                const star = document.createElement('div');
                star.classList.add('star');
                star.style.left = Math.random() * 100 + '%';
                star.style.top = Math.random() * 100 + '%';
                star.style.width = Math.random() * 3 + 1 + 'px';
                star.style.height = star.style.width;
                star.style.animationDelay = Math.random() * 5 + 's';
                starsContainer.appendChild(star);
            }
        }
        
        // 创建漂浮爱心
        function createFloatingHearts() {
            const container = document.getElementById('floatingHearts');
            for (let i = 0; i < 20; i++) {
                setTimeout(() => {
                    const heart = document.createElement('div');
                    heart.classList.add('floating-heart');
                    heart.innerHTML = '❤️';
                    heart.style.left = Math.random() * 100 + '%';
                    heart.style.animationDelay = Math.random() * 5 + 's';
                    container.appendChild(heart);
                    
                    // 移除爱心元素以优化性能
                    setTimeout(() => {
                        heart.remove();
                    }, 5000);
                }, i * 300);
            }
        }
        
        // 创建音乐符号
        function createMusicNotes() {
            const container = document.getElementById('floatingHearts');
            for (let i = 0; i < 10; i++) {
                setTimeout(() => {
                    const note = document.createElement('div');
                    note.classList.add('music-note');
                    note.innerHTML = '♪';
                    note.style.left = Math.random() * 100 + '%';
                    note.style.animationDelay = Math.random() * 3 + 's';
                    container.appendChild(note);
                    
                    // 移除音符元素以优化性能
                    setTimeout(() => {
                        note.remove();
                    }, 3000);
                }, i * 500);
            }
        }
        
        // 打字机效果
        function typeWriter(element, text, speed = 50) {
            return new Promise((resolve) => {
                let i = 0;
                element.innerHTML = '';
                element.classList.add('typing');
                
                function type() {
                    if (i < text.length) {
                        element.innerHTML += text.charAt(i);
                        i++;
                        setTimeout(type, speed);
                    } else {
                        element.classList.remove('typing');
                        resolve();
                    }
                }
                
                type();
            });
        }
        
        // 显示隐藏的元素
        function showElements() {
            const elements = document.querySelectorAll('.hidden');
            elements.forEach((el, index) => {
                setTimeout(() => {
                    el.classList.add('show');
                }, index * 1000);
            });
        }
        
        // 按钮点击事件
        document.getElementById('confessBtn').addEventListener('click', function() {
            this.innerHTML = "❤️ 我爱你，宝贝老婆！ ❤️";
            this.style.background = "linear-gradient(to right, #ff4d79, #ff8fa3)";
            this.style.color = "white";
            
            // 创建更多漂浮元素
            createFloatingHearts();
            createMusicNotes();
            
            // 显示最后的footer
            setTimeout(() => {
                document.getElementById('footer').classList.add('show');
            }, 2000);
            
            // 打字机效果显示最后一条消息
            setTimeout(() => {
                typeWriter(document.getElementById('message3'), "我们的约定：在一起3年就结婚，我都记得");
            }, 1000);
        });
        
        // 初始化
        window.onload = function() {
            createStars();
            createFloatingHearts();
            createMusicNotes();
            
            // 使用打字机效果显示第一条消息
            setTimeout(() => {
                typeWriter(document.getElementById('message1'), "你猜我想说什么？").then(() => {
                    // 显示其他元素
                    setTimeout(showElements, 500);
                    
                    // 打字机效果显示第二条消息
                    setTimeout(() => {
                        typeWriter(document.getElementById('message3'), "我想告诉你...");
                    }, 1000);
                });
            }, 1000);
        };
    </script>
</body>
</html>
