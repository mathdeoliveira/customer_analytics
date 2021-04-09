# Customer Analytics

<center><img src='https://image.freepik.com/vetores-gratis/analista-de-cro-e-especialista-aumentam-a-porcentagem-de-clientes-otimizacao-da-taxa-de-conversao-sistema-de-marketing-digital-conceito-de-marketing-de-atracao-de-chumbo-ilustracao-de-vetor-isolado-de-coral-rosa_335657-2292.jpg'/>

<a href='https://br.freepik.com/vetores/desenho-animado'>Desenho animado vetor criado por vectorjuice - br.freepik.com</a></center>


A análise dos cliente é de suma importância para as empresas, pois a maioria vão lidar com cliente, seja com os seus serviços ou produtos, assim precisamos criar processos pelo qual os dados comportamentais deles são usados para otimizar e melhorar as tomadas de decisões de negócio.

## O que é customer analytics?

Existe diversas definições, mas podemos entender customer analytics como o uso dos dados providos de diversas fontes para entender: comportamento de compra, fidelidade do cliente, reduzir custos de campanha de marketing, otimizar experiência do usuário, encontrar insights, etc.

E atualmente temos fontes de dados gerando um grande volume, nada melhor que utilizar esse "problema" para nos ajudar a solucionar toda a análise de dados dos nosso clientes.

### Com customer analytics podemos nos beneficiar

Já que podemos ter um volume grande de dados, podemos utilizar isso como o novo petróleo para entender toda esfera dos clientes, com isso podemos nos beneficiar, por exemplo:

* **Campanha de marketing**

Com o conhecimento que podemos extrair dos clientes, podemos criar campanhas mais assertivas para cada grupo de cliente até individualmente, melhorando e otimizando o target das campanhas diminui os custos e aumenta o retorno.

* **Comportamento de compra**

Podemos criar método de precifição inteligentes de acordo com a demanda, oferecer produtos na hora e no momento certo para os clientes, solucionar alguma necessidade dos clientes.

* **Experiência do usuário**

Criar técnicas para identificar variáveis chaves que mais impacta na experiência que o usuário tem na loja, produto, serviço, melhorando essa experiência o cliente pode comprar mais, retornar mais vezes e indicar.

* **Fidelidade**

Entregando de forma otimizada e específica, no momento certo, produto/serviço com as características corretas, com o preço ideal melhorar a fidelidade desse cliente com a marca, essencial para um relacionamento a longo prazo, algo que todas empresas buscam.

E diversos outros benefícios!

### Métrica para customer analytics

Visto que temos inúmeras formas de cruzar as informações sobre um cliente, não existe uma métrica de avaliação de performance, mas sim várias delas, vai depender da necessidade do negócio e o que temos de dados disponíveis. Podemos citar algumas, sendo elas:

Revenda, Customer Lifetime, Intenção de compra, Devolução dos produtos, Satisfação, Taxa de conversão, etc.

## 1. Objetivo do nosso projeto
Este projeto tem como objetivo mostrar algumas técnicas de customer analytics para conhecer os nossos clientes, segmentação, cohorts, análise de compras e predição.  

Em uma das nossas técnicas empregadas aqui vamos nos basear em fundamentos do marketing, como marketing mix e o framework STP e a elasticidade dos preços.

### 1.1. STP Framework
STP vem da sigla em inglês: Segmentation, Targeting and Positioning. É um framework fundamental no marketing, podendo ser aplicado em diversos tipos de negócio.
- **Segmentation**: É o processo de dividir os clientes em grupos que compartilham as mesmas características, assim podemos esse pessoal do mesmo grupo pode ter comportamento de compra e responder a difentes campanhas de marketing de forma semelhante.
- **Targeting**: É o processo de avalição o potencial lucro para cada segmento e decidir qual segmento focar, assim podemos selecionar caminhos de promover os produtos, sendo TV ou on-line.
- **Positioning**: É o processo de oferecer os produtos certos para o segmento que precisa, mostrando como o produto pode ser oferecido para o cliente e qual canal é o mais eficiente. Esse processo é tão importante que existe um fundamento bem conhecido que foi criado, o Marketing Mix.

#### 1.1.1. Marketing Mix
O marketing mix é o famoso 4Ps de marketing, de forma bem sucinta e resumida, temos que:
- **Product**: Características do produto
- **Price**: Preço do produto
- **Promotion**: Redução de preço, forma de mostrar
- **Place**: Distribuição

### 1.2. Elasticidade do preço
Elasticidade do preço é a medida que nos mostra como o interesse de compra muda quando acontece a mudança de preço, sendo acréscimo ou decréscimo. Com isso temos duas forma de visualizar, a primeira sendo a elasticidade própria que é a respeito do mesmo produto e a segunda elasticidade de preço cruzada que é a respeito de diferentes produtos. Existe fórmulas que nos ajuda a calcular, vamos ver elas na parte prática.

## 2. Descrição dos dados

Vamos utilizar os dados providos pelo [UCI Machine Learning Repository](http://archive.ics.uci.edu/ml/), e, de acordo com a definição disponibilizada por eles, este é um dataset transnacional que contém todas as transações ocorridas entre 01/12/2009 and 09/12/2011 para um varejo on-line sem loja registrada no Reino Unido. A empresa vende principalmente artigos para presentes exclusivos para todas as ocasiões. Muitos clientes da empresa são atacadistas.

### 2.2. Dicionário dos dados

| Coluna      | Descrição |
|-------------|-----------|
| Invoice   | Número da fatura. Nominal, um número integral de 6 dígitos atribuído exclusivamente a cada transação. Se este código começar com a letra 'c', isso indica um cancelamento.          |
| StockCode   |     Código do produto (item). Nominal, um número integral de 5 dígitos atribuído exclusivamente a cada produto distinto.      |
| Description |     Nome do produto (item). Nominal.      |
| Quantity    |       As quantidades de cada produto (item) por transação.Numérico.    |
| InvoiceDate |      Data e hora da fatura. Numérico, o dia e a hora em que cada transação foi gerada.     |
| Price   |      Preço unitário. Numérico, preço do produto por unidade em libras esterlinas.     |
| CustomerID  |     Número do cliente. Nominal, um número integral de 5 dígitos atribuído exclusivamente a cada cliente.      |
| Country     |        Nome do país. Nominal, o nome do país onde cada cliente reside.   |

### 2.3. Business Undestanding

Anteriormente vimos a descrição dos dados que possuimos, são referentes a uma empresa de varejo on-line. A empresa comercializa presentes exclusivos no ambiente virtual, e muito dos clientes da empresa está espalhados em diferentes países.

O mercado de presentes é bem grande, existe diversas datas comemorativas onde as pessoas podem vim a escolher algum produto para presentear, ter um varejo on-line onde as vendas acontece de forma sem intermediários, assim podendo cobrar um valor mais baixo, os consumidores finais podem utilizar para compras.

<center><img alt="Vaga" width="50%" src="https://images.unsplash.com/photo-1484807352052-23338990c6c6?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"></center>

O mercado on-line vem crescendo a cada ano, mais e mais, o cliente busca na internet por diversos produtos pois ele está mais conectado do que antes, a empresa se colocou de forma estratégia aproveitando desse movimento, conseguindo expandir o seu negócio e também diminuindo os custos.

## Análise exploratória dos dados
Vamos explorar os nosso dados, não vou criar uma análise muito complexa, vou manter de forma mais superficial, já que vamos aplicar técnicas analíticas para os clientes.

<center><img alt="Vaga" width="100%" src="https://github.com/mathdeoliveira/customer_analytics/blob/main/describe.PNG?raw=true"></center>

A tabela de descrição acima nos mostra que, a média de quantidade comprada é de aproximadamente 13 unidades e existe um valor outlier de 19152 unidades comprada em um produto. Já o valor unitário do produto temos que, a média e de aproximadamente £3 e que temos um valor máximo de £10.953.

<center><img alt="Vaga" width="100%" src="https://github.com/mathdeoliveira/customer_analytics/blob/main/total_country.PNG?raw=true"></center>

O gráfico acima temos o valor total comprado para cada país do nosso dataset, temos que o Reino Unido é o país que mais compra presentes da empresa, portanto os clientes desse país podem ser os principais para o negócio.

<center><img alt="Vaga" width="100%" src="https://github.com/mathdeoliveira/customer_analytics/blob/main/frequency_customer.PNG?raw=true"></center>

O gráfico acima nos mostra a frequência de compras dos clientes que mais vezes compraram na empresa, temos um cliente que comprou mais que 200 vezes durante todo o tempo. Interessante saber que possuimos em um cliente bastante fiel e assíduo nas compras de presentes, talvez seja alguma pessoa que compra para revender.

## Cohorts
A análise de cohort é ferramenta que ajuda no entendimento do comportamento dos clientes e entender, por exemplo a retenção do cliente ao decorrer do tempo. O Cohort é uma forma de agrupar os clientes onde eles compartilham características em comum, então podemos utilizar essa ferramenta para agrupar os clientes e entender ao longo de tempo as seus comportamentos.

Nesse caso, iremos olhar a retenção do usuário, é importante saber qual é o nível de retenção que a empresa está tendo para saber como a empresa está de saúde, com a análise podemos inferir a lealdade dos clientes com a empresa. E sabemos que reter clientes comprando na empresa é de muita importância, pois é mais barato manter um cliente que já comprou do que adquirir novos clientes.

Dado que não temos na nossa base de dados a data que o cliente se cadastrou na empresa, vamos levar em consideração que a data da sua primeira compra é o data correta onde ele se cadastrou.

<center><img alt="Vaga" width="100%" src="https://github.com/mathdeoliveira/customer_analytics/blob/main/cohort.PNG?raw=true"></center>

O gráfico acima nos mostra a retenção dos clientes, para cada linha temos a porcentagem dos clientes que recompraram dado o número x de períodos após a sua primeira compra. Olhando a primeira coluna, que nos mostra a porcentagem dos clientes que voltaram no segundo mês, temos que em média 80% dos clientes não voltam a comprar, exceto ao primeiro mês 2009-12 que teve 35% dos clientes voltando no segundo mês.

De fato essa linha do mês 2009-12 é a mais positiva para o negócio, seria de grande interesse estudar os motivos dessa causa de reter melhor que outros meses, nessa data tivemos a maior quantidade de clientes, somando 955. Além de um ano depois 50% dos clientes voltaram a recomprar.

Olhando o restante dos cohorts, vemos uma certa sazonalidade, clientes compram pela primeira vez, fica um tempo sem recomprar e após há um aumento da recompra dos mesmos clientes.

De toda forma, isso já nos da uma grande ajuda no entendimento do comportamento de compra do cliente, sendo necessário a aquisição de mais dados e o entendimento mais profundo do modelo de negócio praticado pela empresa para afirmar as nossos insights.

Não precisamos parar por aqui, podemos analisar os cohorts diários, caso queria ver diariamente. Caso tenha bastante dado, podemos até visualizar os cohorts anuais.

Além disso, podemos segmentar os nossos cohorts por diversas óticas, por campanha de marketing, por dispositivos, etc. E não precisamos ver somente por retenção, mas também por conversão dos clientes, receita gerada, enfim, depende da métrica que o negócio necessita no momento.

## Segmentação
### Feature engineering

Vamos desenvolver o processo de feature engineering, para isso vamos utilizar um método de vetorizar os produtos que temos na nossa base para nos ajudar a clusterizar esses produtos e identificar o cluster desse produtos para cada produto e para cada cliente. Além disso, vamos criar algumas novas variáveis a partir das variáveis das quais já possuimos.
 
 
