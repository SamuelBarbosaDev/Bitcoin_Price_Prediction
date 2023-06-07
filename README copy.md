# Bitcoin Price Prediction:
## Objetivo: 
Defini qual é a melhor loja para espandir o seu tamanho com base no seu desempenho nos últimos 3 anos.

## Metricas:
1. Faturamento anual.
2. Faturamento total.
3. Vendas durante os feriados (Super Bowl, o Dia do Trabalho, o Dia de Ação de Graças e o Natal).
4. Média de vendas semanais.
5. Crescimento do faturamento ano a ano.

## Observações:
Primeiro, nosso objetivo é definir qual é a melhor loja para expandir o seu tamanho com base no seu desempenho nos últimos 3 anos. Tendo isso em mente, é preciso obter mais informações além do faturamento nos últimos anos para definir se a loja em questão deve ou não ser expandida. Por exemplo, é importante considerar o lucro, o custo operacional da loja, a quantidade de funcionários, a localização, a taxa de desemprego na região e a legislação da área. Por exemplo, na Califórnia, uma lei transformou pequenos delitos avaliados em até US$ 950 em contravenção, o que significa que há uma penalidade, mas os criminosos não são presos.

Segundo, com exceção dos dados cuja fonte é o próprio Walmart, como Store, Date, Weekly_Sales e Holiday_Flag, todos os outros dados não são confiáveis, pois não há como verificar nenhum deles. Estamos falando do Walmart, uma empresa multinacional. Como posso tomar uma decisão com base em variáveis como Temperature, fuel_Price, CPI e Unemployment, se não sei onde cada uma das lojas está localizada?

Terceiro, partindo do pressuposto de que as seguintes informações (Temperature, fuel_Price, CPI e Unemployment) são verdadeiras, não encontrei nenhuma correlação positiva ou negativa que afete as vendas semanais.

Como pode ver, há várias variáveis que influenciam na nossa tomada de decisão. Portanto, antes de determinarmos qual é a melhor loja para investir, precisamos responder a todas as perguntas anteriores ou, pelo menos, à maioria delas.

## Insights técnicos da análise:

1. Por fim, mas não menos importante, criei um `algoritmo de ranqueamento de lojas`. Esse algoritmo consiste em atribuir notas as lojas. Cada critério estipulado tem um peso maior ou menor dependendo do caso, sendo que a nota máxima que uma loja pode receber é 320. Chegou o momento de ranquear das lojas. Os critérios utilizados para ranqueá-las foram: `Faturamento Total`, a loja que tiver o maior faturamento ganhará 30 pontos; `Faturamento em 2010`, a loja que tiver o maior faturamento em 2010 ganhará mais 10 pontos; `Faturamento em 2011`, a loja que tiver o maior faturamento em 2011 ganhará mais 10 pontos; `Faturamento em 2012`, a loja que tiver o maior faturamento em 2012 ganhará mais 10 pontos; `Crescimento do Faturamento`, a loja que tiver o maior Crescimento do Faturamento nos ultimos 3 anos ganhará mais 50 pontos; `Venda Total Nos Feriados`, a loja que tiver a maior Venda Total Nos Feriados ganhará 30 pontos; `Venda Nos Feriados em 2010`, a loja que tiver a maior Venda Nos Feriados em 2010 ganhará mais 20 pontos; `Venda Nos Feriados em 2011`, a loja que tiver a maior Venda Nos Feriados em 2011 ganhará mais 20 pontos; `Venda Nos Feriados em 2012`, a loja que tiver a maior Venda Nos Feriados em 2012 ganhará mais 20 pontos; `Crescimento das Vendas Nos Feriados`, a loja que tiver o maior Crescimento das Vendas Nos Feriados nos ultimos 3 anos ganhará mais 50 pontos; `Média de vendas semanais`, a loja que tiver a maior Média de vendas semanais nos ultimos 3 anos ganhará mais 20 pontos.

Critérios  | Notas
---------- | ----
Faturamento Total   | 30
Faturamento em 2010 | 10
Faturamento em 2011 | 10
Faturamento em 2012 | 10
Crescimento do Faturamento | 50
Venda Total Nos Feriados | 30
Venda Nos Feriados em 2010 | 20
Venda Nos Feriados em 2011 | 20
Venda Nos Feriados em 2012 | 20
Crescimento das Vendas Nos Feriados | 50
Média de vendas semanais | 20

---
Linkedin: <https://www.linkedin.com/in/samuel-barbosa-dev/> 

E-mail: <samueloficial@protonmail.com>