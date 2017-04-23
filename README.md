# cloud-head-to-head

## Purpose
To outline the different feature offerings between the 3 major cloud providers


## Azure Functions vs AWS Lambda vs Google Cloud Functions

Feature         | Azure Functions      |      AWS Lambda      
--------------------------| ---------------------|----------------------
Supported Languages       | C#, F#, Node.js, Python, PHP, batch, bash | Node.js, Python, and Java
Pricing Model | Consumption or using existing compute resources
Support Package Managers | NuGet and NPM | ????
Integrated security | OAuth providers such as Azure Active Directory, Facebook, Google, Twitter, and Microsoft Account. | ????
Development environment | Online portal, CI from GitHub/VSTS | ????
Versioning | No | Yes  
Underlying Infrastructure | Azure Webjobs  | ????
Open Source ? | Open Source | Closed Source
Available via HTTP Endpoint | Yes | No
Time Limit | 5 min for Consumption or ?? for 'Classic' | 5 min


### Template Solutions

##### Azure 

- Functions provides templates to get you started with key scenarios, including the following:
- BlobTrigger - Process Azure Storage blobs when they are added to containers. You might use this function for image resizing.
- EventHubTrigger - Respond to events delivered to an Azure Event Hub. Particularly useful in application instrumentation, user experience or workflow processing, and Internet of Things (IoT) scenarios.
- Generic webhook - Process webhook HTTP requests from any service that supports webhooks.
- GitHub webhook - Respond to events that occur in your GitHub repositories. For an example, see Create a webhook or API function.
- HTTPTrigger - Trigger the execution of your code by using an HTTP request.
- QueueTrigger - Respond to messages as they arrive in an Azure Storage queue. For an example, see Create an Azure Function that binds to an Azure service.
- ServiceBusQueueTrigger - Connect your code to other Azure services or on-premises services by listening to message queues.
- ServiceBusTopicTrigger - Connect your code to other Azure services or on-premises services by subscribing to topics.
- TimerTrigger - Execute cleanup or other batch tasks on a predefined schedule. For an example, see Create an event processing function.


### Integrations

##### Azure 

- Azure DocumentDB
- Azure Event Hubs
- Azure Mobile Apps (tables)
- Azure Notification Hubs
- Azure Service Bus (queues and topics)
- Azure Storage (blob, queues, and tables)
- GitHub (webhooks)
- On-premises (using Service Bus)
- Twilio (SMS messages)

### Architectural Differences

'Lambdas are organizationally independently, where Azure Functions are grouped logically into an “application.”'
- serifandsemaphore.io

'Lambdas provision a brand new one and deploys your code (from a zip file) on a cold request. Subsequent requests can be subject to container re-use and be handled much faster. However, you need to understand there is no persistence and with Node.js Lambdas you need to watch your variable scope because the container can be re-used.
However, Azure Functions are less subject to the cold/warm request effects. Azure still provisions resources as needed, but your files aren’t “frozen” somewhere in a zip file. They run on top of Azure’s WebJobs.'
- serifandsemaphore.io


## Other Considerations

- If you use MSDN for all your devs, each subscription comes with an amount of Azure which is going to save you costs

## Microsoft

### Pros

- stronger story for hybrid cloud (cwuk)
  Works well with Active Directory and System Centre
- stronger story for PAAS (cwuk)


## AWS 

### Pros

## References

[An introduction to Azure Functions](https://docs.microsoft.com/en-us/azure/azure-functions/functions-overview)

[Introduction to Microsoft Azure accounts, platform, and services for AWS experts](https://docs.microsoft.com/en-us/azure/architecture/aws-professional/index)

[Choosing a Cloud Platform]( https://aws.amazon.com/choosing-a-cloud-platform/?)

### Pros and Cons

cwuk [Microsoft Azure vs Amazon AWS public cloud comparison: Which cloud is best for the enterprise?](http://www.computerworlduk.com/it-vendors/microsoft-azure-vs-amazon-aws-public-cloud-comparison-which-cloud-is-best-for-enterprise-3624848/3/)

### Feature Comparisons

[Azure Cloud Functions vs. AWS Lambda]
(https://serifandsemaphore.io/azure-cloud-functions-vs-aws-lambda-caf8a90605dd)

[AWS to Azure services comparison](https://docs.microsoft.com/en-us/azure/architecture/aws-professional/services)

[Microsoft Azure vs. Amazon Web Services: Cloud Comparison](http://www.tomsitpro.com/articles/azure-vs-aws-cloud-comparison,2-870-2.html)
