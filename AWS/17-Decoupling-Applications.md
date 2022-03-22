- SQS - queue model
- SNS - pub/sub model
- Kinesis - real time streaming model

## Amazon SQS - Standard Queue

- default retention is 4 days and maximum retention is 14 days
- Limitation of 256KB per message sent
- SQS provides a cloudwatch metric - queue length (ApproximateNumberOfMessages) for the auto scaling group
