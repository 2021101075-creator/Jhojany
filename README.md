<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Para Jhojany ❤️</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
}

body{
font-family:Arial, sans-serif;
background:linear-gradient(135deg,#ff9a9e,#fad0c4);
height:100vh;
overflow:hidden;
display:flex;
justify-content:center;
align-items:center;
}

.contenedor{
text-align:center;
color:white;
z-index:10;
}

h1{
font-size:3rem;
text-shadow:2px 2px 10px black;
}

p{
font-size:1.3rem;
margin:15px;
}

button{
padding:15px 30px;
border:none;
border-radius:50px;
font-size:20px;
cursor:pointer;
background:red;
color:white;
transition:0.3s;
}

button:hover{
transform:scale(1.1);
}

#carta{
display:none;
margin-top:25px;
background:white;
color:#333;
padding:25px;
border-radius:20px;
max-width:700px;
box-shadow:0 0 20px rgba(0,0,0,.3);
animation:aparecer 1s;
}

.fotos{
display:flex;
justify-content:center;
gap:20px;
margin-bottom:20px;
flex-wrap:wrap;
}

.fotos img{
width:180px;
height:220px;
object-fit:cover;
border-radius:20px;
border:4px solid white;
}

@keyframes aparecer{
from{
opacity:0;
transform:translateY(50px);
}
to{
opacity:1;
transform:translateY(0);
}
}

.corazon{
position:absolute;
color:red;
font-size:30px;
animation:caer linear infinite;
}

@keyframes caer{
0%{
transform:translateY(-100px);
}
100%{
transform:translateY(110vh);
}
}
</style>
</head>

<body>

<div class="contenedor">

<h1>❤️ Para Jhojany ❤️</h1>

<p>Daniel tiene algo que decirte...</p>

<button onclick="mostrarCarta()">
❤️ Presiona este corazón ❤️
</button>

<div id="carta">

<div class="fotos">
<img src="jhojany.jpg">
<img src="daniel.jpg">
</div>

<h2>Para ti, Jhojany</h2>

<p>
Desde noviembre hay alguien que no ha dejado de admirarte.
</p>

<p>
Tal vez no siempre encuentre las palabras perfectas,
pero quería que supieras que me gustas mucho.
</p>

<p>
Tu sonrisa, tu forma de ser y esos pequeños detalles
hacen que seas especial para mí.
</p>

<p>
No sé qué nos depare el destino,
pero sí sé que cada vez que pienso en ti,
mi corazón sonríe.
</p>

<p>
Con cariño ❤️<br>
Daniel
</p>

</div>

</div>

<script>

function mostrarCarta(){
document.getElementById("carta").style.display="block";
}

setInterval(()=>{
const corazon=document.createElement("div");
corazon.classList.add("corazon");
corazon.innerHTML="❤️";

corazon.style.left=Math.random()*100+"vw";
corazon.style.fontSize=(20+Math.random()*40)+"px";
corazon.style.animationDuration=(3+Math.random()*5)+"s";

document.body.appendChild(corazon);

setTimeout(()=>{
corazon.remove();
},8000);

},300);

</script>

</body>
</html>
