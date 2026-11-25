# deploy

Deploys a node of a swarm in the host and brings it into service.

The host is deployed and started (the boot component's how-to
`deploy`). A swarm is a node in the host's `main` whose document says
so, `{"kind":"swarm"}`; a node deployed below it is that swarm's, by the
swarm node's name: `swarm-1/node-1`.

## Steps

The script, [steps.haicc](steps.haicc): each line as typed after `haicc`, what it answers under it; run with `howto/run`, shown here at info extraction.

## Then

The node can be given its replica in a container: the how-to `replica`.
