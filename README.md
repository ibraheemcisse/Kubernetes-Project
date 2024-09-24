<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nginx Deployment with Minikube</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
        }
    </style>
</head>
<body>

<header>
    <h1>Nginx Deployment with Minikube</h1>
    <h2>Overview</h2>
</header>

<p>This repository contains the configuration files and deployment setups for running Nginx on Minikube. The project aims to explore Minikube, port forwarding, and Ingress configurations from scratch.</p>

<h2>Getting Started</h2>

<h3>Requirements</h3>
<ul>
    <li><strong>Minikube:</strong> A running Minikube cluster.</li>
    <li><strong>kubectl:</strong> Command-line tool to interact with Kubernetes.</li>
    <li><strong>Docker:</strong> For building and managing container images.</li>
</ul>

<h3>Setup Instructions</h3>

<h4>Clone the Repository:</h4>
<pre><code>git clone https://github.com/&lt;your-github-username&gt;/nginx-deployment.git</code></pre>
<pre><code>cd nginx-deployment</code></pre>

<h4>Deploy Nginx: Apply the deployment files to your Minikube cluster:</h4>
<pre><code>kubectl apply -f nginx-deployment.yml</code></pre>

<h4>Port Forwarding:</h4>
<p>To access your application locally, set up port forwarding:</p>
<pre><code>kubectl port-forward service/nginx-service 8080:80</code></pre>
<p>This command maps port 8080 on your local machine to port 80 of the Nginx service.</p>

<h4>Check Ingress (if applicable):</h4>
<p>Ensure your Ingress controller is set up and your Ingress resource is properly configured.</p>

<h4>Check Status:</h4>
<p>Verify the status of your pods:</p>
<pre><code>kubectl get pods</code></pre>

<h3>Notes</h3>
<p>Feel free to review the files and provide any feedback or suggestions. Your insights would be greatly appreciated.</p>

</body>
</html>
