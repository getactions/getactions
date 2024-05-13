---
title: "Kubernetes"
description: "Deploy your application to Kubernetes securely."
new: true
---

This workflow helps you securely deploy your application to a Kubernetes cluster. Instead of using your `~/.kube/config`, it relies on a service account that's bound to a cluster role, allowing the deployment under a specific user with fine-grained permissions.

If you're not sure how to set up a service account on Kubernetes and properly link it to the correct role, no worries. Simply check out [this article](https://andrekoenig.de/articles/kubernetes-deployment-using-github-actions), and you'll be good to go.
