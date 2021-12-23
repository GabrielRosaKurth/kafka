# kafka
Implementação simples do kafka

Descompacte o arquivo encontrado em /resources

Comando para subir o zookeper -> ./bin/zookeeper-server-start.sh config/zookeeper.properties

Comando para subir o kafka -> ./bin/kafka-server-start.sh config/server.properties

Comando para criar um tópico simples -> ./kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic EXAMPLE_TOPIC

Comando para se conectar ao producer via terminal -> ./kafka-console-producer.sh --broker-list localhost:9092 --topic EXAMPLE_TOPIC

Comando para se conectar ao consumer via terminal -> ./kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic TEST_TOPIC --from-beginning
