# 1. Generate base64 username/password from terminal example (cannot store plain text in secret yaml):
echo -n 'xyz' | base64

# 2. Create Secret first
kubectl apply -f mongo-secret.yaml 

  # Check
  kubectl get secret

# 3. Run mongodb deployment
kubectl apply -f mongo.yaml 

  # Check
  kubectl get deployment


# 4. Run mongo-express configmap
kubectl apply -f mongo-configmap.yaml 

  # Check
  kubectl get configmap

# 5. Run mongo-express deployment
kubectl apply -f mongo-express.yaml 

  # Check
  kubectl get deployment
