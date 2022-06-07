# substrate-parachain-template-zombienet2

### Build the image:
Build the docker image:
`docker build -f docker/Dockerfile.zombie -t gcr.io/paid-network-202104/collator:z1template .`

Push the image:
`docker push gcr.io/paid-network-202104/collator:z1template`

Start minikube:
`minikube start`

Run Zombienet tests
```
  export POLKADOT_VERSION=v0.9.22
  export COLLATOR_VERSION=z1template
  zombienet-linux1236 -p kubernetes test zombienet/0001-small-network.feature
```
