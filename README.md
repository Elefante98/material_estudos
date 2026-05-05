# Trilha: Infraestrutura de Software para Sistemas em Produção

## Estrutura da trilha

Três fases progressivas — cada uma pressupõe a anterior:

| Fase | Módulos | Foco |
|------|---------|------|
| **Iniciante** | 3.1 → 3.5 | Fundamentos. Obrigatórios antes de colocar qualquer coisa no ar |
| **Intermediário** | 4.1 → 4.5 | Produção real: automação, isolamento, resiliência |
| **Avançado** | 5.1 → 5.5 | Escala, missão crítica, compliance corporativo |

> **Nota sobre os arquivos numerados:** Os números `01`–`12` são apenas referência. Vários livros atravessam múltiplos módulos — você voltará a eles em fases diferentes. Não leia cada livro do início ao fim antes de avançar de fase.

---

## Fase Iniciante — Fundamentos

### Módulo 3.1 · Web e Comunicação Cliente-Servidor
**Objetivo:** Entender como cliente e servidor conversam, HTTP, APIs.

- `02-Computer-Networking-Top-Down` — camada de aplicação (HTTP, DNS, sockets)
- `03-High-Performance-Browser-Networking` — TLS, latência, HTTP em profundidade

### Módulo 3.2 · Redes Básicas e Servidores
**Objetivo:** DNS, IP, portas, servidor de aplicação vs. servidor web.

- `02-Computer-Networking-Top-Down` — camadas de transporte e rede (TCP, IP, UDP)
- `01-How-Linux-Works` — processos, rede, como o SO gerencia serviços

### Módulo 3.3 · Ambientes e Configuração
**Objetivo:** Isolar local, homologação e produção; variáveis de ambiente.

- `01-How-Linux-Works` — shell, usuários, permissões, scripts de inicialização

### Módulo 3.4 · Dados e Armazenamento (Base)
**Objetivo:** Banco de dados, backup, restore, armazenamento de arquivos.

- `04-SQL-Performance-Explained` — índices, planos de query, fundamentos de performance

### Módulo 3.5 · Segurança e Operação Básica
**Objetivo:** Autenticação, deploy, rollback, logs, disponibilidade.

- `11-Practical-Monitoring` — introdução: o que são logs, métricas e como usá-los
- `12-Alice-and-Bob-Learn-Secure-Coding` — introdução: autenticação, senhas, vulnerabilidades básicas

---

## Fase Intermediária — Produção Real

### Módulo 4.1 · CI/CD e Automação
**Objetivo:** Git aplicado a deploy, pipelines, testes automáticos antes de subir.

- `08-Continuous-Delivery` — completo

### Módulo 4.2 · Containerização
**Objetivo:** Docker — build, run, compose, redes, volumes.

- `05-Docker-Deep-Dive` — completo

### Módulo 4.3 · Banco de Dados em Produção e Storage
**Objetivo:** Performance sob carga, migrations, connection pool, buckets e URLs assinadas.

- `04-SQL-Performance-Explained` — capítulos avançados (produção, índices compostos)
- `06-Designing-Data-Intensive-Applications` — storage, encoding, replicação básica

### Módulo 4.4 · Segurança, Acessos e Compliance
**Objetivo:** RBAC, multi-tenant, rate limit, CORS, gerenciamento de segredos, LGPD.

- `12-Alice-and-Bob-Learn-Secure-Coding` — RBAC, segurança de APIs, gerenciamento de segredos
- `09-Release-It` — circuit breakers, timeouts, bulkheads (resiliência que impede ataques de DoS acidental)

### Módulo 4.5 · Observabilidade e Resolução de Problemas
**Objetivo:** Logs estruturados, monitoramento de erros, alertas.

- `11-Practical-Monitoring` — parte intermediária/avançada: dashboards, alertas, on-call
- `10-Site-Reliability-Engineering` — SLIs, SLOs, error budgets, alertas baseados em sintomas

---

## Fase Avançada — Escala e Missão Crítica

### Módulo 5.1 · Escala e Alta Disponibilidade
**Objetivo:** Load balancer, filas, workers, cache, CDN, múltiplas instâncias.

- `06-Designing-Data-Intensive-Applications` — replicação, particionamento, consistência
- `09-Release-It` — estabilidade em produção: patterns de longa duração
- `10-Site-Reliability-Engineering` — incident management, toil, postmortems

### Módulo 5.2 · Dados Avançados e Resiliência
**Objetivo:** Replicação de banco, disaster recovery, multi-região.

- `06-Designing-Data-Intensive-Applications` — consenso distribuído, streams, tolerância a falhas catastróficas

### Módulo 5.3 · Cloud Profissional e IaC
**Objetivo:** IAM, VPC, infraestrutura como código, controle de custos.

- `07-Cloud-Native-Patterns` — completo

### Módulo 5.4 · Orquestração e Observabilidade Avançada
**Objetivo:** Kubernetes, tracing distribuído, métricas em sistemas complexos.

- `10-Site-Reliability-Engineering` — capítulos avançados: distributed systems, Kubernetes
- `07-Cloud-Native-Patterns` — orquestração e observabilidade cloud-native
- `03-High-Performance-Browser-Networking` — HTTP/2, QUIC, performance de borda

### Módulo 5.5 · Segurança Avançada e Compliance
**Objetivo:** WAF, pentest, hardening, auditoria, compliance para contratos Enterprise.

- `12-Alice-and-Bob-Learn-Secure-Coding` — parte avançada: pentest, hardening, auditoria de código

---

## Livros que você abre mais de uma vez

| Livro | Módulos |
|-------|---------|
| `02-Computer-Networking-Top-Down` | 3.1 → 3.2 |
| `01-How-Linux-Works` | 3.2 → 3.3 |
| `04-SQL-Performance-Explained` | 3.4 → 4.3 |
| `06-Designing-Data-Intensive-Applications` | 4.3 → 5.1 → 5.2 |
| `09-Release-It` | 4.4 → 5.1 |
| `10-Site-Reliability-Engineering` | 4.5 → 5.1 → 5.4 |
| `11-Practical-Monitoring` | 3.5 → 4.5 |
| `12-Alice-and-Bob-Learn-Secure-Coding` | 3.5 → 4.4 → 5.5 |
| `07-Cloud-Native-Patterns` | 5.3 → 5.4 |
| `03-High-Performance-Browser-Networking` | 3.1 → 5.4 |

---

## Ciclo de estudo por capítulo

```
1. PRÉ-LEITURA (5 min)
   └─ Leia título, subtítulos e conclusão do capítulo
   └─ Anote: "o que espero aprender aqui?"

2. LEITURA ATIVA
   └─ Leia o capítulo inteiro sem interrupção
   └─ Grife só o essencial: definições, mecanismos, decisões de design

3. NOTES BRUTAS (logo após terminar)
   └─ Feche o livro
   └─ Escreva de memória: o que ficou? quais conceitos? como funcionam?
   └─ Use suas próprias palavras — nunca copie trechos

4. NOTEBOOK LM — confronto
   └─ Abra o PDF no NotebookLM
   └─ Compare suas anotações com o texto original
   └─ Marque o que errou, esqueceu ou entendeu diferente
   └─ Use o chat para esclarecer pontos confusos

5. QUESTÕES (geração ativa)
   └─ Escreva 3–5 perguntas que um incidente real ou entrevista poderia levantar
   └─ Formato útil:
       - "O que acontece se X falhar antes de Y?"
       - "Por que usar A em vez de B nesse cenário?"
       - "Qual o tradeoff entre X e Z?"
       - "Como isso se aplica ao sistema de gestão de obras?"

6. REESTUDO GUIADO
   └─ Volte ao livro apenas nas seções onde houve lacuna
   └─ Foco cirúrgico — não releia o capítulo inteiro

7. QUESTÕES FINAIS
   └─ Responda suas próprias perguntas sem consultar nada
   └─ Anote as que ainda tiver dúvida → revisão espaçada
```

---

## Estrutura de anotações sugerida

```
d:\TECH\
├── notas\
│   ├── 3.1-web-cliente-servidor\
│   │   ├── cap-networking.md
│   │   ├── cap-browser-networking.md
│   │   └── questoes.md
│   ├── 3.2-redes-servidores\
│   ├── 3.3-ambientes\
│   ├── 3.4-dados-base\
│   ├── 3.5-segurança-basica\
│   ├── 4.1-cicd\
│   ├── 4.2-containers\
│   ├── 4.3-banco-producao\
│   ├── 4.4-segurança-compliance\
│   ├── 4.5-observabilidade\
│   ├── 5.1-escala-ha\
│   ├── 5.2-dados-avancados\
│   ├── 5.3-cloud-iac\
│   ├── 5.4-orquestração\
│   └── 5.5-segurança-avancada\
└── revisao\
    └── pendentes.md   ← perguntas não dominadas, com número do módulo
```

---

## O que evitar no começo (overengineering)

| Tecnologia | Por que esperar |
|------------|-----------------|
| Kubernetes | Exige equipe dedicada; Docker Compose resolve 99% dos casos iniciais |
| Microserviços | Cria pesadelo de infra antes de existir gargalo real — monólito bem feito escala longe |
| Multi-cloud | Adiciona meses de complexidade sem benefício real na fase de validação |
| Kafka / RabbitMQ complexo | Dificulta debug imensamente em equipes pequenas |
| IaC no primeiro deploy | Travar o primeiro server por sintaxe de Terraform atrasa a validação do produto |

---

## Sinais de que você dominou um módulo

- Consegue explicar o conceito sem abrir o livro
- Consegue dizer quando **não** usar aquela técnica
- Consegue conectar com algo do módulo anterior
- Consegue mapear o risco de negócio se esse módulo for ignorado
