---
title: "Kubernetes"
description: "Deploy your application to Kubernetes securely."
new: true
---

This workflow will securely deploy your container image that is hosted on the GitHub Container Registry to your Kubernetes Cluster. Instead of using your `~/.kube/config`, it relies on a Service Account that's bound to a Cluster Role, allowing the deployment under a specific user with fine-grained permissions.

If you're not sure how to set up a Service Account on Kubernetes and properly link it to the correct role, no worries. Simply check out [this article](https://andrekoenig.de/articles/kubernetes-deployment-using-github-actions), and you'll be good to go.
