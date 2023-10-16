# Load Balancer Algorithms

Load balancer algorithms can be divided into two main types:

## Static Algorithms

Static algorithms do not take into account the state of the target group.

## Dynamic Algorithms

Dynamic algorithms consider the state of the target group (e.g., server). They require communication between these two systems to make decisions about sending requests to the target group.

### Round Robin

Requests are sent to servers in a sequential, round-robin fashion.

### Weighted Round Robin

Requests are sent to servers based on their weight (importance). Servers receive requests in proportion to their weight compared to other servers connected to the same load balancer.

### IP Hash Method

A hashing method is performed on the client's IP address at the load balancer, and the request is then mapped to the same server as before.

### Random Load Balancing Algorithm

Requests are distributed based on a random number generator.

### Least Connection

Requests are sent to the server with the fewest active connections.

### Weighted Least Connection

Similar to the least connection algorithm, but it takes into account the capacity or assigned weight of the server.

### Least Response Times

Requests are sent to the server with the shortest average response time.
