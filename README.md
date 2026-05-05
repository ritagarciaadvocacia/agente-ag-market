# 57 Agents Agencia de Marketing — Claude Code para operar agencia digital

**57 subagentes especializados** para donos, AMs (account managers), traffic managers, criativos, operacoes e financeiro de **agencias de marketing digital brasileiras**, prontos para uso no Claude Code. Cada agente e um especialista em uma rotina interna da agencia — proposta comercial, brief, kickoff, status report, timesheet, churn, hiring criativo, BDI agencia, QBR — que atua proativamente quando o contexto da conversa bate com sua especialidade.

> **Importante:** este pacote NAO duplica os agents de execucao de marketing (Meta Ads, Google Ads, Instagram, lancamento, copy, SEO). Para isso, voce instala em separado os pacotes de **execucao** (skills/agents Bravy de marketing). Este pacote e o que faltava: **gerenciar uma agencia que entrega marketing**.

## Como instalar (usando os zips desta pasta)

Voce tem **57 zips individuais** + este README. Pode instalar **um a um** (so quem voce vai usar) ou **todos de uma vez**.

### Opcao A — Instalar 1 agente individual

1. Baixe o zip do agente que voce quer (ex: `01-prospeccao-outbound-LinkedIn.zip`).
2. Descompacte. Dentro tem o `.md` do agente + um `COMO-INSTALAR.md` com o passo a passo.
3. Copie o `.md` para `.claude/agents/` (no seu projeto) ou `~/.claude/agents/` (global).
4. Reinicie o Claude Code (`/exit` e abra de novo). Pronto.

### Opcao B — Instalar todos os 57 de uma vez (terminal)

```bash
cd /caminho/onde/voce/baixou/57-Agents-Agencia-Marketing
mkdir -p ~/.claude/agents
for z in *.zip; do
  unzip -o -j "$z" "*.md" -d ~/.claude/agents/ -x "COMO-INSTALAR.md"
done
```

Reinicie o Claude Code. Confirme com `/agents`.

## Como usar

- **Automatico**: "preciso fazer kickoff de um cliente que entrou hoje (e-commerce moda, R$ 30k/mes)" -> Claude delega para `kickoff-meeting-roteiro` + `onboarding-cliente-30-60-90-dias`.
- **Manual**: "use o agente `precificacao-fee-agencia` para definir fee mensal de novo prospect SaaS B2B".
- **Em pipeline**: `audit-gratuito-isca` -> `discovery-call-roteiro` -> `proposta-comercial-agencia` -> `contrato-prestacao-servico` -> `kickoff-meeting` -> `onboarding-30-60-90`.

## Catalogo (57 agentes)

### Comercial / novo cliente
01 Prospeccao outbound LinkedIn · 02 Audit gratuito como isca · 03 Discovery call · 04 RFP/RFI resposta
05 Proposta comercial agencia · 06 Precificacao fee · 07 Pitch deck novo cliente · 08 Contrato prestacao servico

### Onboarding e kickoff
09 Brief novo cliente · 10 Kickoff meeting · 11 Onboarding 30-60-90 · 12 Acesso/credenciais handover
13 SLA deliverables · 14 Account plan anual

### Gestao de delivery (project management)
15 Squad/celula cliente · 16 Sprint marketing 2 semanas · 17 Stand-up daily · 18 Status report semanal
19 Tracking ClickUp/Asana/Jira · 20 Timesheet rentabilidade · 21 Capacity planning · 22 Escalation matrix

### Reunioes e comunicacao
23 Reuniao mensal resultados · 24 QBR trimestral · 25 Ata reuniao · 26 Newsletter resultados
27 Apresentacao deck mensal · 28 Follow-up pos-reuniao

### Criacao e processo criativo
29 Brief interno criacao · 30 Fluxo aprovacao 3 rodadas · 31 Banco referencias · 32 Review criativo
33 Versionamento/naming · 34 Entrega final handover

### Financeiro / rentabilidade
35 Hora vendida vs trabalhada · 36 Rentabilidade projeto · 37 BDI agencia overhead · 38 Cobranca recorrente
39 Inadimplencia regua · 40 Forecast MRR/pipeline

### Gestao de pessoas
41 Hiring criativo PJ/CLT · 42 Freelancer marketplace · 43 Onboarding funcionario · 44 Plano carreira
45 Review trimestral 1-on-1 · 46 Retencao talento

### Cliente: retencao, expansao, churn
47 NPS/CSAT cliente · 48 Churn prevencao · 49 Win-back perdido · 50 Upsell/cross-sell
51 Case de sucesso · 52 Off-boarding cliente

### Marketing da propria agencia
53 Personal branding fundador · 54 Conteudo LinkedIn · 55 Networking/eventos · 56 Parceria white-label

### IA aplicada (NOVO)
57 IA na agencia (Claude/ChatGPT/Midjourney/Runway/HeyGen no fluxo: brief -> criacao -> entrega 3x mais rapido)

## Avisos legais

- Os agentes refletem boas praticas de mercado de agencia digital brasileira (RD Summit, ABRADi, IAB Brasil), CLT/Reforma Trabalhista, LGPD para tratamento de dados de clientes/prospects, e tabelas de mercado (referencias APRO/ABAP/Sinapro).
- Outputs gerados sao **rascunhos**; o gestor responsavel revisa antes de enviar a cliente, contratar pessoa ou assinar contrato.
- Templates e exemplos usam dados ficticios.

## Licenca

Uso permitido para clientes ASV Digital / Bravy. Nao redistribuir sem autorizacao.
