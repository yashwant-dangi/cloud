- SQS - queue model
- SNS - pub/sub model
- Kinesis - real time streaming model

## Amazon SQS - Standard Queue

- default retention is 4 days and maximum retention is 14 days
- Limitation of 256KB per message sent
- SQS provides a cloudwatch metric - queue length (ApproximateNumberOfMessages) for the auto scaling group

## Dead Letter Queue

- when a message reached the MaximumReceive Threshold then it will moved to DLQ (useful for debugging)

## FIFO Queue

- ordering of messages
- with limited throughput 300 msg/s with batching
- with batching throughput is 3000 msg/s

## SNS

- Topic Publish (using the SDK)
- Direct Publish (for mobile apps SDK)

## kinesis

- collect, process and analyze streaming data in real-time

## 197 - Data Order for Kinesis vs SQS FIFO

- For Kinesis
- send using a "partition key"
- The same key will always go to the same shard
- For SQS FIFO
- You want to scale the number of customers, but you want messages to be "grouped" when they are related to each other
- Then you use a Group ID (similar to Partition Key in Kinesis)

## 198 - SQS vs SNS vs Kinesis

| SQS                                 | SNS                          | Kinesis                             |
| ----------------------------------- | ---------------------------- | ----------------------------------- |
| Consumer Pull Data                  | Push Dat to many subscribers | Standard: Pull Data - 2MB per shard |
|                                     | Up to 12500000 subscribers   | Enhanced Fan Out: - Push Data -     |
|                                     |                              | 2MB per shard per customer          |
| Data is deleted after consumed      | Data is not persisted        | Possibility to replay data          |
| can have as many workers            | Pub/Sub                      | Meant for real time big data        |
| Order guarantees only on FIFO Queue |                              | Ordering at the shard level         |

## 199 - Amazon MQ

- Amazon MQ is managed message broker service for
  - RabbitMQ
  - ActiveMQ
