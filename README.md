# Curry Company — Painel Operacional de Entregas

Painel estratégico que consolida os KPIs de um marketplace de delivery em uma única ferramenta, organizado nas três visões que o negócio realmente usa para decidir: **empresa**, **restaurantes** e **entregadores**.

### [→ Acessar o painel](https://curry-company-project.streamlit.app/)

---

## Problema de negócio

A Curry Company conecta restaurantes, entregadores e clientes em um modelo de marketplace. O volume de entregas cresce, mas o CEO não tem visibilidade dos indicadores que explicam esse crescimento — os números existem espalhados e nenhuma leitura consolidada chega até ele.

A missão: transformar a base operacional em um painel único, capaz de responder às perguntas de crescimento sem depender de alguém abrir um notebook.

---

## Premissas

- Dados do período entre **11/02/2022 e 06/04/2022**
- Modelo de negócio considerado: marketplace
- Três visões de negócio, cada uma com seu próprio conjunto de métricas

---

## O painel

| Visão | O que responde |
|---|---|
| **Empresa** | Pedidos diários e semanais, distribuição por condição de tráfego, volume por tipo de cidade, pedidos por tipo de entrega e localização central por cidade |
| **Restaurantes** | Entregadores únicos, distância média percorrida, tempo médio e desvio padrão de entrega por cidade e por tipo de pedido, comparação entre festivais e dias normais |
| **Entregadores** | Faixa etária, condição dos veículos, avaliação média por entregador, por tráfego e por clima, e os entregadores mais rápidos por cidade |

Cada visão é uma página independente em `pages/`, com filtros de data e de condição de trânsito aplicados na barra lateral.

---

## Principais insights

1. **A sazonalidade dos pedidos é diária**, com variação de aproximadamente 10% entre dias consecutivos — o planejamento de escala precisa ser diário, não semanal.
2. **Cidades do tipo Semi-Urban não registram condições baixas de tráfego**, o que muda a expectativa de tempo de entrega nessas praças.
3. **As maiores variações no tempo de entrega ocorrem em clima ensolarado**, resultado contraintuitivo que merece investigação: o esperado seria o oposto.

O volume de pedidos cresceu entre as semanas 06 e 13 de 2022.

---

## Como rodar

```bash
pip install -r requirements.txt
streamlit run Home.py
```

O painel sobe em `http://localhost:8501`.

Requer **Python 3.9 ou superior**.

---

## Estrutura

```
Home.py                    pagina inicial e descricao do painel
pages/
  visao_empresa.py         KPIs de crescimento da operacao
  visao_restaurantes.py    tempo e distancia de entrega
  visao_entregadores.py    avaliacoes e performance
dataset/train.csv          base operacional
```

---

## Tecnologias

Python · Pandas · NumPy · Streamlit · Plotly · Folium · Haversine

O cálculo de distância entre restaurante e local de entrega usa a fórmula de **Haversine** sobre as coordenadas de origem e destino.

---

## Próximos passos

1. Reduzir o número de métricas por tela — hoje há densidade demais para leitura rápida
2. Introduzir novos filtros de recorte
3. Adicionar visões de negócio complementares

---

## Observações

- Os dados vêm de uma base pública de exemplo. Nenhum número aqui representa operação real de empresa.
- Projeto desenvolvido durante a formação em análise de dados da Comunidade DS.
