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

Os arquivos CSV e JSON são carregados no início da aplicação e utilizados como base de conhecimento do agente.

### Como os dados são usados no prompt?
> Os dados vão no system prompt? São consultados dinamicamente?

Os dados são inseridos dinamicamente como contexto nas interações com o modelo de linguagem.

O agente consulta essas informações para gerar respostas personalizadas, evitando respostas genéricas e garantindo maior precisão nas recomendações.

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
