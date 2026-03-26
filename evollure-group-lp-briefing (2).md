# BRIEFING — Landing Page Institucional Evollure Group (v4 FINAL)

> **COPY FINAL. Estrutura final. Pronto pra implementar.**
> Usar junto com `evollure-design-system-prompt.md` (DNA visual).

---

## CONTEXTO

| Campo | Valor |
|---|---|
| **Marca** | Evollure Group |
| **Posicionamento** | AI Sales Agency |
| **O que faz** | Soluções de IA sob medida + Marketing estratégico powered by AI |
| **Produto principal** | Evollure Intelligence (análise de calls) |
| **Ação principal** | WhatsApp comercial |
| **Sensação** | "Essa empresa é séria. Eu preciso falar com eles." |

---

## NARRATIVA DE SCROLL

| # | Seção | Energia | Fundo | Papel |
|---|---|---|---|---|
| 1 | Nav | Sutil | Transparente → solid | Orientação + CTA |
| 2 | Hero | MÁXIMA | Void + glow + grid | A promessa |
| 3 | Ticker de ferramentas | BAIXA | Carbon-950 | Credibilidade técnica |
| 4 | O Cenário | ALTA — editorial | Void | Por que IA sob medida importa |
| 5 | Como Trabalhamos | ALTA | Carbon-950 | O processo |
| 6 | Frase de Posicionamento | BAIXA — respiro | Void | Manifesto |
| 7 | Os 4 Pilares | ALTA | Carbon-950 | Método Evollure |
| 8 | Antes vs Depois | ALTA | Void | Transformação concreta |
| 9 | Para Quem | MÉDIA | Carbon-950 | Identificação |
| 10 | Stack | MÉDIA | Void | Credibilidade |
| 11 | FAQ | BAIXA | Carbon-950 | Remoção de dúvidas |
| 12 | CTA Final | MÁXIMA | Void + glow | Conversão |
| 13 | Footer | BAIXA | Void | Encerramento |

---

## SEÇÃO 1 — NAV

**Esquerda:** Orbital Knot SVG (28px) + "Evollure" (Regular 18px) + badge "Group" (mono 9px, ember).
**Direita:** "Sobre" · "Soluções" · "Para Quem" · "FAQ" + CTA "Fale Conosco" (ember).
**Comportamento:** Fixed. Transparente → solid on scroll (backdrop-blur 12px).

---

## SEÇÃO 2 — HERO ✅

**Label:** `AI SALES AGENCY`

**Headline:**
```
Inteligência artificial
projetada sob medida
para o seu negócio.
```
> "para o seu negócio." em italic ember.

**Subtítulo:**
```
Projetamos soluções de inteligência artificial
que se adaptam ao seu processo, aos seus critérios
e aos seus objetivos. Nada de prateleira.
```

**CTAs:**
- Primário: `Falar com a Evollure` → WhatsApp
- Secundário: `Conhecer soluções ↓` → scroll

**Visual direita:** SVG ecossistema (Orbital Knot central + 3 nós: Intelligence, Aquisição, Sob Medida).

**NOTA IMPORTANTE:** A ilustração SVG gerada inicialmente (Orbital Knot central ember com 3 nós conectados por linhas curvas, com ícones de onda sonora, gráfico e engrenagem) ficou EXCELENTE. Manter exatamente como foi gerada. Não alterar.

**Design desta seção:**
- Fundo void LIMPO — sem noise, sem granulado. Grid sutil opcional (.02 max).
- Glow ember atrás do SVG (radial-gradient 300px, .08)
- Headline: fade-up staggered (0.1s por linha)
- SVG: fade-in + scale 0.95→1 (0.8s, delay 0.3s)
- CTAs: fade-up (delay 0.5s)

---

## SEÇÃO 3 — TICKER DE FERRAMENTAS ✅

**Label centralizado:**
```
TECNOLOGIAS QUE IMPULSIONAM NOSSAS SOLUÇÕES
```
> Mono, 9px, c400, uppercase.

**Ferramentas (marquee looping infinito com logos):**
```
Google Ads · Replicate · Vercel · Notion · Gemini · Anthropic · ChatGPT · Claude · N8N · Meta AI
```

**Design:** Fundo carbon-950. Padding 16px. Border top/bottom 1px c800. Logos em opacity .4. Marquee lento (40s). Duplicar 2x pra seamless loop.

**Visual desta seção:**
- Cada logo é SVG inline ou ícone estilizado em c400
- Hover nos logos (se parado): opacity sobe pra 1 com transition .3s
- Separadores entre logos: " · " em c600
- O label "TECNOLOGIAS..." aparece acima com fade-in ao entrar no viewport
- Background: carbon-950 sólido, sem grid, sem glow — seção limpa e rápida

---

## SEÇÃO 4 — O CENÁRIO ✅

**Label:** `O CENÁRIO`

**Headline:**
```
Ferramentas, qualquer empresa tem.
Inteligência aplicada ao seu negócio, não.
```
> "não." em italic ember.

**Corpo:**
```
O mercado está cheio de soluções prontas
que não conhecem a sua operação.

A Evollure não promete. Constrói.
Do diagnóstico à entrega. Do zero. Funcionando.
```

**Punchline (20px, bold):**
```
Não adaptamos soluções prontas.
Construímos a sua.
```
> "a sua." em italic ember.

**Sem cards. Seção editorial pura.**

**Design desta seção:**
- Fundo void LIMPO — sem noise, sem granulado, sem textura
- Glow ember sutil centralizado (radial-gradient 400px, .04) — SUTIL, quase imperceptível
- Headline: fade-up staggered
- **NOTA:** O espaçamento entre "Ferramentas, qualquer empresa tem." e "Inteligência aplicada ao seu negócio, não." deve ser visualmente unificado — as duas linhas pertencem ao mesmo headline, não devem parecer blocos separados. Line-height 1.15 no headline inteiro.
- Corpo: fade-up (delay 0.2s)
- Punchline: delay 0.4s, peso visual separado (margin-top 32px)
- Divider ember (1px, gradient transparent→ember→transparent) entre corpo e punchline
- Padding 120px vertical — respiro editorial
- Max-width 640px centralizado

---

## SEÇÃO 5 — COMO TRABALHAMOS ✅

**Label:** `COMO TRABALHAMOS`

**Headline:**
```
Diagnóstico. Desenho. Construção. Entrega.
```

**Corpo:**
```
Antes de escrever uma linha de código,
entendemos a sua operação. Seus critérios.
Seus gargalos. Seu processo de vendas.

Depois construímos a solução que resolve
exatamente o que precisa ser resolvido.
Sem escopo inflado. Sem feature que ninguém usa.
```

**Visual:** 4 steps conectados por path ember (01→02→03→04).

**Design desta seção:**
- Fundo carbon-950 LIMPO
- **NOTA CRÍTICA:** A animação do path deve ser SIMPLES. Se a ferramenta não renderizar corretamente o path draw-on, usar abordagem estável: 4 blocos horizontais com número + título + descrição, separados por seta "→" ember estática entre eles. Sem path SVG complexo.
- **Abordagem recomendada (estável):** 4 colunas horizontais (desktop) ou 4 rows verticais (mobile). Cada bloco: número mono ember grande (01, 02, 03, 04) + título bold + descrição c300. Seta "→" ember entre cada bloco.
- **Se path SVG funcionar:** 4 nós circulares conectados por linha horizontal ember. Path se desenha suavemente. Nós aparecem com stagger.
- Ember glow sutil atrás do bloco central (.03)
- Fade-up staggered nos blocos

---

## SEÇÃO 6 — FRASE DE POSICIONAMENTO ✅

> Seção de respiro. Só tipografia. Zero decoração. Muito espaço negativo.

**Corpo (3 linhas, 15px, c400):**
```
Não acreditamos em IA genérica.
Não acreditamos em automação sem contexto.
Não acreditamos em soluções que não geram números claros.
```

**Punchline (20px, bold, white):**
```
A Evollure existe para transformar complexidade operacional
em eficiência mensurável e estratégica.
```

**Design:** Fundo void. Padding 120px+. Centralizado. Max-width 640px.

**Design desta seção:**
- Fundo void limpo — ZERO decoração visual. O silêncio é o design.
- As 3 linhas "Não acreditamos..." entram uma por vez com stagger 0.3s (fade-up)
- Punchline entra por último com delay 1s e peso visual maior
- Divider ember sutil (60px, 1.5px) entre as 3 linhas e a punchline
- Tipografia é a única arma: c400 nas negações, white bold na punchline
- Seção de respiro entre duas seções densas — padding generoso obrigatório

---

## SEÇÃO 7 — OS 4 PILARES DO MÉTODO EVOLLURE ✅

**Label:** `MÉTODO EVOLLURE`

**Headline:**
```
Os 4 pilares do Método Evollure.
```

**4 pilares:**

```
01 — Imersão no seu negócio
Entendemos a fundo seus processos, gargalos
e onde a inteligência artificial gera impacto real.
Não começamos pelo código. Começamos por você.

02 — Diagnóstico estratégico
Mapeamos onde a IA entra com mais força e menos
esforço operacional. Sem achismo. Com dados.

03 — Desenvolvimento sob medida
Construímos soluções de IA e estratégias de aquisição
personalizadas. Alinhadas à sua operação, aos seus
critérios e aos seus objetivos.

04 — Escala com resultados
Cada solução entregue gera ganhos mensuráveis.
Automáticos. Sustentáveis. Visíveis no dashboard
e no caixa.
```

**Composição visual:** Orbital Knot centralizado (grande, ember) com 4 nós ao redor:
- `imersao_ia ()` · 1
- `diagnostico_para_ia ()` · 2
- `desenvolver_ia ()` · 3
- `escalar_com_ia ()` · 4
**Composição visual:** Orbital Knot centralizado (grande, ember) com 4 nós ao redor:
- `imersao_ia ()` · 1
- `diagnostico_para_ia ()` · 2
- `desenvolver_ia ()` · 3
- `escalar_com_ia ()` · 4
Linhas curvas conectando os nós ao centro. Paleta Carbon + Ember.

**Design desta seção:**
- Fundo carbon-950 LIMPO
- **NOTA CRÍTICA:** Esta composição visual deve ser SIMPLES e ESTÁVEL. Se a ferramenta não conseguir renderizar corretamente o Orbital Knot com 4 nós conectados, simplificar para: 4 cards em grid 2×2 com numeração 01-04 em mono ember, com Orbital Knot estático centralizado acima dos cards (sem linhas de conexão). A prioridade é estabilidade visual, não complexidade.
- **Fallback estável:** 4 cards em grid 2×2. Cada card: bg carbon-900, border 1px c800, border-left 3px ember. Número (01, 02, 03, 04) em mono ember 24px no topo do card. Título bold. Descrição c300.
- Cards entram com fade-up staggered 0.15s
- Hover: border-color ember + translateY(-3px)

---

## SEÇÃO 8 — ANTES VS DEPOIS DA EVOLLURE ✅

**Headline:**
```
Antes vs Depois da Evollure.
```

**5 cards ANTES → DEPOIS:**

**1.**
ANTES: Tentando entender IA no meio do hype e das promessas vazias
DEPOIS: Agentes de IA sob medida, criados para atuar na sua rotina e nos seus processos específicos

**2.**
ANTES: Gastando tempo e dinheiro com processos manuais e retrabalho
DEPOIS: Processos críticos automatizados, custos reduzidos, equipe focada em atividades de alto impacto

**3.**
ANTES: Contratando mais pessoas para dar conta do crescimento
DEPOIS: Operações escaladas sem aumentar o time, com IA trabalhando 24/7

**4.**
ANTES: Recebendo dados sem saber como transformá-los em decisões estratégicas
DEPOIS: Dados transformados em insights acionáveis, decisões rápidas e precisas

**5.**
ANTES: Dependendo de soluções genéricas que não se adaptam à operação
DEPOIS: Soluções integradas, adaptadas à sua operação e aos seus objetivos estratégicos

**Design:** Cards ANTES: label vermelho sutil, borda c800. Cards DEPOIS: label ember, borda ember, bg ember-dim. Seta → entre cada par. Grid 2 colunas desktop, empilhado mobile.

**Design desta seção:**
- Fundo void com grid sutil (60px, ember .02)
- **Layout:** 5 rows, cada row tem 2 cards lado a lado (ANTES à esquerda, DEPOIS à direita) com seta "→" ember entre eles
- **Card ANTES:** bg carbon-950, border 1px c800. Label "ANTES" em mono 8px vermelho sutil (#EF4444 30% opacity). Texto em c400, 13px.
- **Card DEPOIS:** bg rgba(232,87,15,.03), border 1px rgba(232,87,15,.15). Label "DEPOIS" em mono 8px ember. Texto em c100, 13px.
- **Seta entre cards:** "→" em ember, 16px, centralizado verticalmente
- **Animação:** Cada row entra com fade-up staggered (0.15s entre rows). Card ANTES aparece primeiro, depois a seta, depois card DEPOIS (micro-stagger 0.1s)
- **Hover:** Card DEPOIS ganha border-color ember mais forte + translateY(-2px)
- No mobile: cards empilham verticalmente (ANTES em cima, seta ↓ no meio, DEPOIS embaixo)

---

## SEÇÃO 9 — PARA QUEM

**Label:** `PARA QUEM É A EVOLLURE`

**Headline:**
```
Se a sua operação comercial
envolve conversa, a Evollure
foi feita pra você.
```
> "pra você." em italic ember.

**6 cards grid 3×2:**

1. **Franquias** — "Padronize qualidade de vendas em todas as unidades. Mesmo script, mesmo critério, visibilidade total."
2. **Seguros e financeiro** — "Calls complexas que exigem técnica, compliance e argumentação de valor."
3. **Energia solar** — "Venda consultiva de alto ticket. Ciclo longo. Cada call cirúrgica."
4. **SaaS e tecnologia** — "Demos, trials, onboarding. Meça aderência ao playbook e otimize conversão."
5. **Clínicas e saúde** — "Agendamento é venda. Atendimento é retenção. Meça os dois."
6. **Educação e cursos** — "Matrícula é venda. Objeções específicas. Técnica necessária."

**Design desta seção:**
- Fundo carbon-950
- **Grid 3×2** desktop, 2×3 tablet, 1×6 mobile
- Cada card: bg carbon-900, border 1px c800, **border-left 3px ember**, padding 24px
- **Ícone SVG** geométrico no topo (24px, ember): grid (franquias), escudo (seguros), sol (solar), terminal (SaaS), cruz (saúde), livro (educação)
- Título: 16px bold white. Descrição: 13px c300.
- **Animação:** Cards entram com fade-up staggered (0.1s entre cards)
- **Hover:** border-color ember inteira + translateY(-3px)

---

## SEÇÃO 10 — STACK E PROFISSIONALISMO

**Label:** `COMO ENTREGAMOS`

**Headline:**
```
Tecnologia de ponta.
Execução impecável.
```
> "impecável." em italic ember.

**Corpo:**
```
Por trás de cada solução existe uma stack robusta,
segura e escalável. Você não precisa saber o que roda
por trás. Precisa saber que funciona, que é seguro,
e que tem gente séria cuidando da sua operação.
```

**4 cards:**
1. **Cloud robusta** — "Deploy contínuo. Monitoramento. Escalabilidade sob demanda."
2. **LGPD compliant** — "Dados criptografados. Compliance total. Zero vazamento."
3. **Sob medida** — "Código proprietário. Engenharia pro seu negócio. Não é plugin."
4. **Suporte dedicado** — "Onboarding assistido. Canal direto. Gente real."

**Design desta seção:**
- Fundo void
- **Grid 4×1** desktop, 2×2 tablet, 1×4 mobile
- Cada card: bg carbon-950, border 1px c800, padding 24px, text-align center
- **Ícone SVG** no topo de cada card (20px, c400): server (cloud), shield (LGPD), wrench (sob medida), headset (suporte)
- Label mono ember 8px no topo de cada card
- Título: 14px bold. Descrição: 12px c300.
- **Animação:** Cards fade-up staggered 0.1s
- **Hover:** border-color ember + transition .25s
- Sem glow, sem grid. Seção limpa e funcional.

---

## SEÇÃO 11 — FAQ

**Label:** `PERGUNTAS FREQUENTES`

**Headline:**
```
Dúvidas? A gente responde
sem rodeio.
```
> "sem rodeio." em italic ember.

**10 perguntas:**

Q1: `O que é a Evollure Group?`
A1: `Uma AI Sales Agency. Aplicamos inteligência artificial sob medida em operações comerciais. Da geração de demanda até a análise de cada conversa de vendas.`

Q2: `O que é o Evollure Intelligence?`
A2: `Nosso produto principal. Analisa automaticamente cada call do time de vendas contra os critérios definidos pela sua empresa. Scores, rankings, tendências e insights de coaching em um dashboard.`

Q3: `Vocês fazem marketing e mídia paga?`
A3: `Sim. Estratégia de aquisição e mídia de performance potencializada por IA. Google, Meta, LinkedIn. Segmentação inteligente, otimização de criativos e rastreamento até a conversão. Brasil e exterior.`

Q4: `O que significa "sob medida"?`
A4: `Não temos produto de prateleira. Cada solução é construída do zero em torno da operação do cliente. Critérios, automações, integrações, estratégia. Tudo desenhado pro seu negócio.`

Q5: `Preciso de conhecimento técnico?`
A5: `Nenhum. Onboarding 100% assistido. Configuramos tudo. Treinamos a equipe. Você usa o dashboard e toma decisão. O técnico fica com a gente.`

Q6: `Funciona pra qualquer tipo de empresa?`
A6: `Funciona pra qualquer operação que envolva conversa. Call, videochamada, atendimento. Se tem vendedor e tem conversa, a Evollure potencializa.`

Q7: `Quanto custa?`
A7: `Depende do escopo. Não temos plano fixo. Cada proposta é construída após entendermos a operação. Fala com a gente pelo WhatsApp. Sem compromisso.`

Q8: `Meus dados estão seguros?`
A8: `100%. Infraestrutura cloud, criptografia em trânsito e em repouso, compliance com LGPD. Segurança é premissa, não feature.`

Q9: `Vocês atendem fora do Brasil?`
A9: `Sim. Operações em português e inglês. Mídia no Brasil e exterior. O Intelligence funciona em qualquer idioma.`

Q10: `Como começo?`
A10: `WhatsApp. 15 minutos pra entender sua operação. Sem pitch. Sem slide de 40 páginas. Só conversa honesta.`

**Design desta seção:**
- Fundo carbon-950
- **Accordion funcional** (JavaScript onclick toggle)
- Pergunta: 16px bold white. Ícone "+" à direita que rotaciona pra "×" ao abrir (transition .3s).
- Resposta: 14px c300, max-height 0 → auto com transition .4s
- Border-bottom 1px c800 entre cada item
- **Hover na pergunta:** color ember
- Item aberto: ícone muda pra ember
- Max-width 680px centralizado
- **Animação:** Accordion inteiro fade-up ao entrar no viewport

---

## SEÇÃO 12 — CTA FINAL

**Orbital Knot SVG** fundo: 240px, opacity .08.
**Glow:** radial-gradient 500px, opacity 12%.

**Headline:**
```
O achismo tem prazo de validade.
Fala com a Evollure.
```
> "Evollure." em italic ember.

**Subtítulo:**
```
15 minutos de conversa. Sem compromisso. Sem pitch.
Só uma análise honesta de como IA pode transformar
a sua operação comercial.
```

**CTA:** `Falar pelo WhatsApp` — ember, cantos retos, 16px.

**Micro-copy:** `15 minutos · Sem compromisso · Conversa direta`

**Design desta seção:**
- Fundo void
- **Orbital Knot SVG** centralizado atrás do headline: 240px, opacity .08
- **Glow ember máximo da página:** radial-gradient 500px, opacity .12
- Grid sutil no fundo (60px, ember .02)
- Headline: fade-up. Subtítulo: fade-up delay 0.2s. Botão: fade-up delay 0.4s.
- **Botão CTA grande:** padding 16px 48px, bg ember, color white, cantos retos. Hover: bg white, color void.
- Micro-copy: mono 10px c400 centralizado
- Padding vertical 120px+ — clímax visual da página

---

## SEÇÃO 13 — FOOTER

**Esquerda:** Orbital Knot (20px) + "Evollure" (Regular 16px) + "AI Sales Agency" (mono 9px c400).
**Centro:** Intelligence · Sobre · Para Quem · FAQ · Contato
**Direita:** © 2026 Evollure Group. Social: Instagram · LinkedIn · YouTube.

---

## REGRAS VISUAIS GLOBAIS

> **CLEAN E TECNOLÓGICO.** O fundo deve ser limpo, sem texturas granuladas ou noise pesado. A identidade da Evollure é precisão e tecnologia — não grunge. Cada seção deve ter pelo menos um elemento visual que a diferencia: cards, SVG, animação, composição, ou efeito. Mas o fundo é sempre limpo.

**FUNDO — REGRA ABSOLUTA:**
- Fundo LIMPO. Sem noise pesado. Sem granulado. Sem texturas que pareçam "sujo".
- Grid sutil permitido (opacity .015 a .025 máximo)
- Glow ember pontual permitido (radial-gradient, opacity .04 a .08)
- Se usar noise, opacity MÁXIMA de .01 — quase imperceptível
- O visual deve parecer tecnológico, clean, como painel de controle premium — não como textura de papel ou grunge
- Referência: a LP do Evollure Intelligence em produção (https://matheuscristofolli.github.io/evollure-intelligence-landing-page/) tem o padrão correto de fundo

**Animações globais (scroll-triggered via Intersection Observer):**
- Fade-up: elementos sobem 20px com opacity 0→1, 0.6s ease-out
- Stagger: elementos irmãos entram com delay de 0.1s entre eles
- Path draw-on: SVGs com stroke-dashoffset se desenham conforme scroll
- Todas as animações são sutis e elegantes. Nada bouncy. Nada rápido.
- **IMPORTANTE:** Animações devem ser SIMPLES e ESTÁVEIS. Se uma animação não renderiza bem, é melhor não ter animação do que ter uma quebrada.

**Texturas por seção:**
- Seções em void: grid sutil OPCIONAL (60px, ember .02 opacity MAX)
- Seções em carbon-950: sem grid, profundidade via gradiente suave e glow pontual
- **SEM noise texture pesado em nenhuma seção**

---
## REGRAS DE IMPLEMENTAÇÃO

1. Seguir 100% o `evollure-design-system-prompt.md`
2. PP Neue Montreal + IBM Plex Mono
3. Carbon + Ember. 90/10.
4. Cantos retos. Sem sombras.
5. CTA = WhatsApp. Aparece: nav + hero + CTA final.
6. NUNCA mencionar Whisper, GPT, OpenAI.
7. SVGs inline, originais.
8. Tudo em um único arquivo HTML.
9. "AI Sales Agency" é badge/conceito.
10. Resultado > tecnologia. Sempre.
11. **FUNDO LIMPO.** Sem noise pesado. Sem granulado. Sem textura que pareça sujeira. Clean e tecnológico.
12. **ANIMAÇÕES ESTÁVEIS.** Se uma animação não renderiza corretamente, usar o fallback estável descrito na seção. Melhor sem animação do que com animação bugada.
13. **ILUSTRAÇÃO SVG DO HERO:** Manter a composição gerada (Orbital Knot + 3 nós). Não alterar.
14. **PRIORIDADE:** Estabilidade visual > complexidade. Clean > decorado. Funcional > impressionante.
