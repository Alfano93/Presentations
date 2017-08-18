---?image=images/Ceph_Logo.png&size=auto 95%
# Ceph 101
### What it is
### How it works
### And how to set it up
---
### What is Ceph?


 Ceph is a distributed storage system designed for resiliency, flexibility, and scalability.
---
# Resiliency


Ceph is designed to tolerate multi-node failures.
 - Resiliency through replicaiton
 - Copies are stored on different nodes
 - By default, Ceph creates 2 copies of everything
---
# Flexibility


Ceph works on commodity hardware
 - HDD and SSD can live in the same cluster
 - Can be built for capacity, performance, or both
---
# Scalability


Unlike other distributed storage systems (like Swift), there is no upper bound to the number of nodes you can have in a Ceph cluster.
 - Petabyte scale clusters can be built using the same configs as a 100 TB cluster
---
# CRUSH

## The Backbone of Ceph 
---
**C**ontrolled

**R**eplication

**U**nder

**S**calable

**H**ashing
---
Ceph looks at (minimally) three "units" when placing data

- The Pool  |
- The Node  |
- The Drive |
 
