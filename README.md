# spark-on-k8s

We can deploy spark job on k8s with below methods. 
1. Deploy the spark standalone cluster on k8s. 
2. Using spark-submit 
  a. Deploy-mode = Cluster
    => Create the spark container images with your python/java source code  
    => Using Spark-submit create the driver and executor over the pod. 
  b. Deploy-mode = Client
    => Create the spark container image for executor pod
    => Create the spark Driver on the pod OR one of the worker Node.  
3. Using Spark-operator (BETA Version - Not recommanded for production)
