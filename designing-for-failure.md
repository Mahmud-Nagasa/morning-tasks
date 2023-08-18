# Designing for failure

Identify the kinds of failure readiness described below, giving your reasoning;

- A system that switches to a new server when one fails
this is known as failover tolerant, when a server fails it switch to another one that has copy of the data

- Adding replica databases with a master database
this process is known as redundancy, which creating several copies of critical data, to avoid single point of failure 

- Having a 2-3 colleagues who have access to the master password
this is also considered redundancy. however in this case it avoid human single point of  failure, ensuring continuity, helps spot human error and correct them

- Performing health checks on a server
known as monitoring which is to preform a regular check on the system to spot failure  before it happens or respond to it as soon as possible 

- Spreading out user requests over multiple machines rather than just one powerful one
this is called load balancing, to spread the request over several services helps improve the performance, availability, and scalability of a system