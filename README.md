# dynamo-db-projeto

### Serviço utilizado
  - Amazon DynamoDB
  - Amazon CLI para execução em linha de comando

---
## Anotações do lab

### Caracteristicas do DynamoDB

Escalabilidade: DynamoDB é um banco de dados altamente escalável que pode ser facilmente dimensionado para lidar com grandes volumes de dados e tráfego de aplicativos. Ele também é capaz de lidar com picos de carga de tráfego sem afetar a performance.

Desempenho: DynamoDB oferece um desempenho de leitura e gravação extremamente rápido, o que o torna uma opção ideal para aplicativos que exigem baixa latência.

Flexibilidade: DynamoDB oferece um modelo de dados flexível que permite armazenar e recuperar dados estruturados e semiestruturados. Ele também oferece suporte a várias linguagens de programação e frameworks.

Baixa manutenção: Como um serviço gerenciado da AWS, o DynamoDB não requer muita manutenção e gerenciamento do banco de dados. A AWS gerencia a infraestrutura, o backup e a recuperação de falhas, permitindo que você se concentre em desenvolver sua aplicação.

Integração com outros serviços da AWS: O DynamoDB é completamente integrado com outros serviços da AWS, como o AWS Lambda, Amazon API Gateway, Amazon S3, Amazon EMR e outros, o que permite que você construa soluções de ponta a ponta na AWS.

Segurança: O DynamoDB é altamente seguro e oferece criptografia de dados em repouso e em trânsito, além de suportar controle de acesso baseado em função.

### Boas práticas dentro do banco de dados

Modelagem de dados: A modelagem de dados é essencial no DynamoDB. Você deve projetar seus esquemas de tabela de acordo com as consultas que sua aplicação realizará. Evite a sobrecarga de leitura/gravação ao projetar suas tabelas de acordo com o uso de sua aplicação. Para obter o melhor desempenho, é recomendado usar a chave de partição e de classificação para acessar dados.

Chaves de partição: A chave de partição é usada para distribuir os itens entre as partições do DynamoDB. Deve ser cuidadosamente escolhida para minimizar a contenção de tráfego em uma única partição.

Chaves de classificação: A chave de classificação é usada para ordenar itens dentro de uma partição. Deve ser escolhida de acordo com a consulta que você deseja executar. Tente usar os tipos de dados suportados pelo DynamoDB, como strings, números e binários.

Escolha de índices: Escolha cuidadosamente os índices globais ou locais para otimizar as consultas de sua aplicação. Os índices globais podem ser usados para consultar em toda a tabela, enquanto os índices locais permitem consultas dentro de uma partição.

Monitoramento: Monitore suas métricas do DynamoDB e use alertas para detectar problemas de desempenho ou erros.

Uso de transações: Use transações do DynamoDB para garantir que as atualizações em várias tabelas sejam atômicas.

Batch Operations: Use as operações em lote do DynamoDB, como batch get e batch write, para reduzir a quantidade de chamadas na API e melhorar o desempenho.

Provisionamento de capacidade: Faça um provisionamento cuidadoso da capacidade de leitura/gravação para evitar custos desnecessários. Use as ferramentas de monitoramento para ajustar a capacidade de acordo com as necessidades de sua aplicação.

Segurança: Configure a segurança corretamente, com controle de acesso baseado em função, criptografia em repouso e em trânsito, e outras práticas recomendadas de segurança.
