         ___        ______     ____ _                 _  ___  
        / \ \      / / ___|   / ___| | ___  _   _  __| |/ _ \ 
       / _ \ \ /\ / /\___ \  | |   | |/ _ \| | | |/ _` | (_) |
      / ___ \ V  V /  ___) | | |___| | (_) | |_| | (_| |\__, |
     /_/   \_\_/\_/  |____/   \____|_|\___/ \__,_|\__,_|  /_/ 
 ----------------------------------------------------------------- 


+ Source code follow up this link: https://www.eksworkshop.com/010_introduction/
+ Details content:
  - Overview about K8S basics, K8S Architecture, Amazon EKS
  - How to set up and launch EKS 
  - Deploy K8S Dashboard
  - Deploy example microservice application
  - Deploy Helm chart to monitor miltiple Kubernetes
  - Role based access control (RBAC) in K8S

+ Take note:

kubectl proxy --port=8080 --address=0.0.0.0 --disable-filter=true & -> public k8s dashboard via proxy
aws eks get-token --cluster-name eksworkshop-eksctl | jq .  -> get token login dashboard
/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy -> sub uri connect to dashboard