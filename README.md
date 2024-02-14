# ximeydani
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para mi Ximena de Dani</title>
</head>

<body>
    <div id="conteudo">
        <h1>¿Quieres ser mi San Valentin?</h1>
        <div style="margin: auto;width: 170px;">
        <button style="position: fixed;display: block;" class="btn" onclick="sí()">SÍ</button>
        <button class="btn" onclick="desvia(this)" onmouseover="desvia(this)" style="position: absolute;">NO</button>
    </div>
</div>
</body>

<style>
    #conteudo {
        background: lightcoral;
        width: 100%;
        height: 100%;
        position: fixed;
        top: 0;
        left: 0;
        padding: 10px;
        text-align: center;
        font-family: sans-serif;
}
</style>

<script>
    function sí() {
        alert("¡Aceptaste salir conmigo! :) Dani contento")
        // redireciona para um URL após clicar no SIM
        location.href = "https://i.makeagif.com/media/10-18-2021/l2UQlN.mp4";
    }

    function desvia(btn) {
        // btn declarado na função
        btn.style.position = 'absolute';
        btn.style.bottom = geraPosicao(10, 90);
        btn.style.left = geraPosicao(10, 90);
        console.log('opa, desviei...');
    }

    function geraPosicao(min, max) {
        return (Math.random() * (max - min) + min) + "%";
    }

</script>

</html>
