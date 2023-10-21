# Detecção de Fraude em Cartão de Crédito em Tempo Real

## Descrição

Este projeto visa identificar transações fraudulentas em cartões de crédito em tempo real, aprendendo e analisando os hábitos de gastos anteriores dos titulares de cartões. Ao detectar desvios desses hábitos, a plataforma sinaliza possíveis atividades fraudulentas, permitindo uma intervenção rápida e eficaz.

## Como Funciona

1. **Análise de Hábitos de Gastos:** Com base no histórico de transações, o sistema aprende padrões como valor, comerciantes frequentes, frequência de compras e tipo de produtos adquiridos.
2. **Verificação em Tempo Real:** Cada nova transação é comparada com o comportamento de gasto anteriormente aprendido.
3. **Detecção e Alerta:** Se uma transação desvia significativamente dos padrões aprendidos, ela é classificada como potencialmente fraudulenta e um alerta é gerado no painel.

## Escalabilidade

O sistema é projetado para processar milhões de transações. Para isso, utilizamos estruturas distribuídas que garantem uma análise eficiente e escalabilidade à medida que o volume de transações cresce.

## Tecnologias Utilizadas

- **Spark 2.2:** Para processamento distribuído de dados.
- **Kafka:** Para streaming de dados em tempo real.
- **Cassandra:** Como solução de armazenamento distribuído.
- **Airflow:** Para automação de jobs do Spark.
