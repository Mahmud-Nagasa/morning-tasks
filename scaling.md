# Scaling

In this exercise, you will be given a scenario where some kind of scaling will need to occur to meet demand.
Read through the scenario and give any pros and cons for **both vertical and horizontal** scaling that you can think of, giving examples as to how that specific feature of scaling would positively or negatively affect the infrastructure, the company, or the client.

For example;

Horizontal Scaling:

    Pro
        Cost: This type of scaling can be cheap on demand for short periods of time.

        Scalability: in this type we can add as much devices as required to the meet the demands

        redundancy: using multiple devices can prevent any failure of the system in case a server or two went down, other can keep the system up

    Con
        Data Synchronisation; When dealing with this kind of scaling, it might be difficult to have consistent data across all instances to provide a consistent user experience.

        Maintenance: to keep the servers under check and monitoring regularly is important to ensure that the performance of the system meets the demands, however having several servers will take time and effort.

Vertical Scaling

    Pros
        simplicity: utilising one device can't difficult to implement as it doesn't apply significant changes to the architecture of the system

        Performance: some applications can't be shared between devices and needs to work on  a single instance, which can  be meet by upgrading the resources of that server

        Maintenance: maintaining a single device can be easier and less time consuming compared to Horizontal scaling
        ...

    Cons
        Limited scalability: as there is a limit to how much you can upgrade a device.
   
        Single point of failure: in the situation that the device or server faced an issue or simply not working anymore that will paralyze the system for period of time.

        Usage: in the case of vertical scaling upgrading a device which can be expensive and then just use it for a period of time to meet the demands of a specific event, after which the resources will not be used anymore and we will be have an overpowered server 


        ...

## Scenario

An e-commerce website experiences a sudden surge in traffic due to a flash sale event. The website needs to handle the increased load efficiently to ensure smooth user experience and prevent downtime.

## Extension

What scaling decision would you choose and what steps do you think you might take to achieve the desired infrastructure?

in this situation the demands are temporary for the sale event, hence we just need to handle the traffic for a period of time. Therefore, renting other web servers under a load balancer will solve the issue and after the event is over we can just return these servers and not waste any resources.

in other words using horizontal scaling is the solution I recommend
## More...

If you finish with this one, give one of your mentors a message for another scenario to have a go at
