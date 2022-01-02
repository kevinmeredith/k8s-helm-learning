1. create cluster via eksctl
1. define YAML for gitlab service account
1. create the service account via `kubectl apply -f ...yaml`
1. get the secret for the service account via `kubectl describe secret ...`
1. update the env vars in gitlab CI/CD 

