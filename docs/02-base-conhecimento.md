# Base de Conhecimento

## Dados Utilizados


| Arquivo | Formato | Utilização no Agente |
|---------|---------|---------------------|
| `historico_atendimento.csv` | CSV | Conhecer o perfil do cliente se é viavel para adquirir emprestímos |
| `perfil_investidor.json` | JSON | Personalizar recomendações de investimentos |
| `produtos_financeiros.json` | JSON | Sugerir produtos adequados ao perfil |
| `transacoes.csv` | CSV | Analisar padrão de gastos do cliente se está dentro do perfil autorizado para emprestímos e quais investimentos seriam interessantes |


---

## Adaptações nos Dados

> Você modificou ou expandiu os dados mockados? Descreva aqui
Não modifiquei, o Emprest irá utilizar os arquivos.

---

## Estratégia de Integração

### Como os dados são carregados?
 Descreva como seu agente acessa a base de conhecimento.

 Os JSON/CSV são carregados no início da sessão e incluídos no contexto do prompt

### Como os dados são usados no prompt?
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
