# MANUAL DE INTEGRAÇÃO SUITE MPONTOM

###### Este documento tem como finalidade apresentar à equipe de desenvolvimento da empresa parceira informações essenciais para a integração do módulo MARGEM, versão 5.0, ao seu sistema, assim como orientar sobre as consultas que devem ser viabilizadas e os retornos previstos pela ferramenta.

###### O cliente MARGEM é compatível com os seguintes sistemas de gerenciamento de banco de dados:
 - MYSQL
 - MS SQL SERVER
 - POSTGRESQL
 - MARIADB
 - FIREBIRD
 - ORACLE

### 1 - TOTAL VENDIDO, CUSTO E LUCRO (DIÁRIO)

###### SUGESTÃO DE PARAMETROS: ID E DATA (DATETIME);

##### EXEMPLO DE RETORNO
| | TOTAL VENDIDO | CUSTO | LUCRO |
| :---: | :---: | :---: | :---: |
| TIPO | FLOAT | FLOAT | FLOAT |
| VALOR| 45000 | 27000 | 18000 |

### 2 - TICKET MÉDIO (DIÁRIO)

###### SUGESTÃO DE PARAMETROS: ID E DATA (DATETIME);

##### EXEMPLO DE RETORNO 
| | TICKET MÉDIO |
| :---: | :---: |
| TIPO  | FLOAT |
| VALOR | 45000 |

### 3 - MÉDIA DE PRODUTOS POR ATENDIMENTO (DIÁRIO)

###### SUGESTÃO DE PARAMETROS: ID E DATA (DATETIME);

##### EXEMPLO DE RETORNO 
| | PRODUTOS POR ATENDIMENTO |
| :---:| :---: |
| TIPO | FLOAT |
| VALOR | 45000 |

### 4 - CUPONS VÁLIDOS (DIÁRIO)

###### SUGESTÃO DE PARAMETROS: ID E DATA (DATETIME);

##### EXEMPLO DE RETORNO 
|       | CUPONS |
| :---: | :---: |
| TIPO | INTERGER |
| VALOR | 45000 |

### 5 - CUPONS CANCELADOS (DIÁRIO)

###### SUGESTAO DE PARAMETROS: ID E DATA (DATETIME);

##### EXEMPLO DE RETORNO 
|       | CUPONS CANCELADOS |
| :---: |:---: |
| TIPO | INTERGER |
| VALOR |45000

### 6 - VENDAS POR FAIXA-HORÁRIA (DIÁRIO)

###### SUGESTÃO DE PARAMETROS: ID E DATA (DATETIME);

##### EXEMPLO DE RETORNO 

|       | HORA | VALOR | CUPONS | ITENS | MEDIA ITENS | VEDIA VALOR | 
| :---: | :---: | :---: | :---: | :---: |  :---: | :---: | 
| TIPO | INTEGER | FLOAT | INTEGER | INTERGER | FLOAT | FLOAT |
| VALOR | 8 | 450.50 | 34 | 230 | 78.4 | 22.30| 

### 7 - OS 200 PRODUTOS MAIS VENDIDOS (DIÁRIO)

###### SUGESTÃO DE PARAMETROS: ID E DATA (DATETIME);

##### EXEMPLO DE RETORNO 

|       | EAN | DESCRICAO | V.UNITÁRIO | QUANT | V.TOTAL | CUSTO | LUCRO |
|:---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| TIPO | STRING | STRING | FLOAT | FLOAT | FLOAT | FLOAT | FLOAT |
| VALOR | 7894900709841 | REFR COCA COLA LATA | 7.90 | 3 | 23.70 | 3.25 | 4.65 |

### 8 - OS 10.000 PRODUTOS MAIS VENDIDOS (DIÁRIO)

###### SUGESTÃO DE PARAMETROS: ID E DATA (DATETIME);

##### EXEMPLO DE RETORNO 

|       | EAN | DESCRICAO | V.UNITÁRIO | QUANT | V.TOTAL | CUSTO | LUCRO |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| TIPO  | STRING | STRING | FLOAT | FLOAT | FLOAT | FLOAT | FLOAT |
| VALOR | 7894900709841 | REFR COCA COLA LATA | 7.90 | 3 | 23.70 | 3.25 | 4.65 |


### 9 - TOTAL VENDIDO POR MODALIDADE (DIÁRIO)

###### SUGESTÃO DE PARAMETROS: ID E DATA (DATETIME);

##### EXEMPLO DE RETORNO 

|       | CODIGO | DESCRICAO | QUANTIDADE | TOTAL |
| :---: | :---: | :---: | :---: | :---: |
| TIPO  | INTERGER | STRING | INTERGER | FLOAT |
| VALOR |     1    | DINHEIRO|  290 | 35900 |

### 10 - ESTORNOS DE CUPONS (DIÁRIO)

###### SUGESTÃO DE PARAMETROS: ID E DATA (DATETIME);

##### EXEMPLO DE RETORNO 

|       | PDV | DATA | HORA | OPERADOR | SUPERVISOR | CUPOM | VALOR |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| TIPO  | INTERGER | STRING | STRING | STRING | STRING | STRING | FLOAT |
| VALOR |     1    | 2017-05-05 | 07:40:67 | BRUNA | HELIO | 34575976 | 456.98 |

### 11 - DESCONTOS DE ITENS (DIÁRIO)

###### SUGESTÃO DE PARAMETROS: ID E DATA (DATETIME);

##### EXEMPLO DE RETORNO 

|       | DATA   |  HORA  | OPERADOR | SUPERVISOR | CUPOM | VALOR | ITEM | DESCRICAO | EAN |
| :---: | :---:  | :---:  |   :---:  |   :---:    | :---: | :---: | :---: | :---: | :---: |
| TIPO  | STRING | STRING |  STRING  |   STRING   | STRING | FLOAT | INTERGER | STRING | STRING |
| VALOR | 2017-05-05 | 07:40:67 | BRUNA | HELIO | 34575976 | 456.98 | 3 |FRANGO KG | 2002453423 |

### 12 - VENDAS POR SEÇÕES (DIÁRIO)

###### SUGESTÃO DE PARAMETROS: ID E DATA (DATETIME);

##### EXEMPLO DE RETORNO

| | CODIGO | DESCRICAO | QUANTIDADE | VALOR | CUSTO | LUCRO |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| TIPO | INTERGER | STRING | FLOAT | FLOAT | FLOAT |  FLOAT | 
| VALOR | 1 | LIMPEZA | 3456.78 | 12789.90 | 6789.10 | 6000.90 |

### 13 - TOTAL DE CUPONS PROCESSADOS POR OPERADOR (DIÁRIO)

### 14 - VENDAS POR VENDEDOR (DIÁRIO)

### 15 - MODALIDADES POR OPERADOR (DIÁRIO)

### 16 - VENDAS TRANSACIONAIS (DIÁRIO)