# **1. Informações gerais**
## **1.1 Responsável:** 
[Deborah Carminatti](https://viaaroma.my3cx.com.br:5001/deborah) - Analista de Dados Senior

[Bruna Barbosa](https://viaaroma.my3cx.com.br:5001/bruna) - Analista de Dados Jr.

## **1.2 Objetivo**: 
Esta tabela é a junção das tabelas ordens_producoes, produtos e ordens_producoes_itens, essa query é apenas sobre ordens de produção dos aromatizadores (departamento_id = '4'),
referente ao ano 2023, lista todas as OPS exceto as canceladas

## **1.3 Estrutura da Tabela:**
|campo|formato|descricao|exemplo|
|--|--|---|---|
|id|varchar|identifica o ID da tabela ordens de produção|8448|00271ea0-0a9e-4c4f-8748-4f26528ba5ef|
|data_programada|datetime|data para o dia que a OP foi programada, usada para calcular a aderência|2023-10-26 07:00:00|
|situacao_atual|varchar|referente ao status atual da OP|FINALIZADA|
|situacao_planejamento|varchar|referente ao status do planejamento da OP|FIRMADA|
|id_produto|varchar|identifica o produto final na tabela ordens de producao|2494|
|quantidade_programada|decimal|referente a quantidade a ser produzida quando programada a OP|500.0000|
|rendimento_real|decimal|referente a quantidade que foi produzida quando a OP foi finalizada|499.0000|
|data_inicio_producao|datetime|referente a data em que a produção foi inciada(nos relatorios de producao mensal do sistema são gerados em cima dessa data|2023-10-27 14:42:05|

# **2. SQL**

Query: [fat_ordens_producao.sql]
([https://github.com/carminattideh/datasciencia_viaaroma/blob/viaaroma/fat_soc.sql](https://github.com/carminattideh/datasciencia_viaaroma/blob/viaaroma/fat_ordens_producao.sql))

## **2.1 Regras de SQL**:
2.1.1. 

2.1.2.

2.1.3. 


## **2.2 Regras de atualização:**

A tabela deverá ser atualizada diariamente as 8 (oito) horas da manhã. 

## **2.3 Validações:**

Descrever quais são alguns dos resultados esperados e como pode ser efetuada a validação dos dados na tabela. Ex.:

- A coluna id. da tabela produtos se relaciona com a coluna produto_id da tabela ordens_producoes
- A coluna producao_id da tabela itens se relaciona com a tabela id, da tabela ordens_producoes
- Na tabela ordens_producoes, o campo que esta apenas "data", refere-se a data programada
- Na tabela produtos, o campo departamento_id = '4', refere-se aos aromatizadores
# **3. Fluxos de Dados:** 

## **3.1 Workspace:** 

### 10. Fluxos:

[10. Fluxos](https://app.powerbi.com/groups/3d2030df-c6d5-4176-9b6b-9bc317127a17/list):

## **3.1 Power Automate:** 

Links com os Fluxos do PowerAutomate que são disparados a partir da atualização desta tabela

## **3.2 Estudos:**

Links para os estudos relacionados à esta tabela.


# **4. Data Warehouse**

## **4.1 Create Table**

```SQL    
-- Código do create table
```
## **4.2 Create Index**

```SQL
-- Código de criação dos índices
```


## **4.3 Permissões:** 
|Grupo|Tipo|
|--|--|
|Colaboradores do time Data Science|Leitura|
|Engenharia de Dados|Leitura/Escrita|
|DBA|Leitura/Escrita|

## **4.4 Índice(s):** n/a

## **4.5 Relacionamento(s):** 

```

```

## **4.6 Servidor do ETL:**
Nome do servidor

## **4.7 Nome do ETL:** 
NOME DO ETL

## **4.7.1 Pacote do ETL:** 
Link para o GIT do Dbops

## **4.8 Nome do Job:** 
NOME DO JOB

## **4.9 Periodicidade da Rotina:** 
Agenda de execuções

## **4.10 Notificações de Atualização:**

Quando concluída com sucesso, a atualização envia um e-mail com assunto **_Êxito: NOME_DA_TABELA_**.

> O contato equipedatascience@viacertabanking.com.br recebe um e-mail na caixa de entrada. 

> O contato 5223126f.viacertafinanciadora.com.br@amer.teams.ms faz uma postagem no canal [DW e Power BI](https://teams.microsoft.com/_?lm=deeplink&lmsrc=homePageWeb&cmpid=WebSignIn#/conversations/DW%20e%20Power%20BI?threadId=19:3fbf0af999d4437189f625a478e75c13@thread.skype&ctx=channel)

```
De: Não Responder - VIACERTA <noreply@viacertabanking.com.br>
Para: equipedatascience@viacertabanking.com.br e 5223126f.viacertafinanciadora.com.br@amer.teams.ms

Assunto: Êxito: NOME_DA_TABELA
Corpo:
Olá.
A carga **NOME_DA_TABELA** foi realizada com sucesso!
Não responder este e-mail.
```


## **4.11 Regras de ETL após a carga**

Descrever ações que devem ocorrer após a carga, se necessário

# **5. Análise de Impacto**

## **5.1 Indicadores:**
- Lista de Indicadores que acessam informações desta tabela
- Paineis que usam informações desta tabela
- Outros locais que se baseiam nesta tabela


# **6. Tarefas Relacionadas**

Inserir links com as tarefas relacionadas à esta tabela (criação, atualizações, correções)
