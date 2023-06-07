# Bitcoin Price Prediction:
### Índice

- [Contextualização](#contextualização)
- [Metodologia Aplicada](#metodologia-aplicada)
- [Entendimento do Negócio Aplicada](#metodologia-aplicada)
  - [Metricas](#metricas)
- [Entendimento dos Dados](#entendimento-dos-dados)
  - [Variáveis](#variáveis)
  - [Shape](#shape)
  - [Describe](#describe)
  - [Verificando Valores Nulos](#verificando-valores-nulos)
  - [Verificando Valores Duplicados](#verificando-valores-duplicados)
  - [Verificando Tipos](#verificando-tipos)
  - [Verificando a distribuição da coluna 'sales'](#verificando-a-distribuição-da-coluna-sales)
  - [Identificando outliers](#identificando-outliers)
  - [Identificando correlação](#identificando-correlação)
  - [Investimento por plataforma](#investimento-por-plataforma)

- [Preparação dos Dados](#preparação-dos-dados)
  - [Removendo nulos](#removendo-nulos)

- [Modelagem](#modelagem)

- [Avaliação](#avaliação)
- [Implantação](#implantação)

- [Ambiente virtual e Dependências](#ambiente-virtual-e-dependências)


### Contextualização:
Considere o preço diário do Bitcoin disponível na coluna “PriceUSD” da tabela “https://coinmetrics.io/newdata/btc.csv". Faça um algoritmo (python, R , Excel...) bem simples (média movel, regressão linear,etc..) para prever o preço do dia seguinte. Compartilhe o código, brevemente explique o seu funcionamento e apresente alguns resultados.

### Metodologia Aplicada:
A análise foi realizada utilizando o modelo CRISP-DM, o CRISP-DM (Cross Industry Standard Process for Data Mining) é um modelo padrão de processo para projetos de mineração de dados que define um conjunto de fases e tarefas que devem ser executadas para desenvolver soluções de mineração de dados efetivas.

![CRISP-DM](/core/img/CRISP-DM.png)

O modelo CRISP-DM é uma abordagem sistemática e estruturada para a mineração de dados que ajuda as empresas a desenvolver soluções de mineração de dados de maneira eficiente e eficaz, reduzindo o tempo e os custos do projeto.

## Entendimento do Negócio:

### Objetivo:
Prever o preço do Bitcoin no dia seguinte.

### Variavel Targat:
“PriceUSD”.

### Metricas:
Análisei a correlação entre o `PriceUSD` e as demais variáveis.

## Entendimento dos Dados:
### Variáveis:
![Data Frame](/core/img/dataframe.png)

### Shape:
![Data Frame](/core/img/shape.png)

### Describe:
![Data Frame](/core/img/describe.png)

### Verificando Valores Nulos:
![Data Frame](/core/img/nulos.png)

### Verificando Valores Duplicados:
![Data Frame](/core/img/duplicados.png)

### Verificando Tipos:
![Data Frame](/core/img/tipos.png)

### Verificando a distribuição da coluna 'PriceUSD':
![Data Frame](/core/img/distribuição.png)

### Reta de Regressão:
![Data Frame](/core/img/reta_de_regressão.png)

### Identificando correlação:
![Data Frame](/core/img/correlação.png)

## Preparação dos Dados:
### Removendo nulos:
![Data Frame](/core/img/removendo_nulos.png)

## Modelagem:
### Verificando o desempenho do modelo:
![Data Frame](/core/img/modelo.png)

## Avaliação:
Existem várias observações que precisam ser levantadas. Primeiramente, para que possamos realizar um estudo preciso, é necessário uma documentação mais completa dos dados, uma vez que temos 147 variáveis (colunas). Portanto, um estudo mais aprofundado dos dados se faz necessário.

Em segundo lugar, nosso objetivo com este projeto é prever o preço do Bitcoin no dia seguinte. No entanto, prever os preços diários gera muito ruído, o que dificulta a previsão. Portanto, minha recomendação é aumentar o intervalo de tempo do estudo.

Em terceiro lugar, uma regressão linear simples não é suficiente para prever o preço do Bitcoin. É necessário, no mínimo, uma regressão linear múltipla, levando em consideração várias variáveis interessantes, como hashrate, taxa (fee), sentimento de mercado (fear), o preço mínimo pelo qual os mineradores estão vendendo os Bitcoins minerados, nível de adoção, entre outros.

## Implantação:
Iniciando a etapa de implementação do modelo em produção.

## Ambiente virtual e Dependências:
Criando ambiente virtual:
```
python3 -m venv core/.venv
```

Entrando no ambiente virtual:
```
source core/.venv/bin/activate
```

Instale as dependências:
```
pip install -r core/requirements.txt
```
---
Linkedin: <https://www.linkedin.com/in/samuel-barbosa-dev/> 

E-mail: <samueloficial@protonmail.com>