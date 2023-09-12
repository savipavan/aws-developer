Application Integration:

AWS AppSync
Amazon EventBridge(Amazon CloudWatch Events)
Amazon Simple Notification Service(Amazon SNS)
Amazon Simple Queue Service(Amazon SQS)
AWS Step Functions
**Amazon EventBridge:** An event coordinator use-case: EBS Snapshot Notification Event

At this point in time there are over 90 AWS services that are able to create these events

Amazon EventBridge is the only event-based service that integrates directly with third party support

**Event Bus:** Each event Bus can have up to 100 rules associated to it types: Default Event Bus, Custom Event Bus, SaaS Event Bus

Rules: important part of Event Bus, can defined where the events can go and when to trigger

When creating rules, you need to specify a target for the event to be passed on to

Targets: are the one who actually do the job. ex: lambda, ec2
Cross Account Events can be possible
Amazon EventBridge is aws cloud watch events rebranded as a EventBridge
- it integrates with AWS services and software as a service provider
- Backwards compatible
- If you're already using CloudWatch Events no changes are needed for cloud formation templates or API calls.

Replaying Events and the EventBridge Archives:
We can archive the events and replay them later time. Set retention period. this will be used for disaster recover times

Schema Registry:

Custom Event Schemes

Code Bindings: Extensions to the schema's visual editor. Allows Visual Studio to easily check the variables. Makes programming a lot easier
- Increases development speed
- Available for Java, Python and TypeScript
- Can be created in any supported AWS Service within EventBridge

EventBridge Vs Amazon Simple Notification Service(SNS)
limitation with SNS:
- Operates with limited parameters
- Easily scales to millions of subscribers
- No direct connectivity to SaaS
- Limited routing capability
- Difficult to trigger a Step Function
- Filtering is limited to attributes only

If we need more complex and sophisticated approach we need to go for EventBridge

EventBridge vs Amazon Kinesis
Key differences:
- Routes events and works as event storage
- Ideal for processing real time data at large scales
- Limited number of consumers that can connect in a single stream
- Each consumer needs to filter relevance of messages.

Summary:
