# To setup taints
kubectl taint nodes my-kind-cluster-worker app=blue:NoSchedule

# To verify it
kubectl describe node my-kind-cluster-worker |grep -i taint
Taints:             app=blue:NoSchedule

