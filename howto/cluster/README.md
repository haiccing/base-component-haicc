# cluster

A host with a swarm of two nodes, each with its replica in a container, made by one script.

The host is deployed, in service by its commission. The component's
script `cluster` is then sent to it (`haicc/script`, its lines from the
component's `scripts/cluster.haicc`): `swarms/swarm-1` made, `node-1`
and `node-2` deployed (each in service by its commission) and each given
its running replica (in service by its own), then the swarm's nodes
read. Docker is needed; the containers are left running.

## Steps

The script, [steps.haicc](steps.haicc): each line as typed after `haicc`, what it answers under it; run with `howto/run`, shown here at info extraction.

## Notes

- **Only the host, in service**: its deploy alone.
