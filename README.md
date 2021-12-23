# kafka
Implementação simples do kafka

Clone do projeto-> git clone https://github.com/confluentinc/kafka-images.git

Entrar na pasta 'kafka-images/examples/single-node'

Subir o kafka e zookeeper -> docker-compose up -d

Comando para criação do tópico: 

    docker-compose exec kafka kafka-topics --create --topic EXEMPLO_TOPICO --bootstrap-server localhost:9092 --partitions 1 --replication-factor 1

Comando para verificar se o tópico foi criado corretamente:

    docker-compose exec kafka kafka-topics --describe --topic EXEMPLO_TOPICO --bootstrap-server localhost:9092

