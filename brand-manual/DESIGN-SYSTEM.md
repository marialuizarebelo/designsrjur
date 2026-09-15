# SRJUR — Design System (v1)

> Este documento reúne todos os valores do manual de marca (canvas: https://claude.ai/artifact/JJHZvJGfsWnhrVEpG9EjPF) prontos para você inserir manualmente ao criar/editar um Design System no Claude Design (claude.ai/design).
>
> **Importante:** o canvas montado no Claude Code é uma prévia isolada — não existe um botão de "exportar direto para o Claude Design". Os valores abaixo são o conteúdo a colar/configurar lá.

---

## 1. Cores

| Token | Hex | Uso |
|---|---|---|
| `navy` | `#14213D` | Cor de base — fundo dominante |
| `navy-deep` | `#0B1526` | Extremo escuro de gradientes |
| `navy-mid` | `#1A2C52` | Meio de gradientes |
| `navy-light` | `#26406E` | Superfícies elevadas, extremo claro de gradientes |
| `cream` | `#F5F1E6` | Texto sobre navy e respiros claros — nunca fundo dominante |
| `wine` | `#8B3F42` | Ação e destaque pontual — nunca em área grande |
| `wine-light` | `#A6565A` | Hover / glow do wine |
| `text-secondary` | `#98A2BC` | Texto secundário sobre navy |

**Status/categorias:**

| Token | Hex |
|---|---|
| `status-active` | `#6E9C7D` |
| `status-pending` | `#D9A441` |
| `status-overdue` | `#D96C87` |
| `status-info` | `#8577C9` |

**Regra de proporção:** navy domina (fundo, a maior parte do peso visual); cream aparece como respiro raro; wine só como acento pontual (CTA, chamada, glow) — nunca em área grande.

---

## 2. Tipografia

| Papel | Fonte | Peso(s) | Import (Google Fonts) |
|---|---|---|---|
| Display / editorial | **Italiana** | 400 | `https://fonts.googleapis.com/css2?family=Italiana&display=swap` |
| Interface / corpo | **Manrope** | 400–800 | `https://fonts.googleapis.com/css2?family=Manrope:wght@400;500;600;700;800&display=swap` |
| Acento manuscrito (raro) | **Cedarville Cursive** | 400 | `https://fonts.googleapis.com/css2?family=Cedarville+Cursive&display=swap` |

**Escala:**
- Hero/capa: Italiana, 168px, `letter-spacing: 0.03em`
- H1 editorial (Mm): Italiana, 56px
- H1 monumental (MM): Italiana, 38px, `letter-spacing: 0.08em`, caixa alta
- H2 seção: Manrope ExtraBold (800), 36px
- Subtítulo: Manrope Bold (700), 22px
- Corpo: Manrope Regular (400), 16px
- Rótulo de UI: Manrope Bold (700), 12px, `letter-spacing: 0.1em`, caixa alta

**Regra de ênfase (escrita):** dentro de uma mesma frase, deixe 1–2 palavras maiores e/ou na fonte display para criar ritmo — ex.: *"Advocacia com **clareza** — do escritório ao `hub digital`."* Não repita esse recurso em toda frase; use com intenção.

**Cedarville Cursive:** só para uma assinatura ou recado curtíssimo. Nunca em título, nunca em bloco de texto corrido.

---

## 3. Logo

- **Formato:** selo circular (não quadrado)
- **Preenchimento:** gradiente `linear-gradient(160deg, #26406E, #14213D)`
- **Anel interno:** `box-shadow: 0 0 0 1px rgba(245,241,230,0.2) inset`
- **Conteúdo:** "SRjur" em Italiana, cor única `#F5F1E6`, `letter-spacing: -0.08em` (tracking apertado, uma peça só — nunca duas cores/posições soltas)
- **Área de proteção:** metade do diâmetro do selo, livre ao redor
- **Tamanho mínimo:** 28px de diâmetro em telas
- **Não fazer:** distorcer, recolorir fora da paleta, aplicar sobre fundo sem contraste, rotacionar

> Nota: este é o logo provisório do manual. Você mencionou que pode desenhar a versão final e me enviar depois — quando tiver, é só mandar que eu substituo aqui.

---

## 4. Raios, sombras e vidro (glassmorphism)

| Token | Valor |
|---|---|
| `radius-seal` | `50%` |
| `radius-card` | `20px–28px` |
| `radius-button` | `14px` |
| `radius-pill` | `999px` |
| `radius-tile` | `10px–16px` |
| `shadow-card` | `0 20px 50px -28px rgba(0,0,0,0.6)` |
| `shadow-card-deep` | `0 24px 60px -30px rgba(0,0,0,0.6)` |
| `shadow-button-glow` | `0 16px 30px -14px rgba(139,63,66,0.55)` |
| `glass-surface` | `rgba(245,241,230,0.05)` + `backdrop-filter: blur(24px)` + borda `rgba(245,241,230,0.12)` |

---

## 5. Componentes de produto

- **Botão primário:** gradiente wine (`#A6565A` → `#8B3F42`), texto cream, `radius: 14px`
- **Botão secundário:** superfície de vidro, borda sutil, texto cream, `radius: 14px`
- **Badge de status:** pílula (`radius: 999px`), texto 12px/700, cores por status (tabela acima)
- **Card:** superfície de vidro sobre navy, `radius: 20-28px`, sombra difusa

---

## 6. Voz e tom

**Pilares:** Clareza · Proximidade · Organização leve

**Fazer:** frases diretas, primeira pessoa, referências reais do dia a dia jurídico, humor sutil quando cabe.

**Evitar:** juridiquês desnecessário, jargão de startup vazio, tom professoral, promessas genéricas.

---

## 7. Ritmo do Instagram

- Navy domina o feed (educativo/institucional)
- Wine aparece a cada 3–4 posts, como chamada ou novidade
- Cream é raro — um respiro claro a cada 8–10 posts
- Assimetria com intenção: um único elemento "fora do grid" por peça (ex.: card levemente inclinado), nunca vários soltos ao mesmo tempo

---

## Como usar no Claude Design

1. Abra claude.ai/design e crie (ou edite) o Design System do SRJUR.
2. Cadastre as cores da seção 1 como tokens/paleta.
3. Cadastre as fontes da seção 2 (os links de import do Google Fonts estão prontos para colar).
4. Registre os raios e sombras da seção 4 como tokens de espaçamento/elevação, se o Claude Design suportar esse tipo de token.
5. Suba o logo (quando tiver a versão final) como asset da marca.
6. Use a seção 6 como guia de voz ao gerar conteúdo/textos dentro do Claude Design.

Arquivo irmão `design-tokens.json` traz os mesmos valores em formato estruturado, caso prefira importar programaticamente em outro lugar.
