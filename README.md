# System-Design

##  1) Scalabilty
     Ability of a system to grow in both direction i.e increase or decrease. 
     Some deciding factors include API calls , rate of consumption (i.e less than rate of requests) ,
     number of transactions . A scalable architecture should balance the load on        
     all the participating nodes evenly.
               
     Horizontal scaling, or increasing the number of nodes in the cluster, reduces the responsibilities
     of each member node by spreading the load across all (including new nodes).
     It provides additional endpoints for client connection when the load is higher than configured.
     Reasons to scale horizontally include increasing I/O concurrency, reducing the load on existing nodes.
     
     Vertical scaling, or improving the capabilities of a node/server, gives greater capacity to the node but 
     does not decrease the overall load on existing members of the cluster.  That is, the ability for the 
     improved node to handle existing load is increased, but the load itself is unchanged. Reasons to scale 
     vertically include increasing IOPS, increasing CPU/RAM capacity, and increasing disk capacity.
     
     
##  2) Reliabilty
     Reliability is the probability a system will fail in a given period. In simple terms, a distributed system 
     is considered reliable if it keeps delivering its services even when one or several of its software or hardware 
     components fail.
     
     
##  3) Availability
     It is a simple measure of the percentage of time that a system, service, or a machine remains operational
     under normal conditions. An aircraft that can be flown for many hours a month without much downtime can be 
     said to have a high availability. Availability takes into account maintainability, repair time, spares 
     availability, and other logistics considerations. If an aircraft is down for maintenance, it is considered
     not available during that time.
     
###  Reliability Vs. Availability
     If a system is reliable, it is available. However, if it is available, it is not necessarily reliable.
