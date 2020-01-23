# CAP Theorem
     CAP theorem states that it is impossible for a distributed software system to simultaneously provide 
     more than two out of three of the following guarantees (CAP): Consistency, Availability, and Partition
     tolerance. 
     
     
   **Consistency**:  All nodes see the same data at the same time. Consistency is achieved by updating several nodes before        
     allowing further reads.

   **Availability**: Every request gets a response on success/failure. Availability is achieved by replicating the data across     
     different servers.
     
   **Partition tolerance**: System should continue to work even if communication between nodes fails.

## CAP thorem in NOSQL databases :

   CP database: A CP database delivers consistency and partition tolerance at the expense of availability. When a partition 
   occurs between any two nodes, the system has to shut down the non-consistent node (i.e., make it unavailable) until the 
   partition is resolved.

   AP database: An AP database delivers availability and partition tolerance at the expense of consistency. When a partition 
   occurs, all nodes remain available but those at the wrong end of a partition might return an older version of data than 
   others. (When the partition is resolved, the AP databases typically resync the nodes to repair all inconsistencies in the 
   system.)

   CA database: A CA database delivers consistency and availability across all nodes. It can’t do this if there is a partition 
   between any two nodes in the system, however, and therefore can’t deliver fault tolerance.
   
  _In the context of distributed (NoSQL) databases, this means there is always going to be a trade-off between consistency 
   and availability. This is because distributed systems are always necessarily partition tolerant (ie. it simply wouldn’t be    
   a distributed database if it wasn’t partition tolerant.)_
