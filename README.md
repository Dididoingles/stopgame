# Stop Game

Jogo de Stop (Adedonha) online para praticar vocabulario em ingles. Gire a roleta, descubra a categoria + letra e seja o mais rapido a dizer uma palavra valida antes do tempo acabar.

Jogue agora: https://dididoingles.github.io/stopgame/

Previa do jogo: metatag.png

---

## Como jogar

1. Configure a partida - escolha de 2 a 8 jogadores e digite os nomes.
2. Gire a roleta - o sorteio define aleatoriamente uma categoria e uma letra.
3. Diga uma palavra - o primeiro a falar uma palavra valida em ingles que combine com a categoria e comece com a letra sorteada ganha o ponto.
4. Marque o ponto - toque no jogador que acertou no modal "Quem acertou?".
5. Repita - cada rodada sorteia uma nova combinacao (letras ja sorteadas ficam marcadas na roleta).
6. Fim de jogo - clique em "Fim de jogo" a qualquer momento para ver o placar final e o campeao.

---

## Funcionalidades

- Roleta animada com as 26 letras do alfabeto (letras ja sorteadas ficam destacadas)
- Sorteio aleatorio de categoria + letra
- Timer de 60 segundos com anel de progresso e alerta visual/sonoro nos ultimos 10s
- Suporte de 2 a 8 jogadores com placar em tempo real e destaque para o lider
- Layout responsivo - experiencia otimizada para desktop e mobile (overlay dedicado no celular)
- Efeitos sonoros (giro da roleta, cliques, tique-taque do timer, fim de jogo)
- Tela de fim de jogo com leaderboard, badge de campeao e suporte a empates
- Novo jogo sem recarregar a pagina

---

## Categorias disponiveis

| Ingles            | Portugues         |
|-------------------|-------------------|
| NAME              | nome              |
| ANIMAL            | animal            |
| FRUIT             | fruta             |
| COLOR             | cor               |
| CITY OR COUNTRY   | cidade ou pais    |
| OBJECT            | objeto            |
| BRAND             | marca             |
| PLANT             | planta            |
| SONG              | musica            |
| MOVIE OR SERIES   | filme ou serie    |

---

## Tecnologias

- HTML5 + CSS3 (variaveis CSS, Grid, Flexbox, animacoes)
- JavaScript puro (vanilla, sem dependencias)
- Canvas API para desenhar a roleta
- Web Audio API + arquivos de audio externos para os efeitos sonoros
- Google Fonts - Instrument Serif, Geist e Geist Mono

---

## Estrutura do projeto

stopgame/
  index.html      # Jogo completo (HTML + CSS + JS em um unico arquivo)
  metatag.png     # Imagem de previa para redes sociais (1200x630)
  favicon.ico     # Icone do site

O jogo e single-file: todo o CSS e JavaScript estao embutidos no index.html, o que facilita o deploy no GitHub Pages.

---

## Como rodar localmente

1. Clone o repositorio:

   git clone https://github.com/dididoingles/stopgame.git

2. Abra o arquivo index.html no navegador - pronto. Nao precisa de servidor nem build.

Dica: se quiser testar o audio sem bloqueios do navegador, sirva via servidor local (ex.: npx serve ou a extensao Live Server do VS Code).

---

## Deploy no GitHub Pages

1. Suba os arquivos (index.html, metatag.png, favicon.ico) para a raiz do repositorio.
2. Va em Settings > Pages.
3. Em Source, selecione a branch main e a pasta / (root).
4. Salve e aguarde o deploy - o jogo estara em https://dididoingles.github.io/stopgame/

---

## Metatags de compartilhamento

O index.html ja inclui as metatags Open Graph e Twitter Card para gerar previa com miniatura ao compartilhar o link:

<meta property="og:image" content="https://dididoingles.github.io/stopgame/metatag.png" />
<meta name="twitter:card" content="summary_large_image" />

Apos atualizar a imagem, force a atualizacao do cache usando o Facebook Sharing Debugger (https://developers.facebook.com/tools/debug/) ou o LinkedIn Post Inspector (https://www.linkedin.com/post-inspector/).

---

## Como adicionar novas categorias

No index.html, procure o array CATEGORIES dentro da tag <script> e adicione um novo objeto no formato:

  { en: 'FOOD', pt: 'comida' }

A categoria passa a ser sorteada automaticamente nas proximas rodadas.

---

## Sobre

Este jogo faz parte do plano de ensino da professora @dicarvalho.prof (https://www.instagram.com/dicarvalho.prof/).
Saiba mais: ../teacherdi/

---

## Licenca

Uso educacional livre. Venda proibida. 
