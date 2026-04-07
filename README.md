<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Para Linda 💖</title>

<style>
body{
margin:0;
padding:0;
background: linear-gradient(to bottom, #ff9a9e, #fecfef);
height:100vh;
overflow:hidden;
display:flex;
justify-content:center;
align-items:center;
font-family:Arial, sans-serif;
}

h1{
color:white;
font-size:30px;
text-align:center;
z-index:1;
}

.corazon{
position:absolute;
color:red;
font-size:20px;
animation:flotar 5s linear infinite;
}

@keyframes flotar{
0%{
transform:translateY(0) scale(1);
opacity:1;
}
100%{
transform:translateY(-800px) scale(1.5);
opacity:0;
}
}

</style>

</head>

<body>

<h1>
Para Linda 💖<br>
Eres mi persona favorita 🌹
</h1>

<script>

function crearCorazon(){
const corazon = document.createElement("div");
corazon.classList.add("corazon");

corazon.innerHTML = "💖";

corazon.style.left = Math.random()*100 + "vw";
corazon.style.fontSize = Math.random()*20 + 10 + "px";

document.body.appendChild(corazon);

setTimeout(()=>{
corazon.remove();
},5000);

}

setInterval(crearCorazon,300);

</script>

</body>
</html>
