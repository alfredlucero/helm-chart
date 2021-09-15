## Some kubectl commands to helm lookup

helm lookup returns an object or array of objects i.e. `(lookup "v1" "Namespace" "" "mynamespace").metadata.annotations`

- kubectl get pod mypod -n mynamespace lookup "v1" "Pod" "mynamespace" "mypod"

- kubectl get pods -n mynamespace lookup "v1" "Pod" "mynamespace" ""

- kubectl get pods --all-namespaces lookup "v1" "Pod" "" ""

- kubectl get namespace mynamespace lookup "v1" "Namespace" "" "mynamespace"

- kubectl get namespaces lookup "v1" "Namespace" "" ""
