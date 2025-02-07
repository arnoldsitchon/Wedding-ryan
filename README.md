<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wedding Invitation</title>
    <style>3
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f8f8f8;
            padding: 20px;
        }
        .invitation {
            background: pink;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
            display: inline-block;
        }
        img {
            width: 100%;
            max-width: 400px;
            border-radius: 10px;
        }
        h1 {
            color: #d63384;
        }
        p {
            font-size: 18px;
            color: #333;
        }
    </style>
    <link rel="stylesheet" href="css/style.css" />
</head>

<body>

    <div class="invitation">
        <h1>You're Invited!</h1>
        <img src="Wedding.jpg" alt="Wedding Couple">
        <h2>Mr. & Mrs. Bumanglag</h2>
        <p>We joyfully invite you to our wedding celebration.</p>
        <p><strong>Date:</strong> April 28, 2025</p>
        <p><strong>Time:</strong> [Insert Time]</p>
        <p><strong>Location:</strong> [Insert Venue]</p>
        <p>Join us in celebrating love, laughter, and happily ever after.</p>
    </div

</body>
</html>
<video controls>
    <source src="Wedding1.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>
function countdown() {
    const weddingDate = new Date("April 28, 2025 00:00:00").getTime();
    const now = new Date().getTime();
    const timeLeft = weddingDate - now;

    const days = Math.floor(timeLeft / (1000 * 60 * 60 * 24));
    document.getElementById("countdown").innerHTML = `<h3>${days} Days to Go!</h3>`;

    setTimeout(countdown, 1000 * 60 * 60); 
}

countdown();


