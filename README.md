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

