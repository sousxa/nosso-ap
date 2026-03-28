# Meu AP - Documentacao do Projeto

> Planejamento financeiro imobiliario - Comparativo de dois apartamentos

---

## Estrutura do Projeto

```
meu-ap/
├── index.html      ← App completo (single-file React via CDN)
├── .nojekyll       ← Para GitHub Pages processar corretamente
└── DOCS.md         ← Este arquivo (documentacao)
```

## Stack Tecnica

- **Framework:** React 18 via CDN (sem build step)
- **Transpiler:** Babel Standalone (JSX no browser)
- **Fontes:** DM Sans + JetBrains Mono (Google Fonts)
- **Icones:** Lucide React via CDN
- **Persistencia:** localStorage (anotacoes) + sessionStorage (sessao login)
- **Deploy:** GitHub Pages (gratuito)

## Telas do App

| # | Tela | Descricao | Status |
|---|------|-----------|--------|
| 1 | Login | Tela de senha simples (frontend only) | Pronto |
| 2 | Dashboard | Cards comparativos, contagem regressiva, progresso | Pronto |
| 3 | Cronograma | Timeline mes a mes com marcos importantes | Pronto |
| 4 | Simulador | Sliders interativos para INCC, juros, prazo, FGTS | Pronto |
| 5 | Anotacoes | Notas com categorias, salvas em localStorage | Pronto |
| 6 | FAQ | Perguntas e respostas em accordion | Pronto |

## Funcionalidades

- **Dark/Light Mode:** Toggle no header, preferencia salva em localStorage
- **Senha de acesso:** `joao2026` (validacao frontend)
- **Sessao:** sessionStorage (fecha aba = desloga)
- **Anotacoes persistentes:** localStorage
- **Simulador em tempo real:** Calculos SAC com sliders
- **Responsivo:** Mobile-first, funciona em celular

## Dados dos Apartamentos

### Palestra Life
- Valor: R$ 264.000,00
- Parcela pos-chave: R$ 1.978,00/mes
- Entrega: Agosto 2027 (~17 meses)

### Unique Palestra
- Valor: R$ 189.900,00
- Parcela pos-chave: R$ 958,00/mes
- Entrega: ~Setembro 2028 (~30 meses)

## Parametros Padrão do Simulador

| Parametro | Valor |
|-----------|-------|
| Taxa de juros | 9.5% a.a. + TR |
| Prazo financiamento | 30 anos (360 meses) |
| INCC | 6% a.a. |
| TR estimada | 0.1%/mes |

## Deploy

1. Subir arquivos para repositorio GitHub
2. Settings → Pages → Deploy from branch → main → / (root)
3. Acessar em: `https://SEU_USER.github.io/meu-ap/`

## Historico de Alteracoes

| Data | Alteracao |
|------|-----------|
| 2026-03-28 | Fix PDF viewer - substituido iframe por PDF.js com navegacao de paginas e zoom |
| 2026-03-27 | MVP completo - todas as 6 telas implementadas |
