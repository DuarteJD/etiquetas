# Visualizador de Etiquetas — ZPL · EPL · PPLA

Visualiza no navegador como uma etiqueta vai sair na impressora, a partir do arquivo de comandos (.txt / .prn):

- **ZPL** — Zebra
- **EPL2** — Zebra / Elgin
- **PPLA** — Argox

Funciona 100% no navegador: nada é enviado para servidor. Também funciona sem internet (abrindo o `index.html` direto).

## Como usar

1. Abra a página.
2. Clique em **Abrir arquivo…** (ou arraste o .txt para o editor, ou cole o código).
3. Ajuste resolução (dpi) e tamanho da etiqueta se necessário.
4. Use **Baixar PNG** para salvar a imagem da etiqueta.

Comandos que o visualizador ainda não entende aparecem na lista de avisos abaixo da etiqueta.

## Estrutura

```
index.html                 página completa (HTML + CSS + JavaScript)
vendor/bwip-js-min.js      biblioteca de códigos de barras (bwip-js, licença MIT)
vendor/bwip-js-LICENSE.txt licença da bwip-js
fonts/*.woff2              fontes Roboto Condensed e Roboto Mono (licença Apache 2.0)
.nojekyll                  faz o GitHub Pages servir os arquivos sem processar
```

## Publicar no GitHub Pages

1. Crie um repositório no GitHub (ex.: `etiquetas`).
2. Envie todos os arquivos desta pasta para a raiz do repositório.
3. Em **Settings → Pages**, em *Build and deployment*, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)` e salve.
4. Em 1–2 minutos o site fica disponível em `https://SEU-USUARIO.github.io/etiquetas/`.
