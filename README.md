<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Salon Service Roller</title>

<style>
body {
    font-family: Arial, sans-serif;
    background: linear-gradient(135deg, #fff0f5, #f8e8ff);
    text-align: center;
    padding: 50px 20px;
    color: #333;
}

.container {
    max-width: 600px;
    margin: auto;
    background: white;
    padding: 40px;
    border-radius: 25px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.12);
}

h1 {
    font-size: 42px;
    margin-bottom: 10px;
}

.subtitle {
    font-size: 18px;
    color: #777;
}

#service {
    font-size: 36px;
    font-weight: bold;
    margin: 50px 10px;
    min-height: 50px;
}

button {
    background: #111;
    color: white;
    border: none;
    padding: 18px 45px;
    font-size: 20px;
    border-radius: 50px;
    cursor: pointer;
}

button:hover {
    transform: scale(1.05);
}

#again {
    display: none;
    margin-top: 15px;
    background: #777;
}
</style>
</head>

<body>

<div class="container">

<h1>🎲 Salon Service Roller</h1>

<p class="subtitle">
Let the dice choose your service today!
</p>

<div id="service">
✨ Ready?
</div>

<button onclick="rollService()">
🎲 ROLL
</button>

<button id="again" onclick="rollService()">
ROLL AGAIN
</button>

</div>

<script>

const services = [
    "💇 Haircut",
    "💆 Gel polish",
    "✨ Nail Art",
    "🎨 Hair Wash & blast Dry",
    "💅 Manicure",
    "🌸Gel Polish",
    "💎 Stick on Nails",
    "🧖‍♀️ Foot Massage"
];

function rollService() {

    const service =
        services[Math.floor(Math.random() * services.length)];

    document.getElementById("service").innerText = service;

    document.getElementById("again").style.display = "inline-block";
}

</script>

</body>
</html>
