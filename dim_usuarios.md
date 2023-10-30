# **1. Informações gerais**
## **1.1 Responsável:** 
[Deborah Carminatti](https://viaaroma.my3cx.com.br:5001/deborah) - Analista de Dados Senior

[Bruna Barbosa](https://viaaroma.my3cx.com.br:5001/bruna) - Analista de Dados Jr.

## **1.2 Objetivo**: 
Esta tabela se refere aos usuários do sistema SIG, seus respectivos cargos, gestores e área.

## **1.3 Estrutura da Tabela:**
|campo|formato|descricao|exemplo|
|--|--|---|---|
|usuario|varchar|referente ao nome de usuario no sistema sig|AIRTON|
|area|varchar|referente a area de atuacao do usuario|PRODUCAO|
|gestao|varchar|referente ao gestor(a) do usuario|JULIANO|
|cargo|varchar|referente cargo do usuario|LIDER|




# **2. SQL**

Query: [dim_usuarios_area.sql]
(https://github.com/carminattideh/datasciencia_viaaroma/blob/viaaroma/dim_usuarios_area.sql)

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
tabela1.coluna = tabela2.coluna
tabela1.coluna1 = tabela3.coluna
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
