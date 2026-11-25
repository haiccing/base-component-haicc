# replica

Gives a swarm's node its replica in a container, and brings the replica into service.

The node is deployed and started (the how-to `deploy`). Docker is
needed: the replica is an mrepo built from the node's own package, run
in a container.

## Steps

The script, [steps.haicc](steps.haicc): each line as typed after `haicc`, what it answers under it; run with `howto/run`, shown here at info extraction.

## After

Before the node is torn down its replica is removed: the host's
`boot/teardown <position>`, the boot protocol's at an mrepo, does not
know of a replica's container. The machine's `haicc boot/teardown`
removes every container of the install with the rest.

```sh
haicc host haicc swarms/swarm-1/node-1 container/remove
haicc host boot/teardown swarms/swarm-1/node-1
```
