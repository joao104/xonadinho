<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eu Te Amo</title>
    <!-- Bootstrap CSS -->
    <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.6.2/css/bootstrap.min.css" rel="stylesheet">
    
    <style>
        /* Estilo Geral */
        body {
            background: linear-gradient(to bottom, #ff9a9e, #fad0c4);
            color: #161414;
            font-family: 'Arial', sans-serif;
            height: 100vh;
            overflow: hidden;
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
        }
        .heart-container {
            text-align: center;
        }
        /* Coração Grande */
        .heart {
            position: relative;
            width: 100px;
            height: 100px;
            background-color: #ff4d4d;
            transform: rotate(-45deg);
            animation: heartbeat 1s infinite;
            margin: 0 auto;
        }
        .heart::before,
        .heart::after {
            content: '';
            position: absolute;
            width: 100px;
            height: 100px;
            background-color: #ff4d4d;
            border-radius: 50%;
        }
        .heart::before {
            top: -50px;
            left: 0;
        }
        .heart::after {
            left: 50px;
            top: 0;
        }
        @keyframes heartbeat {
            0%, 100% {
                transform: scale(1) rotate(-45deg);
            }
            50% {
                transform: scale(1.2) rotate(-45deg);
            }
        }
        .message {
            margin-top: 20px;
            font-size: 24px;
            font-weight: bold;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }
        .btn-love {
            margin-top: 30px;
            background-color: #ff4d4d;
            color: #151111;
            border: none;
            padding: 10px 20px;
            font-size: 18px;
            border-radius: 25px;
            transition: all 0.3s;
        }
        .btn-love:hover {
            background-color: #e63939;
            transform: scale(1.1);
        }

        /* Corações Chovendo */
        .falling-hearts {
            position: fixed;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 0;
        }
        .falling-hearts span {
            position: absolute;
            display: block;
            width: 15px;
            height: 15px;
            background: #ff4d4d;
            clip-path: polygon(50% 0%, 100% 35%, 80% 100%, 50% 80%, 20% 100%, 0% 35%);
            animation: fall 5s linear infinite;
        }
        @keyframes fall {
            0% {
                transform: translateY(-100%) rotate(0deg);
                opacity: 1;
            }
            100% {
                transform: translateY(100vh) rotate(360deg);
                opacity: 0;
            }
        }

        /* Gerar corações aleatórios */
        .falling-hearts span:nth-child(1) { left: 10%; animation-duration: 4s; }
        .falling-hearts span:nth-child(2) { left: 20%; animation-duration: 6s; }
        .falling-hearts span:nth-child(3) { left: 30%; animation-duration: 4.5s; }
        .falling-hearts span:nth-child(4) { left: 40%; animation-duration: 5.2s; }
        .falling-hearts span:nth-child(5) { left: 50%; animation-duration: 6.5s; }
        .falling-hearts span:nth-child(6) { left: 60%; animation-duration: 4.8s; }
        .falling-hearts span:nth-child(7) { left: 70%; animation-duration: 5.6s; }
        .falling-hearts span:nth-child(8) { left: 80%; animation-duration: 4.1s; }
        .falling-hearts span:nth-child(9) { left: 90%; animation-duration: 6.2s; }
        .falling-hearts span:nth-child(10) { left: 95%; animation-duration: 5.7s; }
    </style>
</head>
<body>
    <div class="falling-hearts">
        <!-- Gerando os corações -->
        <span></span><span></span><span></span><span></span><span></span>
        <span></span><span></span><span></span><span></span><span></span>
    </div>
    <div class="heart-container">
        <div class="heart"></div>
        <div class="message"> <strong>KALINE E A MAIS LINDA DO MUNDO</strong> ❤️</div>
        <button class="btn-love" onclick="showLove()">Clique para mais amor</button>
    </div>

    <!-- Optional JavaScript -->
    <script>
        function showLove() {
            alert('JESUS TE AMA, E EU TAMBÉM ❤️');
        }
    </script>]<link rel="stylesheet" href="css/bootstrap.min.css">
<script src="js/bootstrap.min.js"></script>




<script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.9.3/dist/umd/popper.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>

</body>
</html>
