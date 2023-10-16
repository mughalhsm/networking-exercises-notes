# Load Balancer Algorithms

Load balancers distribute workloads (data) between different computing services to improve reliability and network performance.
There are different types of load balancing algorithms depending on the distribution of load.
Load balancer algorithms can be divided into two main types:

## Static Algorithms

Static algorithms do not take into account the state of the server. They are simplier and more efficient to implement. 

### Round Robin

Requests are sent to servers in a sequential, round-robin fashion.

### Weighted Round Robin

Requests are sent to servers based on their weight (importance). Servers receive requests in proportion to their weight compared to other servers connected to the same load balancer.

### IP Hash Method

A hashing method is performed on the client's IP address at the load balancer, and the request is then mapped to the same server as before.

### Random Load Balancing Algorithm

Requests are distributed based on a random number generator.

## Dynamic Algorithms

Dynamic algorithms consider the state of the target group (e.g., server) and consider its load. They require communication between these two systems to make decisions about sending requests to the server.

### Least Connection

Requests are sent to the server with the fewest active connections.

### Weighted Least Connection

Similar to the least connection algorithm, but it takes into account the capacity or assigned weight of the server.


![alt text](https://substackcdn.com/image/fetch/w_1272,c_limit,f_webp,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F12dffcce-f231-48cc-915f-d53c0f8bce0c_3735x3573.jpeg)


### Least Response Times

Requests are sent to the server with the shortest average response time.
