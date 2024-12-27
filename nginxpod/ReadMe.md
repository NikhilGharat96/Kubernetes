Pod :  A Pod is the smallest and most basic deployable unit in Kubernetes. 
       It represents a single instance of a running process in your cluster.
       Pods encapsulate one or more containers, their storage resources, a unique network identity,
       and options for managing how the containers should run.

*************  Commands to Apply This Configuration  ******************

1. Save the YAML configuration to a file, e.g., nginxpod.yml

2. Apply the configuration to your Kubernetes cluster :
       command :-  kubectl apply -f nginxpod.yml

3. Verify that the Pod has been created :
       command :-  kubectl get pods

4. Check the details of the Pod :
       command :-  kubectl describe pod nginxpod             # nginxpod is the name of your pod which is you give in yml file.

5. To access the logs of the container :
       commands :- kubectl logs nginxpod

6. To delete the pod :
        command :-  kubectl delete pod nginxpod