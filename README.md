# whereyoutrip
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>오늘의 여행지 추</title>
    <style>
        body {
            text-align: center;
            font-size: 2rem;
            margin-top: 20%;
        }
    </style>
</head>
<body>
    <p id="message">오늘은 어디로 떠나보면 좋을까요?</p>
    <button onclick="showRandomMessage()">눌러서 확인하기</button>

    <script>
        function showRandomMessage() {
            const messages = [
                "역사가 깊은 도시,이스탄불",
                "폭싹 속았수다,제주",
                "라라랜드 속 그곳,LA",
                "푸른 지붕의 하얀 집,산토리니",
                "콜로세움 앞에서 피자를,로마"
                "에펠탑 앞에서 인생샷,파리",
                "춥지만 아름다운 겨울왕국,모스크바",
                "정열적인 삼바를 함께,리우",
                "열대과일과 힐링을,방콕",
                "만 개의 음식의 집합,홍콩"
                "이국적인 매력의 초대,뮌헨",
                "사막에서의 트래킹,리야드",
                "대추야자와 낙타,두바이",
                "정통의 스시와 온천,도쿄",
                "신사와 축구의 공존,런던"
            ];
            document.getElementById("message").innerText = messages[Math.floor(Math.random() * messages.length)];
        }
    </script>
</body>
</html>
