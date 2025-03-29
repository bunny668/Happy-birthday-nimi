<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday Nimra!</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            text-align: center;
            background-color: #1E90FF; /* Blue Theme */
            color: white;
            margin: 0;
            padding: 0;
            overflow: hidden;
        }
        .container {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 90%;
            max-width: 600px;
        }
        h1 {
            font-size: 50px;
            animation: fadeIn 2s ease-in-out;
        }
        p {
            font-size: 22px;
            animation: fadeIn 3s ease-in-out;
        }
        .heart {
            color: red;
            font-size: 30px;
        }
        .btn {
            background-color: white;
            color: #1E90FF;
            padding: 12px 25px;
            font-size: 20px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
            margin-top: 20px;
            transition: 0.3s;
        }
        .btn:hover {
            background-color: lightgray;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: scale(0.8); }
            to { opacity: 1; transform: scale(1); }
        }
        .balloons img {
            width: 50px;
            position: absolute;
            animation: floatUp 5s linear infinite;
        }
        @keyframes floatUp {
            from { transform: translateY(100vh); }
            to { transform: translateY(-10vh); }
        }
    </style>
</head>
<body>
    <audio id="birthdayMusic" src="https://www.myinstants.com/media/sounds/happy-birthday-to-you.mp3"></audio>
    
    <div class="container">
        <h1>Happy Birthday Nimra! 🎉</h1>
        <p>Wishing you a day filled with love, joy, and happiness! <br> You are truly special, and I hope this surprise makes you smile! <span class="heart">❤️</span></p>
        <button class="btn" onclick="playMusic()">Click for a Surprise</button>
    </div>

    <!-- Balloons Animation -->
    <div class="balloons">
        <img src="https://cdn-icons-png.flaticon.com/512/3467/3467988.png" style="left: 10%;" />
        <img src="https://cdn-icons-png.flaticon.com/512/3467/3467988.png" style="right: 10%;" />
    </div>

    <script>
        function playMusic() {
            document.getElementById("birthdayMusic").play();
            alert("Happy Birthday Nimra! 🎂🎈🎁");
        }
    </script>
</body>
</html>
