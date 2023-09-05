<!DOCTYPE html>

<html lang="pt-br">

<head>
    <title>
        Jogo da velha
    </title>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="estilo.css">
</head>

<body>
    <h1>
        Jogo da velha
    </h1>

    <div>
        <div id="1" class="quadrado" onclick="escolherQuadrado(this.id)">-</div>
        <div id="2" class="quadrado" onclick="escolherQuadrado(this.id)">-</div>
        <div id="3" class="quadrado" onclick="escolherQuadrado(this.id)">-</div>
    </div>

    <div>
        <div id="4" class="quadrado" onclick="escolherQuadrado(this.id)">-</div>
        <div id="5" class="quadrado" onclick="escolherQuadrado(this.id)">-</div>
        <div id="6" class="quadrado" onclick="escolherQuadrado(this.id)">-</div>
    </div>
    
    <div>
        <div id="7" class="quadrado" onclick="escolherQuadrado(this.id)">-</div>
        <div id="8" class="quadrado" onclick="escolherQuadrado(this.id)">-</div>
        <div id="9" class="quadrado" onclick="escolherQuadrado(this.id)">-</div>
    </div>

    <div class="jogador">
        <label>
            Jogador:
        </label>
        <label id="jogador-selecionado"></label>
    </div>
    
    <div class="vencedor">
        <label>
            Vencedor:
        </label>
        <label id="vencedor-selecionado"></label>
    </div>

    <div>
        <button onclick="reiniciar()">Reiniciar</button>
    </div>

</body>

<script src="velha.js"></script>

</html>
