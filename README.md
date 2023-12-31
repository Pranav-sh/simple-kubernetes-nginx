# Simple Kubernetes Nginx Deployment Tutorial

Welcome to the "Simple Kubernetes Nginx Deployment" tutorial! In this guide, you will learn how to deploy a basic Nginx web server using Kubernetes.

## Prerequisites

Before you start, ensure you have the following prerequisites:

- A Kubernetes cluster set up and configured.
- The `kubectl` command-line tool installed and configured.
- Familiarity with YAML syntax.


### 1. Clone the Repository

```
git clone https://github.com/Pranav-sh/simple-kubernetes-nginx.git
cd simple-kubernetes-nginx
```

### Step 2: Apply the Nginx Deployment

1. Open a terminal.
2. Run the following command to apply the Nginx Deployment configuration:
```
kubectl apply -f nginx-one.yaml
```

### 3: Check the Pod Status

1. Open a terminal.
2. Run the following command to check the status of the created pod:

```
kubectl get pod
```

### Step 4: Access the Nginx Welcome Page

 Once the pod is in a 'Running' state, run the following command to obtain its IP address:

```
kubectl get pod -o wide
```


### Step 5: Use `curl` to Access the Nginx Welcome Page

- Replace 'POD_IP_ADDRESS' with the IP address you obtained in the previous step.
-  Run the following command to access the Nginx welcome page:

```
curl http://POD_IP_ADDRESS:80
```
# Conclusion

Congratulations! You've successfully deployed Nginx using Kubernetes and accessed its welcome page. Feel free to explore more Kubernetes concepts and experiment with different configurations.

## Additional Resources

- [Kubernetes Documentation](https://kubernetes.io/docs/)
- [Nginx Documentation](http://nginx.org/)
- [GitHub Repository](https://github.com/Pranav-sh/simple-kubernetes-nginx.git)

## License

This tutorial and its code are provided under the [MIT License](LICENSE).

