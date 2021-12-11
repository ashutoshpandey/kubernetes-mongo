# Generate base64 username/password from terminal example (cannot store plain text in secret yaml):
echo -n 'xyz' | base64

# Create Secret first
kubectl apply -f mongo-secret.yaml 

# Run mongodb deployment
kubectl apply -f mongo.yaml 



