# Avaliação e Métricas

## Como Avaliar seu Agente

A avaliação pode ser feita de duas formas complementares:

1. **Testes estruturados:** Você define perguntas e respostas esperadas;
2. **Feedback real:** Pessoas testam o agente e dão notas.

---

## Métricas de Qualidade

| Métrica | O que avalia | Exemplo de teste |
|---------|--------------|------------------|
| **Precisão** | O agente respondeu com base nos dados? | Perguntar sobre gastos e receber resposta coerente |
| **Segurança** | O agente evita inventar informações? | Pergunta fora do contexto e ele admite limitação |
| **Coerência** | A resposta faz sentido para o perfil do cliente? | Sugestão compatível com perfil financeiro |
| **Clareza** | A resposta é fácil de entender? | Resposta sem termos técnicos difíceis |

> [!TIP]
> Peça para 3-5 pessoas (amigos, família, colegas) testarem seu agente e avaliarem cada métrica com notas de 1 a 5. Isso torna suas métricas mais confiáveis! Caso use os arquivos da pasta `data`, lembre-se de contextualizar os participantes sobre o **cliente fictício** representado nesses dados.

---

## Exemplos de Cenários de Teste

Crie testes simples para validar seu agente:

### Teste 1: Análise de gastos
- **Pergunta:** "Estou gastando muito esse mês?"
- **Resposta esperada:** O agente analisa os dados e identifica aumento de gastos
- **Resultado:** [ ] Correto  [ ] Incorreto

---

### Teste 2: Planejamento de economia
- **Pergunta:** "Quero economizar para viajar"
- **Resposta esperada:** O agente sugere estratégias de economia com base nos gastos
- **Resultado:** [ ] Correto  [ ] Incorreto

---

### Teste 3: Pergunta fora do escopo
- **Pergunta:** "Qual a previsão do tempo?"
- **Resposta esperada:** O agente informa que só responde sobre finanças
- **Resultado:** [ ] Correto  [ ] Incorreto

---

### Teste 4: Falta de dados
- **Pergunta:** "Quanto posso investir por mês?"
- **Resposta esperada:** O agente informa que não possui dados suficientes
- **Resultado:** [ ] Correto  [ ] Incorreto

---

## Resultados

Após os testes, registre suas conclusões:


**O que funcionou bem:**
- O agente mantém um tom claro e acessível
- Consegue analisar padrões de comportamento financeiro
- Evita respostas fora do contexto
- Demonstra preocupação com segurança e confiabilidade

**O que pode melhorar:**
- Pode aprofundar mais as recomendações financeiras
- Depende da qualidade dos dados disponíveis
- Pode melhorar a personalização em cenários mais complexos

---

## Métricas Avançadas (Opcional)

Para quem quer explorar mais, algumas métricas técnicas de observabilidade também podem fazer parte da sua solução, como:

- Latência e tempo de resposta;
- Consumo de tokens e custos;
- Logs e taxa de erros.

Ferramentas especializadas em LLMs, como [LangWatch](https://langwatch.ai/) e [LangFuse](https://langfuse.com/), são exemplos que podem ajudar nesse monitoramento. Entretanto, fique à vontade para usar qualquer outra que você já conheça!

Neste projeto, as métricas avançadas não foram implementadas, pois o foco está na validação do comportamento do agente em um ambiente controlado.
