# Load Balancing

Can you decide what type of load balancing from the notes might work best for the following situations;

- A chat service where users maintain active connections for a while

in this case the users might occupy a servicer for different periods of time, which will require sticky session with the load balancer (WRR/least connection/ least response time)

- An AI image generation API with paid tiers

 in this situation the service is expected to handle different types of traffic based on each paid tier. therefore, the best choice is to use Weighted Round Robin load balancer, because this approach will distribute the traffic to servers based on their paid tiers or the server capacity


- A social media website that has users all over the world

for users from all over the world it is better use a load balancer type that ensure low latency and availability by directing the data to nearest server based on their location in the world. one such load balancer is source request information that sends request based on information from the source

- An authorisation service that takes the same amount of time for each request

since the request time is the same using a round robin is the best approach as this type evenly distribute requests in  a sequential manner, however one of the down sides of this type that when a request occupy a server for a longer time, in this case the load won't be balanced (consider a WRR in the busy time so that when the requests are a lot WRR can use bigger servers)

- A gaming server that requires low latency

 for gamers having low latency to improve the gaming experience and having a better performance is the main concern. Therefore using a least connection server is the best choice as this type will send requests to the server with the least connection avoiding tha server being overwhelmed with requests maintaining a low latency and smooth gaming experience (maybe least response time/ to reduce lag and lower the latency)