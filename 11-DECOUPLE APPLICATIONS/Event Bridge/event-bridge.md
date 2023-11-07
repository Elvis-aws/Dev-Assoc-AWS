
# EventBridge
- It is a serverless service that uses events to connect application components together, making it easier for 
  you to build scalable event-driven applications
- Use it to route events from sources such as home-grown applications, AWS services, and third-party software to consumer 
  applications across your organization
- EventBridge provides a simple and consistent way to ingest, filter, transform, and deliver events, so you can build new 
  applications quickly 
- EventBridge event buses are well suited for many-to-many routing of events between event-driven services
- EventBridge Pipes is intended for point-to-point integrations between these sources and targets, with support for 
  advanced transformations and enrichment

- Serverless event bus used in handling pub-sub patterns
- Apps can subscribe to event bus and publish when an event occurs
- Create a serverless event bus and use it to injest events from a variety of sources including Saas apps
- Create rules which are filters
- Up to 300 rules per event bus
- Messages matching a particular rule will be sent to it (Content based filtering)
- You can connect up to 5 targets to any rule
- If target fails to deliver, use exponential back-off for up to 24 hours
- Use DLQ to targets incase event is not delivered