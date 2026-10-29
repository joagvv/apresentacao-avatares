# Apresentação dos Avatares

Player de apresentação para o vídeo dos avatares: a introdução e cada fala
tocam uma de cada vez, e o vídeo só segue quando você aperta **espaço**.
Na tela aparece só o vídeo.

## Online

**https://joagvv.github.io/apresentacao-avatares/**

Ao abrir, a página baixa a apresentação inteira antes de mostrar, o que leva
alguns segundos. Depois disso não trava em nenhum momento. A versão online usa
vídeos otimizados para web (branch `gh-pages`); este repositório (`main`) tem
os vídeos em qualidade máxima, para rodar no computador.

## Como rodar no computador (sem internet)

1. Baixe o projeto:
   - pelo GitHub: botão verde **Code → Download ZIP**, ou
   - pelo terminal: `git clone <endereço deste repositório>`
2. Se baixou o ZIP, **extraia** (no Mac, dois cliques no ZIP; no Windows, botão direito → *Extrair tudo*).
   Não abra a apresentação de dentro do ZIP sem extrair: os vídeos não carregam.
3. Dentro da pasta, dê dois cliques em **`ABRIR APRESENTACAO.html`**.
   Ele abre no seu navegador padrão (Chrome, Edge, Safari ou Firefox).
4. Aperte **espaço** para começar. Na primeira vez a página entra em tela cheia.

Não precisa instalar nada nem ter internet. O arquivo `.html`, o `icone.png`
e a pasta `videos/` precisam ficar juntos, na mesma estrutura.

> Se o navegador não abrir com dois cliques, arraste o `ABRIR APRESENTACAO.html`
> para uma janela do navegador.

## Controles

| Tecla | O que faz |
|---|---|
| **Espaço** | Solta a próxima parte (intro ou próxima fala) |
| **←** | Volta uma parte inteira (com fade) |
| **→** | Avança uma parte (com fade) |
| **R** | Reinicia. Enquanto o vídeo não acabou, pergunta antes (**Enter** confirma, **Esc** cancela) |
| **F** | Liga/desliga tela cheia |

No celular ou tablet: tocar na tela avança e deslizar para o lado volta ou avança.

## Como funciona

O vídeo original foi dividido em 14 partes (`videos/00.mp4` a `videos/13.mp4`):

- `00`: a introdução (0:00 → 0:29.83), que para no logo da Copa 2026.
- `01` a `13`: uma fala de avatar cada.

Entre as falas, o vídeo original mostra a mesa vazia por um instante (é aí que
um avatar troca pelo outro). Esses trechos foram identificados quadro a quadro
e **removidos**: cada parte termina no último quadro do avatar, e o espaço já
entra direto no próximo.

Trechos de mesa vazia removidos (tempo do vídeo original):

| # | Mesa vazia | # | Mesa vazia |
|---|---|---|---|
| 1 | 0:43.22 → 0:43.63 | 7 | 1:54.26 → 1:54.47 |
| 2 | 1:01.13 → 1:01.71 | 8 | 2:07.33 → 2:07.74 |
| 3 | 1:10.75 → 1:11.50 | 9 | 2:18.78 → 2:18.99 |
| 4 | 1:25.14 → 1:25.68 | 10 | 2:24.10 → 2:24.52 |
| 5 | 1:35.64 → 1:36.18 | 11 | 2:32.16 → 2:32.41 |
| 6 | 1:46.36 → 1:46.90 | 12 | 2:41.98 → 2:42.40 |

Os vídeos estão em H.264 + AAC (MP4), que tocam em qualquer navegador e sistema.

## Estrutura

```
ABRIR APRESENTACAO.html   o player (HTML, CSS e JavaScript num arquivo só)
icone.png                 ícone da aba
videos/00.mp4 … 13.mp4    intro + 13 falas
```
