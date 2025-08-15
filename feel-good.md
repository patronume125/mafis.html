<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Feel Good Space</title>
<style>
    body {
        margin: 0;
        font-family: 'Poppins', sans-serif;
        background: linear-gradient(135deg, #a8d0e6, #f6d6d6);
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        flex-direction: column;
        color: #333;
        text-align: center;
    }
    h1 {
        font-size: 2.5rem;
        margin-bottom: 10px;
    }
    p {
        font-size: 1.2rem;
        max-width: 400px;
    }
    .quote {
        font-style: italic;
        margin-top: 20px;
        background: rgba(255, 255, 255, 0.3);
        padding: 15px;
        border-radius: 10px;
        box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }
    button {
        margin-top: 20px;
        padding: 10px 20px;
        font-size: 1rem;
        border: none;
        background: #76c7c0;
        color: white;
        border-radius: 25px;
        cursor: pointer;
        transition: 0.3s;
    }
    button:hover {
        background: #5aa7a2;
    }
</style>
</head>
<body>

<h1>Welcome, Mahimai Anthony 🌸</h1>
<p>Take a deep breath. This is your peaceful corner on the web.</p>

<div class="quote" id="quote">"Happiness is not something ready made. It comes from your own actions."</div>

<button onclick="newQuote()">New Quote</button>

<script>
    const quotes = [
        "Happiness is not something ready made. It comes from your own actions.",
        "Every day may not be good, but there’s something good in every day.",
        "Peace begins with a smile.",
        "Believe you can and you're halfway there.",
        "You are exactly where you need to be."
    ];
    function newQuote() {
        const randomIndex = Math.floor(Math.random() * quotes.length);
        document.getElementById("quote").textContent = `"${quotes[randomIndex]}"`;
    }
</script>

</body>
</html>
