# Kaiburr-Task2
Kubernetes.
For building docker image we need to go with this command - docker build -t your-docker-image-name.<br>
Deploy Local Kubernetes Cluster (using Docker Desktop)<br>
Ensure Docker Desktop is installed and Kubernetes is enabled in Docker Desktop settings.<br>
We need to run this in terminal - <br>kubectl apply -f deployment.yaml<br>
kubectl apply -f service.yaml<br>
After that deploy MongoDB to cluster.<br>
helm repo add bitnami https://charts.bitnami.com/bitnami<br>
helm repo update<br>
<b>Verify Deployment</b><br>
kubectl get service your-application-service.
<br>Ensure that the Helm chart you used for MongoDB (or your custom MongoDB deployment) uses a persistent volume for storing data. This way, data won't be lost when the MongoDB pod is deleted.

With these steps, you should have your Java application and MongoDB running on a local Kubernetes cluster. Adjustments might be needed based on specific details of your application or any custom configurations you have.
