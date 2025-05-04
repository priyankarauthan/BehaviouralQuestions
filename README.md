# BehaviouralQuestions


### Q1- Apple is known for innovation. Tell me about a time when you came up with a creative solution to a difficult problem.

Sample Answer:-

In one of my recent projects, we were dealing with performance bottlenecks while syncing large volumes of CRM data between our internal system and third-party CRMs like Salesforce and Zoho. The system was timing out and struggling to handle concurrent data sync requests, especially during peak load hours.

Instead of going with a traditional batch-processing fix, I proposed implementing an event-driven architecture using Kafka. I broke the data sync process into stages: ingestion, transformation, and persistence — each triggered by Kafka topics. We also introduced parallel processing using consumer groups, which drastically improved throughput.

Additionally, I created a custom retry and dead-letter mechanism to gracefully handle transient API failures and ensure data consistency.

This approach not only solved the timeout issue but also made the system highly scalable and maintainable. We reduced sync time by over 60% and improved overall system reliability. The solution was later adopted for other modules as well.

