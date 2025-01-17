## General Concepts of SDN Laboratory
### Controller
The SDN Controller is a single point of contact for the applications to provide real-time information about status, configuration and topology for constant optimization and automation of the network. The SDN Controller offers a REST based interface at its northbound interface for external applications to access the resources. The Applications can request the real-time network status and can provide the configurations at the network elements over the standard REST based interface. At the south side, the SDN controller will manage the underlying Network elements through standardized NetConf based requests.

![NorthSouthController](./Images/Capture.PNG)

### Mediators
Mediator for Microwave is a software product which enables SDN (Software Defined Networking) solutions to utilize an installed base of network elements without native NetConf interfaces. It maps NetConf messages based on the ONF YANG information model for microwave equipment to/from the proprietary protocols of the supported network elements.

Mediators are used to send the response towards NetConf YANG interface. An OpenDaylight SDN Controller translates the response from NetConf to RestConf.

### Network Elements (NE)

Network Element, or SDN switch which provides APIs to interact with the SDN controller. Network Elements should be mounted to the controller based on controller basekeys which is used to access resources that retrieve, update/modify data on the Network Element.

### Applications

Currently, the application pattern is building an application layer on SDN controller using the microservice architecture where the complex applications are spilt into small pieces and make them run independently. 


[<- Back to Testing Applications](../../../TestingApplications.md)
