# Enterprise-Data-Fabric

An Enterprise Scale Data Fabric that 'blueprints' a NoSQL Storage layer in functionality to support Java, .NET, /REST and ORM mapping to a Multi-tier caching layer that is geographically aware. 

Many enterprise data-usecases fit around what is conventionally called a 'DataLake'. We believe the same functionality can be built by leveraging NoSQL platforms in conjunction with a DataGridLayer (eventing etc) and Apache Spark (+streaming); 

####Target platforms
The solution is being developed with commercial vendors around the following opensource platforms.
* Cassandra
* Couchbase
* Mongodb

####High level non-functional requirements:
* Caching (*): A highly scalable data caching layer: Compute engines cannot afford the chatter or repeated request for data required to build pricing environments. 
* Eventing(*): Data Eventing supports the notion that a consumer can receives notifications that data has changed, or even the data itself.
*	Java/.NET/Restful APIs: Requesting data need to facilitate standardised technology stacks, including language or API convention (*)
*	Security: Use/Role bases access
*	Multi-tenancy: Support multiple schema sets
*	Workload Isolation: Separate different types of processing, querying
*	Geo-locale data gravity: Making data sticky to locations 
*	Multi-site/datacentre data awareness: Making data flow to regions based upon attributes

(*) represent features being developed using the OpenSource DataGridforNoSQL platform.

####Non-core functional requirements:
*	Cloud burst-out – moving data between sites
*	Data-gravity – large scale deployments
*	Multi-site awareness – conflict resolution

#### Usecases
* Hybrid cloud
* Compute-Grid-Nearside caching
* DEV, UAT, PROD environment sharing
* Trade surveillance
* Enterprise-wide-cache
* Trader desktop live view

#### So what does it look like? (End product format)
The format of the solution will map product specific features and functionality to usecases and phases of adoption. For example Couchbase will utlitise platform specific features such as XDR to achieve multi-tenancy between clusters, with Cassandra it may rely a different KeySpace. The adoption roadmap will map onto realworld usecases ranging from single-install, single-team-multi-environment, single-team-mutli-env with Analytics (Workload isolation) and so on. Various workload characteristics particular to to financial services will also be mapped out. For example Continuous Query caching to provide a live view of trader portfolio and streaming market data. 

A final product offering for each DataPlatform is to be made available via docker.

### The goal is to provide enterprise grade, low-latency and scalable access to data that doesn’t crush the storage layer.


