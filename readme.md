# Under Construction

# Kafka

## Notes
# Notes

- The software under `kafka` directory is downloaded from official website. However, there are some fixes I implemented. You may want to download itself from `https://kafka.apache.org/downloads`
- Please use Git Bash as terminal for Windows 10.

## Run Kafka on localhost

```bash
sh C:\\Users\\user\\Desktop\\Desk\\projects\\dotnet-third-party-integrations-core\\kafka\\bin\\zookeeper-server-start.sh C:\\Users\\user\\Desktop\\Desk\\projects\\dotnet-third-party-integrations-core\\kafka\\config\\zookeeper.properties
```

```bash
sh C:\\Users\\user\\Desktop\\Desk\\projects\\dotnet-third-party-integrations-core\\kafka\\bin\\kafka-server-start.sh C:\\Users\\user\\Desktop\\Desk\\projects\\dotnet-third-party-integrations-core\\kafka\\config\\server.properties
```

```bash
sh C:\\Users\\user\\Desktop\\Desk\\projects\\dotnet-third-party-integrations-core\\kafka\\bin\\kafka-consumer-groups.sh --bootstrap-server localhost:9092 --describe --group PigeonApp --offsets
```

## Test Kafka

```bash
sh C:\\Users\\user\\Desktop\\Desk\\projects\\dotnet-third-party-integrations-core\\kafka\\bin\\kafka-topics.sh --create --topic ContactIsCreated --bootstrap-server localhost:9092 --partitions 1 --replication-factor 1
```

```bash
sh C:\\Users\\user\\Desktop\\Desk\\projects\\dotnet-third-party-integrations-core\\kafka\\bin\\kafka-console-producer.sh --topic ContactIsCreated --bootstrap-server localhost:9092
```

```bash
C:\\Users\\user\\Desktop\\Desk\\projects\\dotnet-third-party-integrations-core\\kafka\\bin\\kafka-console-consumer.sh --topic ContactIsCreated --bootstrap-server localhost:9092 --from-beginning
```



