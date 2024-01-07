# docker-app

list of app docker base yml file

docker exec -it <kafka*conatiner_id> /bin/sh
cd /opt/kafka*<version>/bin
kafka-topics.sh --create --zookeeper zookeeper:2181 --replication-factor 1 --partitions 1 --topic quickstart
kafka-console-producer.sh --topic quickstart --bootstrap-server localhost:9092
kafka-console-consumer.sh --topic quickstart --from-beginning --bootstrap-server localhost:9092
