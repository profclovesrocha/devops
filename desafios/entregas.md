# DATAS DAS ENTREGAS
- 1. DESAFIO 1: 04/MAR/2026 (Formação de Equipe e Tema).
- 2. DESAFIO 2: 11/MAR/2026 (da AULA 3).
- 3. DESAFIO 3: 18/MAR/2026 (da AULA 4).
- 4. DESAFIO 4: 25/MAR/2026 (da AULA 6).
- 5. DESAFIO FINAL: 10/JUNHO/2026 (AV2 - EM SALA)
- 6. Link em destaque INSCRIÇÕES | FACEPE E SECTI EDITAL COMPET 14/2026: https://forms.gle/zD3ZLcyEcpTMdEfn7

# 🎓 Desafio Final: Seminário DevOps e Observabilidade 360°
# Tema: "Arquitetura e Orquestração de Microserviços Resilientes com Foco em Observabilidade"

# 📋 Visão Geral do Desafio
As equipes (de até 5 pessoas) deverão desenvolver e apresentar uma solução tecnológica que simule um ambiente real de produção. O projeto deve sair do "funciona na minha máquina" para uma infraestrutura orquestrada, automatizada e monitorada.

# 🏗️ Requisitos Práticos (A Solução)
1.  **Desenvolvimento e Containerização:** Criar uma aplicação (ou utilizar uma existente de Smart City) e construir um **Dockerfile** otimizado, preferencialmente utilizando imagens *alpine* para menor footprint.
2.  **Pipeline CI/CD (GitHub Actions):** Configurar um workflow automatizado que execute builds, testes unitários/integração e análise estática a cada commit.
3.  **Orquestração (Kubernetes + Helm):** Realizar o deploy da aplicação em um cluster K8s utilizando **Helm**. É obrigatório o uso de um `values.yaml` para gerenciar diferentes ambientes (ex: staging e prod).
4.  **Observabilidade e Logs:** Implementar uma estratégia de **logging centralizado** (usando Syslog-ng ou Stack ELK) para evitar a perda de dados pela efemeridade dos containers. Adicionalmente, configurar métricas básicas de **APM** (latência e taxa de erro).

---

# 🎙️ Formato do Seminário (Apresentação)
O seminário deve ser dividido em quatro momentos principais, seguindo as fases de planejamento e validação:

*   **Momento 1: Defesa Teórica:** Explicar a escolha entre Containers e VMs para o cenário proposto, destacando o isolamento a nível de processo.
*   **Momento 2: Arquitetura da Solução:** Apresentar o diagrama da infraestrutura, detalhando como os **Pods, Services e Deployments** interagem no Kubernetes.
*   **Momento 3: Live Demo (O "Pulo do Gato"):** 
    *   Demonstrar um deploy bem-sucedido via Helm.
    *   Provocar propositalmente um erro no pipeline para mostrar o travamento do deploy (Qualidade Sustentável).
    *   Realizar um **Rollback** ao vivo usando comandos Helm.
*   **Momento 4: Painel de Observabilidade:** Mostrar logs sendo gerados em tempo real e visualizados centralizadamente.

---

# 📊 Critérios de Avaliação (Peso 0-10)

| Critério | Descrição | Peso |
| :--- | :--- | :--- |
| **Automação (CI/CD)** | O código principal permanece sempre em estado deployável? O pipeline bloqueia falhas? | 2.5 |
| **Orquestração (Helm)** | Uso correto de templates e parametrização via `values.yaml`. O rollback funcionou? | 2.5 |
| **Observabilidade** | Prova de persistência de logs (mesmo após destruir o container) e monitoramento de performance. | 2.5 |
| **Seminário e Didática** | Clareza na explicação, domínio dos comandos (kubectl/helm) e organização do repositório no GitHub. | 2.5 |

---

# 📂 Entrega Final
Deverá ser postado no repositório oficial da disciplina:
*   Link do repositório da equipe com o **README.md** detalhado (instruções de build e deploy).
*   Slides da apresentação (formato PDF/GML).
*   Arquivo `docker-compose.yml` (para testes locais) e pasta do **Helm Chart**.

> **Dica do Professor:** "Um sistema sem logging adequado é como dirigir um carro sem painel". Certifiquem-se de que sua aplicação tenha visibilidade total antes da apresentação final!
 
# TIMES - GRUPOS EM ANDAMENTO
- TIME 01: JOÃO VICTOR,...
- TIME 02: Pedro Gabriel, Odenir, Diego Henrique, Matheus Francisco
- TIME 03: Pedro Gutemberg e Aylana Santos
- TIME 04: Alysson Gomes, Jonnathan Mendes, Lindalva Evellyn, Matheus Peixoto, Natalia Maria, Natthan Gonçalves, Sabrina Lemos, Vitor Hugo

# SUGESTÃO - Desafios para Smart City 
- https://docs.google.com/document/d/1C0nNNBLqCDSXJoIcvWlhaoC26HUpmbETfKGtKsIpeJs/edit?usp=sharing
- EXEMPLO DE MONITORAMENTO: https://cybermap.kaspersky.com/pt
- EXEMPLOS DE PROJETOS PRONTOS: https://github.com/clovesrocha/app-ideias
