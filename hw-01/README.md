# kafka-homework 01
# Шаги
1) Запуск Kafka и Zookeeper через Docker-Compose
png1.png
2) Создание топика командой 
bin\windows\kafka-topics.bat --create --topic test --bootstrap-server localhost:19092
bin\windows\kafka-topics.bat --describe --topic test --bootstrap-server localhost:19092
png2.png
3) Запишем сообщения
bin\windows\kafka-console-producer.bat --topic test --bootstrap-server localhost:19092 test_msg_1
bin\windows\kafka-console-producer.bat --topic test --bootstrap-server localhost:19092 test_msg_2
png3.png
4) Читаем записи
bin\windows\kafka-console-consumer.bat --topic test --from-beginning --bootstrap-server localhost:19092