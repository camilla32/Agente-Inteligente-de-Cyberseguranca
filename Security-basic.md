# Base de Conhecimento — Fundamentos de Cibersegurança

## Objetivo

Este documento reúne os conceitos fundamentais utilizados pelo CyberGuard AI para analisar vulnerabilidades, avaliar riscos e recomendar medidas de proteção.

Sempre que possível, o agente deve utilizar estes conceitos como base para explicar suas conclusões de forma clara e consistente.

---

# 1. Conceitos Fundamentais

## Ativo

Um **ativo** é qualquer recurso que possua valor para uma pessoa ou organização.

Exemplos:

- Aplicações
- Servidores
- Bancos de dados
- APIs
- Computadores
- Dispositivos móveis
- Credenciais
- Informações pessoais
- Documentos internos

A importância do ativo influencia diretamente a avaliação do risco.

---

## Ameaça

Uma **ameaça** é qualquer evento, agente ou circunstância capaz de causar danos a um ativo.

Exemplos:

- Phishing
- Malware
- Ransomware
- Engenharia social
- Acesso não autorizado
- Erro humano
- Configuração incorreta
- Ataques internos

Uma ameaça representa uma possibilidade de ocorrência, não necessariamente um incidente confirmado.

---

## Vulnerabilidade

Uma **vulnerabilidade** é uma fraqueza existente em um sistema, processo ou configuração que pode ser explorada ou contribuir para um incidente de segurança.

Exemplos:

- Software desatualizado
- Senhas fracas
- Permissões excessivas
- Armazenamento público indevido
- Falta de autenticação multifator
- Entradas sem validação
- Serviços expostos desnecessariamente

Nem toda vulnerabilidade significa que um ataque já ocorreu.

---

## Risco

**Risco** é a possibilidade de uma ameaça explorar uma vulnerabilidade e causar impacto sobre um ativo.

A avaliação deve considerar:

- Probabilidade
- Impacto
- Exposição
- Controles existentes
- Contexto do ambiente

---

# 2. Tríade CIA

A Tríade CIA representa os três pilares da segurança da informação.

## Confidencialidade

Garante que apenas pessoas autorizadas tenham acesso às informações.

### Possíveis riscos

- Vazamento de dados
- Acesso indevido
- Roubo de informações

### Controles comuns

- Criptografia
- Controle de acesso
- Autenticação multifator
- Classificação de informações

---

## Integridade

Garante que os dados permaneçam corretos e não sejam alterados indevidamente.

### Possíveis riscos

- Alteração não autorizada
- Corrupção de dados
- Fraudes

### Controles comuns

- Logs
- Controle de alterações
- Assinaturas digitais
- Hashes

---

## Disponibilidade

Garante que sistemas e informações estejam acessíveis quando necessários.

### Possíveis riscos

- Interrupções
- Ataques de negação de serviço
- Falhas de infraestrutura

### Controles comuns

- Backups
- Redundância
- Monitoramento
- Plano de recuperação

---

# 3. Probabilidade

A probabilidade representa uma estimativa da chance de exploração de uma vulnerabilidade.

O CyberGuard AI utiliza três níveis qualitativos.

| Nível | Significado |
|--------|------------|
| Baixa | Poucas condições favorecem a exploração. |
| Média | Existem condições relevantes para exploração. |
| Alta | A exploração parece significativamente favorecida pelo contexto. |

A classificação deve sempre ser acompanhada de justificativa.

---

# 4. Impacto

O impacto representa as possíveis consequências caso a vulnerabilidade seja explorada.

Também utiliza três níveis qualitativos.

| Nível | Significado |
|--------|------------|
| Baixo | Consequências limitadas. |
| Médio | Consequências relevantes. |
| Alto | Consequências graves para o ativo ou organização. |

O impacto pode afetar:

- Confidencialidade
- Integridade
- Disponibilidade
- Operações
- Reputação
- Aspectos legais

---

# 5. Matriz Qualitativa de Risco

O CyberGuard AI utiliza a seguinte matriz para estimar a severidade do risco.

| Probabilidade | Impacto Baixo | Impacto Médio | Impacto Alto |
|---------------|---------------|---------------|--------------|
| Baixa | Baixo | Baixo | Médio |
| Média | Baixo | Médio | Alto |
| Alta | Médio | Alto | Crítico |

Esta matriz é uma convenção educacional utilizada pelo projeto.

Ela não substitui metodologias formais como o CVSS.

---

# 6. Grau de Confiança

Além da severidade, o agente deve indicar o nível de confiança da análise.

| Nível | Significado |
|--------|------------|
| Alto | Informações suficientes sustentam a análise. |
| Médio | Existem algumas incertezas. |
| Baixo | Faltam informações importantes. |

O grau de confiança representa a qualidade das evidências disponíveis.

---

# 7. Boas Práticas de Segurança

O CyberGuard AI deve priorizar recomendações alinhadas às seguintes boas práticas.

## Gestão de acesso

- Menor privilégio
- Revisão periódica de permissões
- MFA para contas críticas

## Gestão de vulnerabilidades

- Atualizar sistemas regularmente
- Corrigir falhas priorizadas
- Inventariar ativos

## Proteção de dados

- Criptografia
- Backup
- Classificação de informações

## Monitoramento

- Logs
- Alertas
- Auditoria

## Segurança de aplicações

- Validação de entradas
- Tratamento seguro de erros
- Controle de autenticação
- Atualização de dependências

## Cultura de segurança

- Treinamento contra phishing
- Conscientização dos usuários
- Procedimentos documentados

---

# 8. Processo de Tratamento de Vulnerabilidades

O agente deve seguir uma lógica semelhante ao ciclo abaixo.

1. Identificar o problema.
2. Entender o contexto.
3. Avaliar probabilidade.
4. Avaliar impacto.
5. Estimar a severidade.
6. Priorizar ações.
7. Aplicar correções.
8. Validar a correção.
9. Acompanhar o risco residual.

---

# 9. Referências Técnicas

O CyberGuard AI utiliza como inspiração conceitos amplamente reconhecidos na área de cibersegurança.

- NIST Cybersecurity Framework
- NIST National Vulnerability Database
- OWASP Top 10
- FIRST CVSS

O agente deve utilizar esses conceitos como referência educacional, sem afirmar que consultou essas fontes em tempo real.

---

# 10. Diretriz Final

Toda análise deve ser baseada em contexto, evidências disponíveis e transparência sobre incertezas.

Quando não houver informações suficientes para uma classificação confiável, o CyberGuard AI deve reconhecer essa limitação e solicitar os dados necessários antes de chegar a uma conclusão.