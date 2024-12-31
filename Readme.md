**Project Overview**

Container Image with Python and R
Built a Docker image containing both Python 2, Python 3, and R.
Installed necessary dependencies via requirements.txt for Python packages.
Uploaded the image to Docker Hub. 

Improvements
Security Scan: Scanned the image for vulnerabilities (CVEs) and generated a report. CVEs were addressed by updating packages and using secure base images.
Mitigating Risks: Implemented scanning for malicious packages and followed best practices like using signed images,and updating dependencies regularly.

Kubernetes Deployment and Exposure
Deployed the Docker image in a Kubernetes cluster 
Exposed the deployed service via an external load balancer and made it accessible. 

Automated CI/CD Pipeline
Integrated CI/CD pipeline in the repository, automating the entire process of building, testing, and deploying the containerized application.

Development Environments for Employees
Provided a system for employees to launch customized development environments based on the following:

Base Image Selection.
Package Installation: Users could specify dependencies via values.yml.
Resource Allocation: Specified CPU, memory, and GPU requests in the values.yml

Monitoring and Scaling:
Resource Monitoring: Deployed Prometheus and Horizontal Pod Autoscaler (HPA) to monitor CPU, memory utilization, and scale pods dynamically.
Downscaling and Optimization: Implemented alerts for underutilized resources and auto-downscaling based on set thresholds.
Tracking Usage: Saved data to track resource requests and usage for performance evaluation.

Integrated AWS Route 53 and ExternalDNS to manage DNS routing automatically.





