## CloudWatch

- Metrics

- Logs
  CloudWatch Logs can use filter expressions
  For example, find a specific IP inside of a log
  Metric Filter can be used to trigger CloudWatch alarms

## CloudWatch Agent and CloudWatch Logs Agent

- By default no logs from EC2 will go to cloudwatch
- Need to run a cloudwatch agent on EC2 to push the log files you want

  - CloudWatch Logs Agent - old version of the agent
  - CloudWatch Unified Agent - collect additional system level metrics such as RAM, processes

## CloudWatch Alarms

- Alearms are used to trigger notifications for any metric
- Alear Targets
  - Stop, Terminate, Reboot or Recover an EC2 Instance
  - Trigger Auto Scaling Action
  - Send notification to SNS

## Amazon EventBridge (formerly CloudWatch Events)
