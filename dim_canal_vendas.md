# **1. Informações gerais**
## **1.1 Responsável:** 
[Deborah Carminatti](https://viaaroma.my3cx.com.br:5001/deborah) - Analista de Dados Senior

[Bruna Barbosa](https://viaaroma.my3cx.com.br:5001/bruna) - Analista de Dados Jr.

## **1.2 Objetivo**: 
Esta tabela lista os cadas de venda existentes e seus respectivos tipos de venda.

## **1.3 Estrutura da Tabela:**
|campo|formato|descricao|exemplo|
|--|--|---|---|
|canal_venda|varchar|descrição do canal de venda|LOJA VIRTUAL|
|tipo_venda|varchar|descrição do tipo de venda do canal|B2B|

# **2. SQL**

Query: [dim_canal_venda.sql]
(https://github.com/carminattideh/datasciencia_viaaroma/blob/viaaroma/dim_canal_venda.sql)

## **2.1 Regras de SQL**:
2.1.1. Tipo de venda
```
CASE
        WHEN canal_venda IN ('MARKETPLACE' , 'LOJA VIRTUAL') THEN 'B2C'
        WHEN canal_venda = 'sac' THEN 'SAC'
        WHEN canal_venda = 'LOJISTA' THEN 'B2B'
    END 'tipo_venda'
```
2.1.2. Canal de Venda
```
CASE
        WHEN razao_social IN ('SHOPEE' , 'MARKETPLACE', 'AMAZON', 'MERCADO LIVRE', 'MAGALU', 'AMERICANAS') THEN 'MARKETPLACE'
        WHEN razao_social IN ('SAC' , 'LOJA VIRTUAL') THEN razao_social
ELSE 'LOJISTA'
    END canal_venda
```

## **2.2 Regras de atualização:**

A tabela deverá ser atualizada semanalmente as 7 (sete) horas da manhã. 

## **2.3 Validações:**
N/A

# **3. Fluxos de Dados:** 
N/A

## **3.1 Workspace:** 
N/A

### 10. Fluxos:


## **3.1 Power Automate:** 


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
dim_canal_vendas.canal_venda = dim_vendedores_canal_vendas.canal_venda

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
