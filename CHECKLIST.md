# AUKAN Beauty Template — Checklist de Progresso
> Projeto: Landing Page Premium para Profissionais de Beleza
> Agência: AUKAN · aukan.com.br
> Última atualização: Abril 2025

---

## ✅ FASE 1 — Design & Código Base
- [x] Definir paleta Nude & Earth Tones (`#fdf9f5`, `#d4b896`, `#6b4c34`)
- [x] Escolher tipografia: Cormorant Garamond (Serif) + DM Sans (Sans)
- [x] Criar estrutura HTML5 com Tailwind CSS via CDN
- [x] Implementar Sticky Header com Glassmorphism
- [x] Criar seção Hero com tipografia elegante e subtítulo persuasivo
- [x] Adicionar pill de Social Proof no Hero
- [x] Criar seção Diferenciais com 3 cards + 4 métricas
- [x] Montar Bento Grid de Serviços (6 cards responsivos)
- [x] Criar seção Depoimentos com glass cards
- [x] Criar seção Contato + Formulário
- [x] Criar Footer com redes sociais
- [x] Garantir responsividade Mobile First

---

## ✅ FASE 2 — Elite Upgrade (Awwwards Style)
- [x] Grain texture via `body::after` (SVG noise, opacity 0.035)
- [x] Letter-spacing `-0.03em` em H1 e H2
- [x] Line-height `1.8` no body
- [x] Formas orgânicas (arcos) em cards alternados do Bento Grid
- [x] Integrar GSAP via CDN
- [x] Efeito line-mask clip reveal no H1 do Hero
- [x] Parallax suave nas imagens da Bento Grid (ScrollTrigger)
- [x] Substituir todas as transições por `cubic-bezier(0.23, 1, 0.32, 1)`
- [x] Animação de entrada do header com stagger
- [x] Glow suave nos botões CTA ao hover

---

## ✅ FASE 3 — Template Replicável
- [x] Criar estrutura de pastas `assets/img/hero|servicos|depoimentos`
- [x] Substituir URLs Unsplash por caminhos `assets/img/` com fallback `onerror`
- [x] Criar `css/config-cliente.css` com todas as variáveis CSS centralizadas
- [x] Documentar paletas pré-definidas por nicho no config
- [x] Marcar todos os pontos de edição com comentários `[CLIENTE]`
- [x] Salvar template validado na memória do Claude

---

## ⬜ FASE 4 — Publicação & Backend
- [ ] Substituir imagens Unsplash pelas fotos reais da cliente
- [ ] Preencher dados reais: nome, telefone, endereço, WhatsApp, Instagram
- [ ] Comprimir imagens (max 300KB cada — tinypng.com ou squoosh.app)
- [ ] Subir pasta completa na Hostinger (File Manager ou FTP/FileZilla)
  - Caminho sugerido: `public_html/clientes/isabelle-moura/`
- [ ] Testar acesso via URL: `aukan.com.br/clientes/isabelle-moura`
- [ ] Conectar formulário ao backend (opção A: Make.com → Google Sheets + WhatsApp)
- [ ] Conectar formulário ao backend (opção B: PHP mail da Hostinger)
- [ ] Validar formulário no lado cliente (campos obrigatórios)

---

## ⬜ FASE 5 — Captação de Clientes com o Template
- [ ] Criar versão demo pública do template no domínio AUKAN
- [ ] Gravar vídeo de 60s mostrando o template em ação (Reels/TikTok)
- [ ] Definir pacote de preços: Landing Page Premium = R$800–R$1.500
- [ ] Listar 10 cabeleireiras/esteticistas premium em SJC para prospectar
- [ ] Enviar DM no Instagram com preview ao vivo para 3 prospects/semana
- [ ] Montar proposta comercial padrão PDF (AUKAN)

---

## ⬜ FASE 6 — Bundle com Agente WhatsApp
- [ ] Adaptar agente FAQ (boutique feminina) para nicho de salão de beleza
- [ ] Criar fluxo Make: formulário → lead no Google Sheets → notificação WhatsApp
- [ ] Criar fluxo Make: resposta automática para novos leads via Z-API
- [ ] Montar oferta bundle: Landing Page + Agente WhatsApp = R$1.800–R$2.500/mês
- [ ] Pilotar bundle com cliente real (custo zero — usar irmã ou parceira)
- [ ] Documentar resultados para usar como case de vendas

---

## ⬜ FASE 7 — Expansão para Outros Nichos
- [ ] Adaptar template para Clínica Estética / SPA (paleta Sage & Marble)
- [ ] Adaptar template para Personal Trainer (paleta Steel & Energy)
- [ ] Adaptar template para Fotógrafo (Dark Matte — template escuro AUKAN)
- [ ] Adaptar template para Arquitetura / Interiores (paleta Warm White)
- [ ] Criar sistema de onboarding: formulário Google Forms → Claude gera copy personalizada

---

## ESTRUTURA DE ARQUIVOS DO TEMPLATE

```
aukan-beauty-template/
│
├── index.html                  ← página principal
├── css/
│   └── config-cliente.css      ← variáveis e paleta (editar por cliente)
│
└── assets/
    ├── img/
    │   ├── hero/
    │   │   └── hero-bg.jpg     ← fundo do Hero (1800×1200px min)
    │   ├── servicos/
    │   │   ├── servico-01.jpg  ← Bento card grande
    │   │   ├── servico-02.jpg  ← Card arco
    │   │   ├── servico-03.jpg
    │   │   ├── servico-04.jpg
    │   │   ├── servico-05.jpg  ← Card arco direito
    │   │   └── servico-06.jpg
    │   └── depoimentos/
    │       ├── cliente-01.jpg  ← 80×80px min
    │       ├── cliente-02.jpg
    │       └── cliente-03.jpg
    └── fonts/                  ← (opcional — se usar fontes locais)
```

---

## PALETAS POR NICHO (referência rápida)

| Nicho               | `--cor-bg`  | `--cor-primaria` | `--cor-areia` |
|---------------------|-------------|------------------|---------------|
| Beleza / Cabelo     | `#fdf9f5`   | `#6b4c34`        | `#d4b896`     |
| Clínica / SPA       | `#f5f7f4`   | `#4a6741`        | `#c8d5c2`     |
| Personal Trainer    | `#f8f8f6`   | `#2c3e50`        | `#e67e22`     |
| Arquitetura         | `#fafaf8`   | `#8b7355`        | `#c4b49a`     |
| Advocacia           | `#f9f8f6`   | `#1a2744`        | `#c9a84c`     |
| Fotógrafo (dark)    | `#141414`   | `#d4b896`        | `#8a7560`     |
