# dp [![GoDoc](https://godoc.org/github.com/armen/dp?status.png)](https://godoc.org/github.com/armen/dp) [![Build Status](https://travis-ci.org/armen/dp.svg?branch=master)](https://travis-ci.org/armen/dp) [![codecov](https://codecov.io/gh/armen/dp/branch/master/graph/badge.svg)](https://codecov.io/gh/armen/dp)

A pure Go implementation of [*Introduction to Reliable and Secure Distributed Programming*][dp] abstractions.

## Example Algorithms

- Job handler ([interface and properties](https://godoc.org/github.com/armen/dp/job#Handler))
	- Synchronous job handler ([implementation](https://raw.githubusercontent.com/armen/dp/master/job/handler/sync/sync.go), [algorithm](https://raw.githubusercontent.com/armen/dp/master/job/handler/sync/sync.txt))
	- Asynchronous job handler ([implementation](https://raw.githubusercontent.com/armen/dp/master/job/handler/async/async.go), [algorithm](https://raw.githubusercontent.com/armen/dp/master/job/handler/async/async.txt))
- Job transformation and processing abstraction ([interface and properties](https://godoc.org/github.com/armen/dp/job#TransformationHandler))
	- Job-Transformation by buffering ([implementation](https://raw.githubusercontent.com/armen/dp/master/job/transformation/transformation.go), [algorithm](https://raw.githubusercontent.com/armen/dp/master/job/transformation/transformation.txt))

## List of Algorithms

### Link

- Perfect point-to-point link ([interface and properties](https://godoc.org/github.com/armen/dp/link#Perfect))
	- TCP based perfect peer-to-peer link ([implementation](https://raw.githubusercontent.com/armen/dp/master/link/perfect/p2p/p2p.go))

### Failure Detector

- Perfect failure detector ([interface and properties](https://godoc.org/github.com/armen/dp/fd#Perfect))
- Eventually perfect failure detector ([interface and properties](https://godoc.org/github.com/armen/dp/fd#EventuallyPerfect))

### Broadcast

- Best-Effort broadcast ([interface and properties](https://godoc.org/github.com/armen/dp/broadcast#BestEffort))
	- Basic Broadcast ([implementation](https://raw.githubusercontent.com/armen/dp/master/broadcast/besteffort/beb/beb.go), [algorithm](https://raw.githubusercontent.com/armen/dp/master/broadcast/besteffort/beb/beb.txt))

### Consensus

- Regular Consensus ([interface and properties](https://godoc.org/github.com/armen/dp/consensus#Regular))
- Uniform Consensus ([interface and properties](https://godoc.org/github.com/armen/dp/consensus#Uniform))
	- Single Decree Paxos Proposer ([implementation](https://raw.githubusercontent.com/armen/dp/master/consensus/paxos/basic/proposer.go), [algorithm](https://raw.githubusercontent.com/armen/dp/master/consensus/paxos/basic/proposer.txt))
	- Single Decree Paxos Acceptor ([implementation](https://raw.githubusercontent.com/armen/dp/master/consensus/paxos/basic/acceptor.go), [algorithm](https://raw.githubusercontent.com/armen/dp/master/consensus/paxos/basic/acceptor.txt))

## Notes

WARNING: The API is not stable yet and can change without notice.


[dp]: http://distributedprogramming.net
