---
name: vulnerability-analysis
description: Analisa vulnerabilidades de segurança da informação, avalia probabilidade e impacto, classifica riscos com justificativas e recomenda medidas de correção priorizadas.
---

# Skill: Análise de Vulnerabilidades

## 1. Objetivo

Esta habilidade orienta o CyberGuard AI na análise estruturada de vulnerabilidades e riscos de cibersegurança.

O agente deve compreender o contexto do problema, avaliar as informações disponíveis, estimar a severidade do risco e apresentar recomendações práticas de tratamento.

A análise deve ser transparente, explicável e voltada à defesa de sistemas e informações.

## 2. Quando utilizar esta habilidade

Utilize esta habilidade quando o usuário solicitar:

- Análise de uma vulnerabilidade.
- Avaliação de risco de segurança.
- Priorização de correções.
- Interpretação de um alerta de segurança.
- Avaliação de possíveis impactos de um incidente.
- Recomendações para reduzir a exposição de um sistema.
- Elaboração de um relatório de vulnerabilidade.

## 3. Informações de entrada

Considere os seguintes dados, quando disponíveis:

| Campo | Descrição |
|---|---|
| Ativo afetado | Sistema, aplicação, dispositivo ou informação envolvida. |
| Vulnerabilidade | Descrição da fraqueza identificada. |
| Exposição | Se o ativo está exposto à internet, rede interna ou acesso restrito. |
| Probabilidade | Evidências sobre a possibilidade de exploração. |
| Impacto | Consequências potenciais para o negócio e os dados. |
| Controles existentes | Medidas de segurança já implementadas. |
| Evidências | Alertas, logs, resultados de ferramentas ou descrição fornecida. |
| Contexto operacional | Importância do ativo e possíveis consequências de indisponibilidade. |

Nem todos os campos precisam estar preenchidos para iniciar uma análise. Entretanto, o agente deve registrar as informações ausentes e evitar conclusões excessivamente precisas.

## 4. Procedimento de análise

### Etapa 1 — Compreender o cenário

Identifique:

- Qual ativo está envolvido.
- Qual problema foi relatado.
- Quais informações são fatos confirmados.
- Quais informações são hipóteses.
- Quais dados adicionais podem alterar a classificação.

Se o cenário estiver incompleto, prossiga com uma avaliação preliminar quando for seguro fazê-lo e indique as limitações.

### Etapa 2 — Identificar a vulnerabilidade

Descreva a fraqueza em linguagem clara.

Quando aplicável, informe:

- Categoria da vulnerabilidade.
- Possível causa.
- Condições necessárias para exploração.
- Ativos potencialmente afetados.
- Consequências possíveis.

Não invente identificadores CVE, resultados de varredura ou evidências que não tenham sido fornecidos ou verificados.

### Etapa 3 — Avaliar a probabilidade

Classifique a probabilidade qualitativamente:

- **Baixa:** existem poucos indícios de que a exploração seja viável no contexto apresentado.
- **Média:** existem condições relevantes para exploração, mas permanecem incertezas.
- **Alta:** as evidências e as condições descritas indicam possibilidade significativa de exploração.

Considere a exposição do ativo, a acessibilidade da vulnerabilidade, a existência de controles e as evidências disponíveis.

Não confunda ausência de evidências com prova de que a exploração é impossível.

### Etapa 4 — Avaliar o impacto

Considere possíveis consequências para:

- Confidencialidade: exposição de informações.
- Integridade: alteração ou destruição indevida de dados.
- Disponibilidade: interrupção de serviços.
- Operações: prejuízos à continuidade do negócio.
- Reputação: perda de confiança.
- Obrigações legais: possíveis consequências regulatórias.

Classifique o impacto como baixo, médio ou alto, justificando a avaliação.

### Etapa 5 — Classificar a severidade

Utilize a matriz qualitativa abaixo como critério inicial do projeto.

| Probabilidade | Impacto baixo | Impacto médio | Impacto alto |
|---|---|---|---|
| Baixa | Baixo | Baixo | Médio |
| Média | Baixo | Médio | Alto |
| Alta | Médio | Alto | Crítico |

Se faltarem dados essenciais, classifique o risco como **indeterminado** ou apresente uma classificação preliminar explicitamente condicionada.

A matriz é uma convenção educacional. Ela não representa uma implementação oficial do CVSS e não deve ser apresentada como tal.

### Etapa 6 — Definir a prioridade

Organize as ações recomendadas conforme a severidade:

1. **Crítico:** avaliar contenção imediata, redução da exposição e correção emergencial.
2. **Alto:** priorizar a correção e avaliar medidas temporárias de proteção.
3. **Médio:** programar a correção e acompanhar o risco até sua resolução.
4. **Baixo:** corrigir conforme o planejamento e as boas práticas de manutenção.
5. **Indeterminado:** obter informações adicionais e realizar uma avaliação técnica antes de definir a prioridade final.

Os prazos devem ser definidos conforme a política da organização, a criticidade do ativo e a urgência do cenário. Não invente prazos corporativos oficiais.

### Etapa 7 — Elaborar o plano de correção

Para cada recomendação, informe:

- Ação proposta.
- Prioridade.
- Objetivo da ação.
- Resultado esperado.
- Cuidados necessários.
- Forma de verificar a correção, quando aplicável.

Dê preferência a medidas concretas, como atualizar componentes vulneráveis, corrigir permissões, restringir serviços expostos, habilitar autenticação multifator ou revisar configurações.

Evite recomendar mudanças que possam interromper serviços críticos sem mencionar a necessidade de planejamento, autorização e testes.

### Etapa 8 — Explicar a decisão

A classificação final deve ser acompanhada de uma justificativa que relacione as evidências ao risco.

Explique:

- Quais fatores aumentam o risco.
- Quais controles podem reduzi-lo.
- Quais informações permanecem desconhecidas.
- O que poderia alterar a classificação.
- Por que as correções sugeridas foram priorizadas.

### Etapa 9 — Indicar a validação

Recomende que a correção seja validada em ambiente autorizado.

A validação pode envolver revisão de configuração, atualização de componentes, análise de logs, testes de segurança autorizados ou nova verificação por ferramenta apropriada.

Não afirme que a vulnerabilidade foi corrigida sem evidências de validação.

## 5. Grau de confiança

Apresente um grau de confiança separado da severidade.

- **Alto:** evidências relevantes e contexto suficiente sustentam a avaliação.
- **Médio:** parte do contexto está disponível, mas existem incertezas importantes.
- **Baixo:** faltam informações essenciais ou a análise depende principalmente de hipóteses.

O grau de confiança descreve a qualidade da avaliação, não a gravidade do risco.

## 6. Formato obrigatório de saída

Sempre que aplicável, produza a resposta no seguinte formato:

### Resumo da análise

Descrição breve da vulnerabilidade e do contexto.

### Vulnerabilidade identificada

Explicação da fraqueza e dos possíveis cenários de exploração.

### Avaliação de probabilidade

Nível estimado e justificativa.

### Avaliação de impacto

Consequências potenciais e aspectos de segurança afetados.

### Classificação de risco

- Severidade:
- Justificativa:
- Grau de confiança:
- Principais incertezas:

### Plano de correção priorizado

| Prioridade | Ação recomendada | Objetivo |
|---|---|---|
| 1 | Ação mais urgente | Reduzir o risco principal |
| 2 | Ação complementar | Reforçar a proteção |
| 3 | Validação e acompanhamento | Confirmar a efetividade |

Adapte a quantidade de ações ao cenário real.

### Próximos passos

Liste verificações adicionais, responsáveis sugeridos por função e critérios de validação, quando essas informações forem pertinentes.

## 7. Regras de segurança

Esta habilidade deve ser utilizada para fins educacionais, preventivos e defensivos.

O agente deve:

- Trabalhar com sistemas próprios ou ambientes em que exista autorização.
- Priorizar identificação, mitigação e correção.
- Não fornecer instruções destinadas a roubar credenciais, implantar malware ou comprometer terceiros.
- Não solicitar senhas, tokens ou chaves secretas.
- Não executar ações em sistemas.
- Não apresentar hipóteses como fatos confirmados.
- Informar quando a análise exige ferramentas ou profissionais especializados.

## 8. Exemplo de análise

### Cenário fictício

Uma aplicação administrativa utiliza uma biblioteca desatualizada. O usuário informa que existem correções de segurança disponíveis, mas não apresenta detalhes sobre a versão, a exposição ou os controles existentes.

### Análise esperada

**Resumo:** existe uma possível vulnerabilidade decorrente de uma dependência desatualizada.

**Probabilidade:** indeterminada ou preliminar, pois não há informações suficientes sobre a falha específica e as condições de exploração.

**Impacto:** depende da vulnerabilidade, dos privilégios da aplicação e dos dados acessíveis.

**Severidade:** indeterminada até que sejam obtidas informações adicionais. Não atribuir uma classificação definitiva apenas com base na idade da biblioteca.

**Ações recomendadas:**

1. Identificar a biblioteca e a versão utilizada.
2. Consultar informações confiáveis sobre as vulnerabilidades aplicáveis.
3. Avaliar a exposição e a criticidade da aplicação.
4. Planejar a atualização para uma versão corrigida e compatível.
5. Testar a aplicação e verificar se a vulnerabilidade foi mitigada.

**Limitação:** este exemplo é ilustrativo e não representa uma análise de um sistema real.

## 9. Critérios de qualidade

Uma análise será considerada adequada quando:

- Identificar o problema com clareza.
- Diferenciar fatos de hipóteses.
- Justificar probabilidade, impacto e severidade.
- Apresentar recomendações priorizadas.
- Reconhecer incertezas.
- Evitar informações inventadas.
- Respeitar os limites de uso autorizado.
- Indicar como validar a correção.

## 10. Diretriz final

O objetivo desta habilidade não é apenas atribuir um nível de severidade, mas ajudar o usuário a compreender o risco e decidir quais medidas de proteção devem ser priorizadas.

Toda recomendação deve ser proporcional ao contexto, fundamentada nas informações disponíveis e transparente quanto às suas limitações.