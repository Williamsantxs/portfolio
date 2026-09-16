# Portfólio

Meu site pessoal, com os projetos que entreguei e o que estou construindo.

**[williamsantos.dev.br](https://williamsantos.dev.br)**

---

## Sobre o projeto

Página única, em HTML, CSS e JavaScript puro. Sem framework, sem build, sem
dependência de pacote — o site inteiro são um `index.html` e a pasta `assets/`.

## Decisões técnicas

**Sem framework.** Uma página estática, sem estado e sem rota. Qualquer camada a
mais só aumentaria o tempo de carregamento de uma página cujo trabalho é abrir
rápido no celular de quem está lendo.

**Fontes auto-hospedadas.** Syne nos títulos, Inter Tight no texto, servidas em
`.woff2` do próprio site. Baixei apenas os pesos que a página usa e apenas o
subconjunto `latin` — o `latin-ext` cobre caracteres do leste europeu e não
serve para português. Só isso economizou 130 KB, mais que o peso de todas as
fontes que ficaram.

**Imagens em WebP**, com `width` e `height` declarados em todas as tags. Sem as
dimensões, o navegador não sabe o espaço a reservar e a página salta enquanto
carrega.

Os prints dos projetos são recortes do topo de cada site, em 1200×760. As
capturas de página inteira chegavam a 2 MB cada e não entram no repositório.

**Ícones de marca.** GitHub e Instagram entram como SVG inline, com
`fill="currentColor"`, para herdarem a cor do texto. O do LinkedIn entra como
`<img>` com o arquivo oficial: as diretrizes da marca não permitem recolorir o
logo, e inline ele seria recolorido pelo CSS.

**Acessibilidade.** Um `<h1>` por página, hierarquia de títulos contínua,
`alt` em todas as imagens, `aria-hidden` nos ícones decorativos — o rótulo ao
lado já diz o que são —, foco visível no teclado e `prefers-reduced-motion`
respeitado.

**Compartilhamento.** Open Graph com imagem própria de 1200×630, gerada com a
mesma tipografia e a mesma paleta da página, para o link render miniatura no
WhatsApp e nas redes.

## Peso

| | |
|---|---|
| `index.html` | 28 KB |
| fontes | 95 KB |
| imagens | 280 KB |
| **total** | **~400 KB** |

## Estrutura

```
index.html          pagina completa, com CSS e JS embutidos
assets/
  fonts/            Syne e Inter Tight em .woff2, subset latin
  prints/           recortes do topo dos tres sites, em .webp
  icons/            icone do LinkedIn (os outros sao inline no HTML)
  william.webp      foto
  og-william.jpg    imagem de compartilhamento
  icon-*.png        favicon em 32, 180 e 512
```

## Tecnologias

`HTML5` · `CSS3` · `JavaScript` · `WebP` · `Open Graph` · `Netlify`

---

## Autor

**William dos Santos** — desenvolvedor web, Ubatuba/SP

[LinkedIn](https://www.linkedin.com/in/william-dos-santos-) ·
[GitHub](https://github.com/Williamsantxs) ·
williamdsantos.souza@gmail.com
