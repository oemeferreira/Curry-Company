# 1. Problema de Negócios
A Cury Company, uma empresa de tecnologia especializada em conectar restaurantes, entregadores e clientes, enfrenta a necessidade de aprimorar a visibilidade dos principais indicadores de crescimento. 

Mesmo com um aumento nas entregas, o CEO precisa de uma compreensão abrangente dos KPIs de expansão da empresa. 

Como Cientista de Dados, a missão é criar soluções de dados para otimizar as operações de entrega e, inicialmente, consolidar os principais KPIs estratégicos em uma ferramenta única para facilitar as decisões do CEO.

A Cury Company opera por meio de um modelo de negócios denominado Marketplace, intermediando transações entre restaurantes, entregadores e consumidores. Para acompanhar o crescimento dessas operações, o CEO expressa o desejo de monitorar diversas métricas cruciais.

## Do ponto de vista da empresa:
  1. Número diário de pedidos.
  2. Número semanal de pedidos.
  3. Distribuição dos pedidos por tipo de tráfego.
  4. Comparação do volume de pedidos por cidade e tipo de tráfego.
  5. Quantidade de pedidos por entregador semanal.
  6. Localização central de cada cidade por tipo de tráfego.

## Do ponto de vista do entregador:
  1. Faixa etária dos entregadores.
  2. Condição dos veículos (melhor e pior).
  3. Avaliação média por entregador.
  4. Avaliação média e desvio padrão por tipo de tráfego.
  5. Avaliação média e desvio padrão por condições climáticas.
  6. Top 10 entregadores mais rápidos e lentos por cidade.

## Do ponto de vista dos restaurantes:
  1. Quantidade de entregadores únicos.
  2. Distância média entre restaurantes e locais de entrega.
  3. Tempo médio e desvio padrão de entrega por cidade.
  4. Tempo médio e desvio padrão de entrega por cidade e tipo de pedido.
  5. Tempo médio e desvio padrão de entrega por cidade e tipo de tráfego.
  6. Tempo médio de entrega durante festivais.
  7. O objetivo do projeto é criar gráficos e tabelas que apresentem essas métricas de forma clara e concisa para o CEO.

# 2. Premissas para Análise
  1. A análise utiliza dados do período entre 11/02/2022 e 06/04/2022.
  2. O modelo de negócios considerado é o Marketplace.
  3. Três principais visões do negócio foram identificadas: Visão Transacional de Pedidos, Visão de Restaurantes e Visão de Entregadores.

# 3. Estratégia de Solução
Desenvolvemos um painel estratégico com base nas métricas que refletem as três principais visões do modelo de negócios da empresa:

  1. Visão do crescimento da empresa
  2. Visão do crescimento dos restaurantes
  3. Visão do crescimento dos entregadores

Cada visão é representada pelo seguinte conjunto de métricas.

### 1. Visão do crescimento da empresa
  1. Pedidos diários
  2. Percentual de pedidos por condições de tráfego
  3. Quantidade de pedidos por tipo e por cidade
  4. Pedidos semanais
  5. Quantidade de pedidos por tipo de entrega
  6. Quantidade de pedidos por condições de tráfego e tipo de cidade
  7. Visão do Crescimento dos Restaurantes

### 2. Visão do crescimento dos restaurantes
  1. Quantidade de pedidos únicos
  2. Distância média percorrida
  3. Tempo médio de entrega durante festivais e dias normais
  4. Desvio padrão do tempo de entrega durante festivais e dias normais
  5. Tempo de entrega médio por cidade
  6. Distribuição do tempo médio de entrega por cidade
  7. Tempo médio de entrega por tipo de pedido
  8. Visão do Crescimento dos Entregadores

### 3. Visão do crescimento dos entregadores
  1. Idade do entregador mais velho e mais novo
  2. Avaliação do melhor e pior veículo
  3. Avaliação média por entregador
  4. Avaliação média por condições de tráfego
  5. Avaliação média por condições climáticas
  6. Tempo médio do entregador mais rápido
  7. Tempo médio do entregador mais rápido por cidade

# 4. Principais Insights de Dados
  1. A sazonalidade da quantidade de pedidos é diária, com uma variação de aproximadamente 10% entre dias consecutivos.
  2. Cidades do tipo Semi-Urban não apresentam condições baixas de tráfego.
  3. As maiores variações no tempo de entrega ocorrem durante condições climáticas ensolaradas.
     
# 5. Produto Final do Projeto
Desenvolvemos um painel online, hospedado na nuvem e acessível por qualquer dispositivo conectado à internet. O painel pode ser acessado aqui. [https://curry-company-project.streamlit.app/](https://curry-company-project.streamlit.app/)

# 6. Conclusão
O projeto visa fornecer um conjunto de gráficos e tabelas para apresentar métricas de forma eficaz ao CEO. A análise revelou um crescimento no número de pedidos entre as semanas 06 e 13 de 2022.

# 7. Próximos Passos
  1. Reduzir o número de métricas para simplificar a visualização.
  2. Introduzir novos filtros para aprimorar a análise.
  3. Adicionar novas visões de negócio para uma compreensão mais abrangente.
