# Documentação do Projeto: Jogo da Velha

## Descrição:
Este é um jogo da velha simples desenvolvido em HTML, CSS e JavaScript. O objetivo do jogo é alcançar uma linha, coluna ou diagonal preenchida com o símbolo do jogador (X ou O) antes do adversário.

## Estrutura do Projeto:

### Arquivos:
- **index.html**: Contém a estrutura HTML do jogo, incluindo a grade do jogo, elementos de interface do usuário e referências aos arquivos de estilo e script.
- **estilo.css**: Este arquivo contém estilos CSS para estilizar a aparência do jogo.
- **velha.js**: Este é o arquivo JavaScript que contém a lógica do jogo.

### Funcionalidades:

- **Escolha de Quadrado**: Os jogadores podem clicar em qualquer quadrado vazio para selecioná-lo. Cada clique alterna entre os símbolos do jogador atual (X ou O).
- **Atualização do Jogador Atual**: Um elemento de texto exibe qual jogador está atualmente jogando.
- **Verificação de Vencedor**: O jogo verifica automaticamente se um jogador alcançou uma linha, coluna ou diagonal preenchida com seus símbolos. Se um jogador vence, o jogo exibe o vencedor e encerra.
- **Reiniciar o Jogo**: Um botão "Reiniciar" permite reiniciar o jogo a qualquer momento.

## Como Jogar:

1. Abra o arquivo `index.html` em um navegador da web compatível.
2. Clique em qualquer quadrado vazio para fazer sua jogada.
3. O jogo alternará entre os jogadores, exibindo qual jogador está atualmente jogando.
4. Continue jogando até que um jogador alcance uma linha, coluna ou diagonal preenchida com seus símbolos.
5. Se houver um vencedor, o jogo exibirá o vencedor. Você pode clicar no botão "Reiniciar" para começar um novo jogo.

## Documentação do Código: Jogo da Velha

### Variáveis Globais:
- `jogador`: Armazena o símbolo do jogador atual (X ou O).
- `vencedor`: Armazena o símbolo do jogador que venceu o jogo ou null se não houver vencedor.
- `jogadorSelecionado`: Referência ao elemento HTML que exibe o jogador atual.
- `vencedorSelecionado`: Referência ao elemento HTML que exibe o vencedor.
- `quadrados`: Lista de elementos HTML que representam os quadrados do tabuleiro.

### Função `mudarJogador(valor)`:
- Atualiza o símbolo do jogador atual e exibe no elemento HTML `jogadorSelecionado`.

### Função `escolherQuadrado(id)`:
- Recebe o ID de um quadrado clicado e verifica se o jogo já tem um vencedor.
- Se o quadrado estiver vazio, atualiza o conteúdo com o símbolo do jogador atual e alterna para o próximo jogador.
- Chama a função `checaVencedor()` após cada jogada para verificar se há um vencedor.

### Função `checaVencedor()`:
- Verifica todas as combinações possíveis de vitória (linhas, colunas e diagonais).
- Se uma sequência vencedora for encontrada, atualiza a cor dos quadrados vencedores e exibe o vencedor.
- Se não houver vencedor, o jogo continua.

### Função `reiniciar()`:
- Reinicia o jogo, limpando o tabuleiro, redefinindo as variáveis de controle e exibindo o jogador inicial.

### Funções Auxiliares:
- `mudaCorQuadrado(quadrado1, quadrado2, quadrado3)`: Atualiza a cor de fundo dos quadrados vencedores.
- `checaSequencia(quadrado1, quadrado2, quadrado3)`: Verifica se três quadrados têm o mesmo conteúdo.

Este código implementa a lógica do jogo da velha em JavaScript, permitindo aos jogadores jogar e determinando automaticamente o vencedor.

## Créditos:
Este projeto foi desenvolvido como parte de um tutorial ou exercício prático de programação. Créditos aos criadores originais do tutorial ou curso.

## Conclusão:
O jogo da velha é um projeto simples, mas divertido, que demonstra conceitos básicos de desenvolvimento web usando HTML, CSS e JavaScript. Com um pouco de criatividade e habilidades de programação, é possível criar muitas variações e melhorias neste projeto básico.
