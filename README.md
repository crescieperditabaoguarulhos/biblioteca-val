# Biblioteca de Conteúdo — Val Crochês

Site estático com os 34 Reels de crochê que mais viralizaram (29/07 a 27/10/2026), cada um com capa, link para o vídeo, análise e roteiro adaptado para a Val Crochês.

## Estrutura

```
index.html   página (layout, filtros e fichas)
data.js      conteúdo: análise e roteiro de cada vídeo
capas/       capas dos Reels (J01–J19, M01–M15)
vercel.json  configuração da Vercel (sem indexação no Google, cache das capas)
```

## Editar um roteiro

Abra `data.js`, procure pelo código do vídeo (ex.: `id: "J09"`) e altere os textos. Campos entre `[colchetes]` são para preencher com a peça, o valor ou o nome real.

## Ver no computador

Abra `index.html` direto no navegador, ou rode:

```
npx serve .
```

## Publicar na Vercel

1. Suba esta pasta para um repositório no GitHub.
2. Na Vercel: **Add New → Project → Import** o repositório.
3. Framework Preset: **Other**. Não precisa de build command nem output directory.
4. Clique em **Deploy**. Cada novo commit no GitHub publica de novo automaticamente.
