# Enterprise-Data-Fabric

An Enterprise Scale Data Fabric that 'blueprints' a NoSQL Storage layer in functionality to support Java, .NET, /REST and ORM mapping to a Multi-tier caching layer that is geographically aware. 

Many enterprise data-usecases fit around what is conventionally called a 'DataLake'. We believe the same functionality can be built by leveraging NoSQL platforms in conjunction with a DataGridLayer (eventing etc) and Apache Spark (+streaming); 

####High level non-functional requirements:
* Caching: A highly scalable data caching layer: Compute engines cannot afford the chatter or repeated request for data required to build pricing environments. 
* Eventing: Data Eventing supports the notion that a consumer can receives notifications that data has changed, or even the data itself.
*	Java/.NET/Restful APIs: Requesting data need to facilitate standardised technology stacks, including language or API convention
*	Security: Use/Role bases access
*	Multi-tenancy: Support multiple schema sets
*	Workload Isolation: Separate different types of processing, querying
*	Geo-locale data gravity: Making data sticky to locations 
*	Multi-site/datacentre data awareness: Making data flow to regions based upon attributes

####Non-core functional requirements:
*	Cloud burst-out – moving data between site
*	Data-gravity – large scale deployments
*	Multi-site awareness – conflict resolution



### The goal is to provide enterprise grade, low-latency and scalable access to data that doesn’t crush the storage layer.


