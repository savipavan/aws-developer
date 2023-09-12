Application Integration:
1. AWS AppSync
2. Amazon EventBridge(Amazon CloudWatch Events)
3. Amazon Simple Notification Service(Amazon SNS)
4. Amazon Simple Queue Service(Amazon SQS)
5. AWS Step Functions

Amazon EventBridge:
An event coordinator
use-case: EBS Snapshot Notification Event

At this point in time there are over 90 AWS services that are able to create these events

Amazon EventBridge is the only event-based service that integrates directly with third party support

Event Bus: Each event Bus can have up to 100 rules assocaited to it
types: Default Event Bus, Custom Event Bus, SaaS Event Bus

Rules: important part of Event Bus, can defined where the events can go and when to trigger

When creating rules, you need to specify a target for the event to be passed on to

Targets: are the one who actually do the job. ex: lambda, ec2
