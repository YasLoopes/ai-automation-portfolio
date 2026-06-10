# Portfólio — Automação & Agentes de IA

**Yasmin Lopes · Analista de CRM | Automação & Agentes de IA | HubSpot**

Interseção entre dados, processos e IA — com foco em escalar operações sem perder controle.

---

## O que este repositório mostra

Automações reais com IA em produção numa scale-up de energia, com dados sanitizados para portfólio.  
Todo o material aqui é baseado em trabalho real: resultados quantificados, arquitetura documentada, decisões registradas.

### Cases

| # | Case | Resultado principal |
|---|------|---------------------|
| 01 | [Agentes de IA no CRM com humano no loop](cases/01-agentes-ia-crm-humano-no-loop.md) | Operações manuais escalonadas com governança — zero dados corrompidos em produção |
| 02 | [Campanha segmentada: 49% de economia](cases/02-campanha-segmentada-49pct-economia.md) | Filtro de base pré-campanha reduziu disparos de 290 para 143, ~49% de economia |
| 03 | [Documentação reprodutível: 41 workflows mapeados](cases/03-documentacao-reprodutivel-41-workflows.md) | Inventário vivo de automações — base para transição de time e auditoria de processos |

## Demo — Painel de ofertas interativo

**Problema:** as ofertas da campanha do 2º trimestre eram gerenciadas num PDF de 7 páginas com mais de 30 linhas por tabela. Baixa visibilidade, difícil de filtrar, gerava retrabalho constante para o time comercial da Clarke Energia consultar as ofertas — e um gargalo adicional para os parceiros, que dependiam do time para tirar dúvidas básicas.

**Solução:** site interativo em arquivo HTML único, prototipado com Claude Code.  
Três visões alternáveis (90 dias, 180 dias, oferta especial), filtros por distribuidora/faixa de consumo/fidelidade, cards de resumo calculados em tempo real. Sem servidor, sem dependências — abre direto no navegador.

**Resultado:** time comercial passou a consultar as ofertas de forma autônoma, sem retrabalho. Parceiros conseguiram navegar pelas ofertas sem intermediação — eliminando o gargalo de atendimento para dúvidas operacionais.

→ **[Abrir demo](https://yasloopes.github.io/ai-automation-portfolio/demo-site-promocional/)** _(GitHub Pages)_

---

## Como trabalho com agentes de IA

Automação sem governança é só outra fonte de erro em escala. Meu padrão operacional:

1. **Área restrita primeiro** — o agente começa em lista/segmento de teste; efeitos contidos e reversíveis antes de escalar.
2. **Instrução step-by-step** — cada passo descrito de forma verificável, não um pedido amplo.
3. **Aba de dúvidas** — casos ambíguos são separados para validação humana antes de processar.
4. **Conferência pós-execução** — "rodou" ≠ "está certo"; resultado revisado antes de encerrar.
5. **Disciplina de custo** — base filtrada antes de qualquer disparo em volume.

Esse padrão está documentado com mais detalhe no [Case 01](cases/01-agentes-ia-crm-humano-no-loop.md).

---

## Stack

| Camada | Ferramentas |
|--------|-------------|
| CRM | HubSpot (workflows, objetos customizados, listas, propriedades) |
| IA | Claude — Cowork (agente com humano no loop) e Code (prototipagem) |
| Comunicação | WhatsApp/API, e-mail, SMS, webhooks |
| Automação | N8N, HubSpot Workflows |
| Documentação | Notion, Figma |

---

> **Aviso:** todos os dados, ofertas, códigos promocionais e condições exibidos neste repositório são fictícios ou agregados.  
> Nomes de distribuidoras são informação pública. Nenhuma informação confidencial é exposta.  
> Ver `SANITIZACAO.md` no repositório privado para o log completo.

---

_Este repositório foi montado e publicado com [Claude Code](https://claude.ai/code)._
