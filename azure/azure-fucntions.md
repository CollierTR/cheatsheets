# Azure Functions

## Bindings & Triggers
### Supported Bindings/Triggers
- blob storage
- cosmos db
- Azure SQL
- Dapr (runtime for micro-services)
- Event Grid
- Event Hub
- Http & Webhooks
- IoT Hub
- Kafka
- SendGrid
- Service Bus
- Queue storage
- RabbitMQ
- Notification Hub
- Mobile Apps
- Signal R (.net client side notification sender)
- Table storage (noSQL Key/Value Store)
- Timer/Chron Triggers

### Binding Direction
You can bind in and out. Example:  
Chron Trigger > Function > Blob storage  
Http Trigger > Function > SendGrid  
Queue storage > Function > Queue storage  

## Local Setting File - local.settings.json
> [!NOTE]
> This should be included in the .gitignore file

## Azure Functions Core Tools
```func init``` Creates a new Function project in a specific language  
```func new``` Creates a new Function in the current project based on a template  
```func logs``` Get logs for Funcs running in Kubernettes Clusters  
```func start``` Starts the local runtime for the function  
```func run``` Runs the function directly  
> [!NOTE]
> This only work with version 1
```func azure``` working with Azure resources including Functions  
```func templates``` for listing available function templates  

## Custom Handlers
light weight web server that receive events from the Functions host  
This is a way to use any language that supports https protocols  
> [!NOTE]
> this just sounds like a regular function but in a language of your choice

