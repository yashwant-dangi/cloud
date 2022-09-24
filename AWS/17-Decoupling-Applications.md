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
