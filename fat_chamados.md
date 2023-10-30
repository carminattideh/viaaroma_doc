# **1. Informações gerais**
## **1.1 Responsável:** 
[Deborah Carminatti](https://viaaroma.my3cx.com.br:5001/deborah) - Analista de Dados Senior

[Bruna Barbosa](https://viaaroma.my3cx.com.br:5001/bruna) - Analista de Dados Jr.

## **1.2 Objetivo**: 
Esta tabela é a junção das tabelas chamados e chamados_grupos, referente aos chamados dos grupos SISTEMA SIG e BI - SISTEMA, a partir de 01/01/2021 onde o status é diferente de 'CANCELADA'.

## **1.3 Estrutura da Tabela:**
|campo|formato|descricao|exemplo|
|--|--|---|---|
|numero_chamado|int|referente ao número do chamado no sistema|8448|
|data_hora_inclusao|datetime|data e hora de inclusão do chamado no sistema|2023-09-11 08:52:27|
|descricao|varchar|referente ao grupo responsável pelo chamado|SISTEMA SIG|
|usuario_autor|varchar|referente ao usuário que abriu o chamado no sistema|sampaio|
|titulo|varchar|referente ao título do chamado|Cont Rec - Layout de integração Mercadolivre|
|descricao|text|descreve o motivo do chamado ter sido aberto, o problema ou solução|Subchamado do 5541 Segue arquivo em anexo|
|situacao|varchar|referente ao status do chamado|NOVA|
|prioridade|varchar|referente ao grau de prioridade do chamado|MEDIA|
|usuario_atribuido|varchar|referente ao usuário responsável pelo chamado|GERSON
|data_inicio|date|referente a data que foi iniciada a execução do chamado|2023-09-11|
|data_inicio_desenvolvimento|datetime|referente a data que foi iniciada a execução do chamado|2023-09-12 00:00:00|
|data_previsao|date|referente a data prevista para conclusão do chamado|2023-09-13|
|data_previsao_nova|date|referente a data prevista para conclusão caso haja um adiamento ou nova data|0001-01-01|
|data_atualizacao|datetime|referente a ultima data que o chamado foi atualizado|2023-09-12 09:47:19|
|data_hora_conclusao|datetime|referente a data de conclusão do chamado|0001-01-01 00:00:00|
|data_vizualizado|datetime|referente a data que o chamado concluído foi vizualizado|2023-09-12 09:46:13|
|sub_tarefa_chamado_numero|int|referente a algum numero de subchamado|0|
|tipo_chamado|varchar|referente ao tipo de chamado|SUPORTE|
|usuarios_vizualizado|text|referente aos usuários que podem visualizar o chamado no sistema|COORD.JULIANO;TI.VANDRE|

# **2. SQL**

Query: [fat_soc.sql]
(https://github.com/carminattideh/datasciencia_viaaroma/blob/viaaroma/fat_soc.sql)

## **2.1 Regras de SQL**:
2.1.1. 

2.1.2.

2.1.3. 


## **2.2 Regras de atualização:**

A tabela deverá ser atualizada diariamente as 8 (oito) horas da manhã. 

## **2.3 Validações:**

Descrever quais são alguns dos resultados esperados e como pode ser efetuada a validação dos dados na tabela. Ex.:

- Contagem de valores no período entre Jan e Fev/2020.
- Soma da coluna _x_ para o cliente _y_ deve ser _z_ entre o período de _a_ e _b_
- etc.

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
