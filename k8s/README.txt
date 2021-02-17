1. Run in cmd as admin - minikube start
    If some errors arise try: minikube stop, minikube delete

2. Look if there is some running deployments
    kubectl get deployments,     kubectl get services

2.1 Store env variables in secret
    // kubectl create secret generic SECRET_NAME --from-literal VARIABLE_KEY=VARIABLE_VALUE
    kubectl create secret generic pgpassword --from-literal PGPASSWORD=pgpassword

3. kubectl apply -f k8s ////// to use all config files from k8s directory in a project

4. Check //// kubectl get deployments, kubectl get pods, kubectl get services