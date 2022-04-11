## Notes
- template manifests generated with `helm template kube-prometheus-stack prometheus-community/kube-prometheus-stack -f ./values-kube-prometheus-stack.yaml > template/manifests/kube-prometheus-stack-customized.yml`
- civo nodes didn't have the port 9100 available, needed to patch the daemon set and service to use a different port

## TODO
- add alertmanager alerts and receivers
- configure persistent storage
- add authentication middleware annotations for Ingress resources
- add custom grafana dashboards through extra configmaps
- add Hashicorp vault integration to fetch passwords
