
# Formação Kafka (Curso Alura)

#### Baixar o kafka

Link: https://kafka.apache.org/downloads/

#### COMANDOS
Na pasta do kafka descompactado:

* Subir zookeper  
`bin/zookeeper-server-start.sh config/zookeeper.properties`

* Subir kafka  
`bin/kafka-server-start.sh config/server.properties`

* Criar um topic no kafka  
`bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic LOJA_NOVO_PEDIDO`

* Listar os topics existentes:  
`bin/kafka-topics.sh --list --bootstrap-server localhost:9092`

* Criar um producer  
`bin/kafka-console-producer.sh --broker-list localhost:9092 --topic LOJA_NOVO_PEDIDO`

* Criar um consumidor que le somente as mensagens novas  
`bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic LOJA_NOVO_PEDIDO`

* Criar um consumidor que busca as mensagens desde o inicio  
`bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic LOJA_NOVO_PEDIDO --from-beginning`
	


