# Base de Conhecimento

## Dados Utilizados

Descreva se usou os arquivos da pasta `data`, por exemplo:

| Arquivo | Formato | Utilização no Agente |
|---------|---------|---------------------|
| `historico_atendimento.csv` | CSV | Contextualizar interações anteriores e melhorar personalização |
| `perfil_investidor.json` | JSON | Definir perfil financeiro do cliente (conservador, moderado, agressivo) |
| `produtos_financeiros.json` | JSON | Sugerir produtos e soluções financeiras adequadas |
| `transacoes.csv` | CSV | Analisar padrão de gastos e comportamento financeiro |

> [!TIP]
> **Quer um dataset mais robusto?** Você pode utilizar datasets públicos do [Hugging Face](https://huggingface.co/datasets) relacionados a finanças, desde que sejam adequados ao contexto do desafio.

---

## Adaptações nos Dados

Os dados mockados foram mantidos, mas interpretados de forma a simular cenários reais de uso.

Podem ser ajustados para representar diferentes perfis de clientes, níveis de renda e padrões de consumo, permitindo testar o comportamento do agente em situações variadas.

---

## Estratégia de Integração

### Como os dados são carregados?
> Descreva como seu agente acessa a base de conhecimento.

[ex: Os JSON/CSV são carregados no início da sessão e incluídos no contexto do prompt]

### Como os dados são usados no prompt?
> Os dados vão no system prompt? São consultados dinamicamente?

Os arquivos CSV e JSON são carregados no início da aplicação e utilizados como base de conhecimento do agente.

Esses dados são processados e organizados para facilitar a análise do comportamento financeiro do cliente.

---

## Exemplo de Contexto Montado

> Mostre um exemplo de como os dados são formatados para o agente.

```
Dados do Cliente:
- Nome: João Silva
- Perfil: Moderado
- Saldo disponível: R$ 5.000

Últimas transações:
- 01/11: Supermercado - R$ 450
- 03/11: Streaming - R$ 55
...
```
