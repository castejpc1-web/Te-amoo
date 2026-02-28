<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Solo Para Ti ❤️</title>

<style>
body{
    margin:0;
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    background:linear-gradient(-45deg,#ff758c,#ff7eb3,#ff9a9e,#fad0c4);
    background-size:400% 400%;
    animation: fondo 8s ease infinite;
    font-family: 'Segoe UI', sans-serif;
    text-align:center;
    overflow:hidden;
}

@keyframes fondo{
    0%{background-position:0% 50%;}
    50%{background-position:100% 50%;}
    100%{background-position:0% 50%;}
}

.contenedor{
    background:rgba(255,255,255,0.15);
    backdrop-filter:blur(10px);
    padding:40px;
    border-radius:25px;
    box-shadow:0 0 30px rgba(255,255,255,0.4);
}

h1{
    font-size:40px;
    color:white;
    animation:latido 1.2s infinite alternate;
}

p{
    font-size:20px;
    color:white;
    margin-top:15px;
}

@keyframes latido{
    from{transform:scale(1);}
    to{transform:scale(1.08);}
}

.corazon{
    position:absolute;
    color:white;
    animation:flotar 6s linear infinite;
}

@keyframes flotar{
    0%{transform:translateY(100vh) scale(1);}
    100%{transform:translateY(-10vh) scale(1.5);}
}
</style>
</head>

<body>

<div class="contenedor">
    <h1>TE AMOOOOOOO<br>INMENSAMENTE ❤️</h1>
    <p>Eres la razón de mi sonrisa todos los días 💖</p>
</div>

<script>
for(let i=0;i<15;i++){
    let heart=document.createElement("div");
    heart.innerHTML="❤️";
    heart.className="corazon";
    heart.style.left=Math.random()*100+"vw";
    heart.style.fontSize=(20+Math.random()*30)+"px";
    heart.style.animationDuration=(4+Math.random()*4)+"s";
    document.body.appendChild(heart);
}
</script>

</body>
</html>
