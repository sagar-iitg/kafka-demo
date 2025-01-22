
# Start Zookeeper server in the background
bin/zookeeper-server-start.sh config/zookeeper.properties


# Start Kafka server in the background
bin/kafka-server-start.sh config/server.properties

ps aux | grep zookeeper



curl -X POST http://localhost:8080/send -H "Content-Type: application/json" -d "\"Hello, sk"