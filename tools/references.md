## Steps to follow
1. https://github.com/knative/serving/blob/main/DEVELOPMENT.md
Use kind.
Don't do Starting Knative Serving yet.

2. Follow https://github.com/knative-sandbox/kn-plugin-quickstart to start knative locally using kind.

3. https://medium.com/@munza/local-kubernetes-with-kind-helm-dashboard-41152e4b3b3d 
Install Kubernetes UI to see things. \
To create the token, use `kubectl create token admin-user -n kubernetes-dashboard` \

4. https://adamtheautomator.com/prometheus-kubernetes/ \
https://knative.dev/docs/serving/observability/metrics/collecting-metrics/#setting-up-prometheus \
To install prometheus into monitoring namespace.

5. Create a sample application with:
`kn service create helloworld-go --image=docker.io/hieungo91/helloworld-go --env TARGET="Go Sample v1"`