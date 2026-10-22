# Skill: Vulnerability Analysis

## 1. Visão geral

A habilidade **Vulnerability Analysis** faz parte do projeto CyberGuard AI e define um procedimento estruturado para analisar vulnerabilidades de segurança da informação.

Seu objetivo é ajudar o agente a interpretar cenários, avaliar riscos, justificar classificações e recomendar ações corretivas priorizadas.

Esta habilidade foi desenvolvida para fins educacionais, com foco em prevenção, análise defensiva e uso responsável de inteligência artificial.

## 2. Objetivos

A habilidade permite orientar o agente para:

- Identificar e descrever vulnerabilidades.
- Analisar o contexto do ativo afetado.
- Avaliar a probabilidade de exploração.
- Estimar impactos potenciais.
- Classificar a severidade do risco.
- Recomendar medidas de mitigação e correção.
- Explicar as razões da avaliação.
- Registrar limitações e incertezas.

## 3. Arquivos relacionados

Esta habilidade é composta pelos seguintes arquivos:

| Arquivo | Finalidade |
|---|---|
| `SKILL.md` | Define as instruções operacionais, os critérios de análise e o formato de saída. |
| `README.md` | Documenta a habilidade, sua finalidade e as formas de utilização. |

A habilidade também utiliza como referência conceitual os arquivos gerais do agente:

- `agent/persona.md`: define a identidade e o comportamento esperado do CyberGuard AI.
- `agent/knowledge/security-basics.md`: apresenta conceitos fundamentais de cibersegurança.
- `AGENTS.md`: contém as orientações gerais para o desenvolvimento do projeto.

## 4. Fluxo de funcionamento

O processo de análise segue estas etapas:

1. Receber a descrição de uma vulnerabilidade.
2. Identificar o contexto e o ativo afetado.
3. Avaliar as evidências disponíveis.
4. Estimar probabilidade e impacto.
5. Classificar a severidade ou indicar que ela é indeterminada.
6. Elaborar um plano de correção priorizado.
7. Explicar a classificação e suas limitações.
8. Recomendar a validação das medidas aplicadas.

## 5. Critérios de avaliação

A análise considera os seguintes fatores:

### Probabilidade

Avalia as condições que podem favorecer a exploração da vulnerabilidade.

### Impacto

Considera possíveis consequências para a confidencialidade, integridade, disponibilidade e continuidade das operações.

### Severidade

Combina qualitativamente probabilidade e impacto, considerando também o contexto e os controles existentes.

### Grau de confiança

Indica a qualidade das informações disponíveis para sustentar a análise. Não representa a gravidade do risco.

## 6. Exemplo de entrada

```text
Ativo: Aplicação administrativa.

Problema relatado: Biblioteca desatualizada com possíveis
correções de segurança disponíveis.

Exposição: Ainda não identificada.

Controles existentes: Não informados.

Objetivo: Avaliar o risco e recomendar próximos passos.
```

## 7. Resultado esperado

Para o cenário apresentado, o agente deve:

- Explicar por que uma dependência desatualizada pode representar um risco.
- Solicitar a identificação da biblioteca e da versão utilizada.
- Verificar quais informações são necessárias para confirmar a vulnerabilidade.
- Evitar uma classificação definitiva sem evidências suficientes.
- Recomendar a análise da versão afetada e o planejamento de uma atualização segura.
- Sugerir testes autorizados para validar a correção.

O resultado deve distinguir fatos conhecidos de hipóteses.

## 8. Como utilizar no projeto

O arquivo `SKILL.md` funciona como especificação da habilidade para orientar o desenvolvimento do agente.

Na versão inicial do CyberGuard AI, esses documentos são instruções e referências para implementação. **A presença dos arquivos Markdown, isoladamente, não executa uma análise automática nem integra um modelo de inteligência artificial.**

Para tornar a habilidade funcional, será necessário implementar uma aplicação que interprete os dados de entrada e aplique os critérios definidos ou integrar um modelo de IA por meio de um backend seguro.

## 9. Testes recomendados

Durante o desenvolvimento, utilize cenários fictícios para verificar se o agente:

- Diferencia vulnerabilidades de ameaças.
- Explica a probabilidade e o impacto.
- Evita inventar evidências.
- Reconhece quando faltam informações.
- Apresenta recomendações proporcionais ao risco.
- Separa severidade de grau de confiança.
- Recomenda validação após a correção.
- Mantém o foco em atividades defensivas autorizadas.

## 10. Limitações

As classificações produzidas dependem da qualidade das informações fornecidas e das regras efetivamente implementadas.

A matriz qualitativa do projeto tem finalidade educacional e não substitui métodos formais de avaliação, ferramentas especializadas ou análise profissional.

O agente não deve afirmar que realizou varreduras, consultou bases em tempo real ou confirmou uma correção sem que essas ações tenham sido realmente executadas.

## 11. Evolução futura

Possíveis melhorias incluem:

- Interface web para submissão de vulnerabilidades.
- Matriz visual de probabilidade e impacto.
- Relatórios exportáveis.
- Histórico de análises.
- Consulta a fontes públicas de vulnerabilidades.
- Integração segura com um modelo de IA.
- Testes automatizados de consistência das classificações.

## 12. Segurança e responsabilidade

Utilize o CyberGuard AI para aprendizado, prevenção e análise defensiva em ambientes autorizados.

Não inclua credenciais, senhas, tokens ou outras informações confidenciais nos exemplos, testes ou repositórios públicos.

---

**Projeto:** CyberGuard AI  
**Habilidade:** Vulnerability Analysis  
**Finalidade:** Análise e priorização defensiva de vulnerabilidades.