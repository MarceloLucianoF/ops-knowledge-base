# Ops Knowledge Base (DevOps / SRE)

Repositório público de conhecimento voltado para operações, confiabilidade e práticas modernas de DevOps/SRE.

Este projeto consolida runbooks, troubleshooting estruturado, padrões de CI/CD, GitOps, SLOs e boas práticas de engenharia de confiabilidade.

---

## 🎯 Objetivos

- Diagnóstico estruturado e repetível (reduzir MTTR)
- Padronização de resposta a incidentes (SEV, IC, Postmortem)
- Implementação prática de SLO/SLI e Error Budgets
- Boas práticas de CI/CD e estratégias de release/rollback
- Aplicação de princípios GitOps
- Segurança por padrão (conteúdo sanitizado)

---

## 📂 Estrutura do Repositório

### `sre/`
Princípios e fundamentos de confiabilidade:
- Severidade de incidentes (SEV)
- Incident Command
- Golden Signals
- SLI / SLO / SLA
- Error Budgets
- Filosofia de alertas
- Change management

### `runbooks/`
Templates e guias operacionais:
- Incident template
- Postmortem (blameless)
- Deploy checklist
- Rollback runbook
- Change risk assessment

### `linux/`
Operação e troubleshooting de hosts Linux:
- Health checks
- Diagnóstico por sintoma (latência, serviço down, disco cheio, rede)
- Performance (CPU, memória, I/O)
- Hardening básico

### `docker/`
Operações e segurança de containers:
- Debug
- Hardening
- Boas práticas operacionais

### `postgresql/`
Banco de dados sob ótica operacional:
- Health checks
- Performance (slow queries)
- Backup & restore

### `networking/`
Diagnóstico e fundamentos:
- DNS
- SSH / Tunneling
- VPN (WireGuard)
- Firewall

### `cicd/`
Práticas modernas de entrega contínua:
- Pipeline blueprint
- Quality gates
- Versionamento (SemVer)
- Estratégias de release (Rolling, Blue/Green, Canary)
- Rollback strategy
- GitOps (Argo / Flux)

---

## 📈 Abordagem

Este repositório segue princípios práticos de SRE:

- Mitigar primeiro, investigar depois
- Alertar por impacto ao usuário
- Versionar e auditar mudanças
- Deploys reversíveis
- Melhoria contínua via postmortem

---

## 🔐 Nota de Segurança

Este repositório **não contém**:
- IPs reais
- Hostnames corporativos
- Credenciais
- Logs produtivos
- Detalhes internos de ambientes empresariais

Todo conteúdo é genérico e sanitizado, com fins educacionais e técnicos.

---

## 🏗 Público-alvo

- DevOps Engineers
- SREs
- Analistas de Infraestrutura
- Profissionais de Operações
- Times que desejam estruturar confiabilidade operacional

---

## 📌 Status

Em evolução contínua — novas seções e aprofundamentos são adicionados progressivamente.