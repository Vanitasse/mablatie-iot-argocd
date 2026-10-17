# mablatie-iot-argocd

Configuration watched by Argo CD (Inception-of-Things, part 3): the `manifests/`
folder is deployed into the `dev` namespace of the k3d cluster.

Change the application version by editing the image tag in
`manifests/deployment.yaml` (`wil42/playground:v1` or `wil42/playground:v2`),
then commit and push: Argo CD synchronises the cluster.
