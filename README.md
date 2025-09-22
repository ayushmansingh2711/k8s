1--Pod.yaml  file ----- to create a pod 



2--pv.yaml -- for PersistentVolume    

  command  --kubectl get pv 



3 -- pvc.yaml --  PersistentVolumeClaim

     command -- kubectl get pvc 




3--secrets.yaml  --    kubectl get secrets 

note - secrets name is mycred  and use this into to the pod.yaml with tag --imagePullSecrets:
    - name: mydocker 
 


note1 - kubectl create secret docker-registry mycred \
  --docker-server=https://index.docker.io/v1/ \
  --docker-username=ayush \
  --docker-password=qwerty123   first create the secrets then write it into yaml file 




4 -   for name space 

   ![alt text](<image (1).png>)




   the name space is using in pod.yaml 





5--    service.yaml   --- kubectl get svc


  - -  kubectl describe svc  svcname 

   minikube ip:portnum 


     