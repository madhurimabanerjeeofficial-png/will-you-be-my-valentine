repo:madhurimabanerjeeofficial-png/will-you-be-my-valentine 
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For Aneesh ❤️</title>
<style>
    body {
        margin: 0;
        padding: 0;
        background: linear-gradient(135deg, #ff4e8a, #ff9ecf);
        font-family: 'Arial', sans-serif;
        text-align: center;
        color: white;
        height: 100vh;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        overflow: hidden;
    }
    h1 {
        font-size: 2.8em;
        margin-bottom: 10px;
    }
    h2 {
        font-weight: normal;
        margin-bottom: 30px;
    }
    .btn {
        padding: 15px 30px;
        font-size: 1.2em;
        border: none;
        border-radius: 30px;
        cursor: pointer;
        margin: 10px;
        transition: 0.3s;
    }
    .yes {
        background-color: white;
        color: #ff4e8a;
    }
    .yes:hover {
        background-color: #ffe6f0;
        transform: scale(1.05);
    }
    .no {
        background-color: #ff2e63;
        color: white;
        position: relative;
    }
    .heart {
        position: absolute;
        font-size: 20px;
        animation: float 5s linear infinite;
    }
    @keyframes float {
        from { transform: translateY(100vh); opacity: 1; }
        to { transform: translateY(-10vh); opacity: 0; }
    }
</style>

<script>
function moveButton() {
    const button = document.querySelector('.no');
    button.style.position = 'absolute';
    button.style.top = Math.random() * window.innerHeight + 'px';
    button.style.left = Math.random() * window.innerWidth + 'px';
}

function yesClicked() {
    document.body.innerHTML = "<h1>Yay Aneesh 💖</h1><h2>You just made Madhurima the happiest person!</h2>";
}

// Floating hearts
setInterval(() => {
    const heart = document.createElement("div");
    heart.classList.add("heart");
    heart.innerHTML = "💖";
    heart.style.left = Math.random() * 100 + "vw";
    heart.style.fontSize = Math.random() * 20 + 15 + "px";
    document.body.appendChild(heart);
    setTimeout(() => heart.remove(), 5000);
}, 500);
</script>

</head>
<body>

<h1>Aneesh Mishra 💌</h1>
<h2>Will you be my Valentine?</h2>

<button class="btn yes" onclick="yesClicked()">Yes 💖</button>
<button class="btn no" onmouseover="moveButton()">No 😜</button>

</body>
</html>
