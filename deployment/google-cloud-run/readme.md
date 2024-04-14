---
title: "Google Cloud Run"
description: "Deploy your stateless, containerized application on Google Cloud Run."
---

Imagine you've just built an amazing, stateless, containerized application and you want to share it with the world. Your best bet? [Google Cloud Run](https://cloud.google.com/run). With just a `Dockerfile`, you're ready to start your journey

Before installing this workflow, you have to make sure that the following prerequisites are met on the Google Cloud Platform:.

1. Enable the following APIs: the [Artifact Registry API](https://console.cloud.google.com/apis/api/artifactregistry.googleapis.com) and the [Cloud Run Admin API](https://console.cloud.google.com/apis/api/run.googleapis.com).
2. [Create](https://console.cloud.google.com/iam-admin/serviceaccounts/create) a new service account.
3. Assign the following roles to the service account: **Artifact Registry Writer**, **Cloud Run Developer**, **Service Account User**.
4. Create a new (JSON) key for the service account.
5. [Create](https://console.cloud.google.com/artifacts/create-repo) a new repository in the [Artifact Registry](https://cloud.google.com/artifact-registry).

The script below will ask you for the required information during the installation.
