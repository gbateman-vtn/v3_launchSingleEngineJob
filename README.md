# v3_launchSingleEngineJob

https://docs.veritone.com/#/quickstart/jobs/


In aiWARE, the main unit of work is the Job. A Job, in turn, wraps Tasks; and the work for each Task is done by an engine.

Jobs are typically long-running, since there may be multiple Tasks within a Job, each one operating on a potentially large media file. Thus, Jobs operate asynchronously and you should plan on polling the Job to discover its status.

This page gives a quick overview of how Jobs work in aiWARE. We will show examples of how to run a job using the GraphQL API (the "cloud API") as well as the Edge REST API (which is tyically used in on-premise/hosted aiWARE).

The process involves these steps:

Step One: Authorization and Authentication (Get a Token) or use Veritone provided API Key
Step Two: Choose an Engine (sample calls in GitHub repository contain launchSingleEngine job examples)
Step Three: Create the Job
Step Four: Poll for Status
Step Five: Obtain the Results
