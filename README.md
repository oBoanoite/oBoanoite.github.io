<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Namora comigo?</title>
</head>

<body>
    <div id="conteudo">
    <h2>Aceita namorar comigo?</h2>
    <button class="btn" onclick="sim()">SIM</button>
    <button class="btn" onclick="desviar(this)">NÃO</button>
    </div>
    <button id="Recado" onclick="Recado()" style="color: white;font-size: 17px;background: #08f;padding: 
    12px;position: fixed;bottom: 0;right: 0;width: 100%;border: 1px solid white;">Tem um papel no bolso 
        pequeno da sua mochila</button>
</body>

<style>
   #conteudo{
    background: #fb4d4d;
    width: 100%;
    height: 100%;
    position: fixed;
    top: 0;
    left: 0;
    padding: 10px;
    text-align: center;
   }

   .btn{
    background: black;
    color: white;
    border: none;
    padding: 10px;
    width: 80px;
    border-radius: 5px;
}

</style>

<script>
    function sim(){
    alert("Então estamos namorando! <3")
    }

function desviar(t) {
     var btn = t;
     btn.style.position = "absolute";
     btn.style.bottom = geraPosicao(10, 90);
     btn.style.left = geraPosicao(10, 90);
     console.log("NOPE :P")

}

function geraPosicao(min, max) {
 return(Math.random() * (max - min) + min) + "%";

}

</script>

</html>
