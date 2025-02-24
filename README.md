# Aula FrontEnd 03 (20/02/2025)

# index.html
O código HTML apresentado define a estrutura básica de uma página web. Vamos analisar cada parte:
- &lt;!DOCTYPE html&gt;: Esta declaração indica ao navegador que o documento é um documento HTML5.
- &lt;html lang="pt-BR"&gt;: Define o idioma do documento como português do Brasil. Isso é importante para a acessibilidade e para que o navegador possa renderizar corretamente caracteres especiais e acentuação.
- &lt;head&gt;: Contém metadados sobre a página, como o título, charset e informações para o navegador.
- &lt;meta charset="UTF-8"&gt;: Define o conjunto de caracteres utilizado na página. UTF-8 é um padrão amplamente utilizado que suporta uma ampla variedade de caracteres.
- &lt;meta name="viewport" content="width=device-width, initial-scale=1.0"&gt;: Configura a viewport para dispositivos móveis, garantindo que a página seja exibida corretamente em diferentes tamanhos de tela.   
- &lt;title&gt;Exemplo de Layout&lt;/title&gt;: Define o título da página, que é exibido na barra de título do navegador.
- &lt;link rel="stylesheet" href="styles.css"&gt;: Inclui um arquivo CSS externo chamado "styles.css", que contém as regras de estilo para a página.
- &lt;body&gt;: Contém o conteúdo visível da página.

## Layout da Página
O código utiliza um layout de três colunas:
- &lt;aside class="menu-lateral"&gt;: Define a seção lateral para o menu de navegação.
- &lt;header class="cabecalho"&gt;: Define o cabeçalho da página, contendo o título e um botão.
- &lt;main class="principal"&gt;: Define a seção principal da página, onde o conteúdo principal será exibido.

## Elementos e Classes
- &lt;div class="container"&gt;: Cria um contêiner para organizar os elementos da página.
- &lt;ul&gt; e &lt;li&gt;: Usados para criar uma lista não ordenada.
- &lt;a href="#"&gt;: Cria um link para outra página ou seção da página.
- &lt;button class="btn-animate"&gt;: Cria um botão.

# style.css
Classes CSS: As classes CSS definidas no arquivo "styles.css" serão usadas para estilizar os elementos da página.
O código CSS apresentado definiu o estilo visual da página HTML. Vamos analisar cada parte:

## Layout Base com Grid
- body { ... }: Define as propriedades gerais do corpo da página, como margem, fonte e layout.
- display: grid;: Configura o elemento &lt;body&gt; para usar o layout em grid, permitindo posicionar os elementos de forma flexível.
- grid-template-areas: Define as áreas de grid para os elementos. Neste caso, o layout é dividido em duas áreas: "menu" e "principal".
- grid-template-columns: Define a largura das colunas do grid. A primeira coluna tem 200 pixels e a segunda ocupa o restante do espaço.
- gap: 10px;: Define o espaço entre os elementos do grid.

## Menu Lateral
- .menu-lateral { ... }: Define o estilo da seção lateral do menu.
- grid-area: menu;: Associa essa classe à área de grid "menu".
- background-color: #f0f0f0;: Define a cor de fundo do menu.
- padding: 15px;: Adiciona espaçamento interno ao menu.

## Cabeçalho
- .cabecalho { ... }: Define o estilo do cabeçalho.
- grid-area: cabecalho;: Associa essa classe à área de grid "cabecalho".
- background: linear-gradient(90deg, #007bff, #00d084);: Define um gradiente de cores para o fundo.
- color: white;: Define a cor do texto.
- display: flex;: Configura o cabeçalho para usar o layout flexbox.
- justify-content: space-between;: Distribui os elementos dentro do cabeçalho de forma uniforme.
- align-items: center;: Alinha os elementos verticalmente no centro.

## Botão com Transição e Animação
- .btn-animate { ... }: Define o estilo do botão.
- transition: background-color 0.3s, color 0.3s;: Aplica uma transição para as propriedades de cor e fundo do botão, criando um efeito de animação quando o botão é hoverado.
- .btn-animate:hover { ... }: Define o estilo do botão quando o mouse está sobre ele.

## Conteúdo Principal
- .principal { ... }: Define o estilo da seção principal.
- display: flex;: Configura a seção principal para usar o layout flexbox.
- flex-direction: column;: Orienta os elementos na direção vertical.
- gap: 10px;: Define o espaço entre os elementos.

## Animação
- @keyframes slideIn { ... }: Define uma animação chamada "slideIn" que desliza os elementos para baixo.
- .content-box { ... }: Aplica a animação "slideIn" ao elemento .content-box.

## Responsividade
- @media (max-width: 768px) { ... }: Define estilos para dispositivos com largura máxima de 768 pixels.
- @media (max-width: 1024px) and (min-width: 769px) { ... }: Define estilos para dispositivos com largura entre 769 e 1024 pixels.
