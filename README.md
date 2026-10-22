# 🛡️ CyberGuard AI — Agente Inteligente de Cibersegurança

## 📌 Sobre o projeto

O **CyberGuard AI** é um projeto de agente inteligente de cibersegurança desenvolvido para auxiliar na identificação, análise e priorização de vulnerabilidades.

Em vez de apenas apresentar informações sobre uma ameaça, o agente busca compreender o contexto, avaliar a probabilidade de exploração, estimar os impactos e recomendar medidas de correção priorizadas.

O projeto tem como objetivo demonstrar como a inteligência artificial pode apoiar a análise de riscos e a tomada de decisões em segurança da informação.

## 🎯 Objetivo

Desenvolver um agente de cibersegurança capaz de:

- Analisar vulnerabilidades e cenários de segurança.
- Avaliar probabilidade de exploração e impacto potencial.
- Classificar riscos por nível de severidade.
- Priorizar ações corretivas.
- Explicar os critérios utilizados na análise.
- Apresentar recomendações práticas de segurança.
- Organizar os resultados em relatórios compreensíveis.

## 💡 Problema que o projeto busca resolver

A identificação de uma vulnerabilidade não é suficiente para determinar qual problema deve ser tratado primeiro.

É necessário considerar o contexto do ativo, a exposição do sistema, a probabilidade de exploração, os possíveis impactos e os controles de segurança existentes.

O CyberGuard AI foi idealizado para organizar essas informações e ajudar o usuário a compreender quais riscos merecem maior atenção e quais ações podem reduzir a exposição.

## ⚙️ Como o agente funciona

O processo de análise está organizado nas seguintes etapas:

1. **Entrada de informações:** o usuário descreve uma vulnerabilidade ou um cenário de segurança.
2. **Análise do contexto:** o agente identifica o sistema afetado e as informações disponíveis.
3. **Avaliação de risco:** considera probabilidade de exploração e impacto potencial.
4. **Classificação:** atribui uma categoria de risco — crítico, alto, médio, baixo ou indeterminado.
5. **Plano de correção:** recomenda medidas de tratamento em ordem de prioridade.
6. **Explicabilidade:** apresenta as justificativas, limitações e informações que precisam ser verificadas.

## 📊 Classificação de risco

| Nível | Descrição |
|---|---|
| Crítico | Risco muito elevado que pode exigir ação imediata. |
| Alto | Risco significativo que exige correção prioritária. |
| Médio | Risco relevante que deve ser tratado de forma planejada. |
| Baixo | Risco limitado que deve ser acompanhado e corrigido conforme a prioridade. |
| Indeterminado | Informações insuficientes para uma avaliação confiável. |

A classificação é orientativa e deve considerar o contexto real do ambiente. Ela não substitui uma avaliação técnica especializada.

## 🧠 Diferenciais do projeto

- **Análise contextual:** considera mais do que o nome da vulnerabilidade.
- **Priorização de riscos:** ajuda a organizar as ações de correção.
- **Explicabilidade:** apresenta os motivos da classificação.
- **Recomendações práticas:** sugere medidas preventivas e corretivas.
- **Transparência:** reconhece incertezas e informações ausentes.
- **Uso responsável:** prioriza a proteção de sistemas e ambientes autorizados.

## 🗂️ Estrutura do projeto

```text
CyberGuard-AI/
├── AGENTS.md
├── README.md
├── agent/
│   ├── persona.md
│   └── security-basics.md
└── vulnerability-analysis/
        ├── SKILL.md
        └── README.md
```

## 🛠️ Tecnologias e recursos previstos

- **Markdown:** documentação, instruções e conhecimento do agente.
- **Visual Studio Code:** ambiente de desenvolvimento.
- **HTML, CSS e JavaScript:** tecnologias previstas para a interface web.
- **Inteligência artificial:** integração futura para interpretar cenários e elaborar recomendações, caso seja configurado um modelo compatível.

> **Observação:** a estrutura inicial contém arquivos de documentação e instruções. A interface web e a integração funcional com um modelo de IA serão desenvolvidas nas próximas etapas.

## 🔐 Segurança e uso responsável

O CyberGuard AI tem finalidade educacional e defensiva.

O projeto prioriza a identificação de riscos, a prevenção de incidentes e a recomendação de correções em ambientes autorizados. Não deve ser utilizado para acessar sistemas sem permissão, obter credenciais ou executar ações maliciosas.

Dados confidenciais, senhas e chaves de API não devem ser incluídos nos exemplos ou na documentação pública.

## 🚀 Próximas etapas

- [ ] Definir a persona do agente.
- [ ] Construir a base de conhecimento em cibersegurança.
- [ ] Desenvolver a habilidade de análise de vulnerabilidades.
- [ ] Criar a interface web em HTML, CSS e JavaScript.
- [ ] Implementar a avaliação de probabilidade, impacto e severidade.
- [ ] Exibir recomendações de correção priorizadas.
- [ ] Testar o agente com cenários fictícios.
- [ ] Documentar os resultados e publicar o projeto.

## 🎓 Contexto educacional

Projeto desenvolvido como proposta de aplicação prática dos conhecimentos do bootcamp Santander de Cibersegurança, com foco na utilização de inteligência artificial para análise e priorização de riscos.

## 👩‍💻 Autoria

Projeto educacional **CyberGuard AI**.

---

*CyberGuard AI — compreender o risco, priorizar a correção e fortalecer a segurança.*
