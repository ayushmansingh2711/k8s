Pod.yaml  file ----- to create a pod 


pv.yaml -- for PersistentVolume    

  command  --kubectl get pv 


secrets.yaml  --    kubectl get secrets 

note - secrets name is mycred  and use this into to the pod.yaml with tag --imagePullSecrets:
    - name: mydocker 
 


note1 - kubectl create secret docker-registry mycred \
  --docker-server=https://index.docker.io/v1/ \
  --docker-username=ayush \
  --docker-password=qwerty123   first create the secrets then write it into yaml file 




   for name space 

   ![alt text](<image (1).png>)




   the name space is using in pod.yaml 



   service.yaml   --- kubectl get svc   

  2 -  kubectl describe svc  svcname 


     