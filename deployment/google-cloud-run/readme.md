---
title: "Google Cloud Run"
description: "Deploy your application to Google Cloud Run directly from source – no Dockerfile required."
---

Imagine you've just built an amazing application, and you want to share it with the world. Your best bet? [Google Cloud Run](https://cloud.google.com/run). The good thing is, you don't have to mess around with creating a Dockerfile. This workflow will directly deploy your application from source.

Before installing this workflow, you have to make sure that the following prerequisites are met on the Google Cloud Platform:

1. Enable the following APIs: the [Artifact Registry API](https://console.cloud.google.com/apis/api/artifactregistry.googleapis.com), the [Cloud Run Admin API](https://console.cloud.google.com/apis/api/run.googleapis.com) and the [Google Build API](https://console.cloud.google.com/apis/api/cloudbuild.googleapis.com).
2. [Create](https://console.cloud.google.com/iam-admin/serviceaccounts/create) a new service account.
3. Assign the following roles to the service account: **Artifact Registry Administrator**, **Cloud Build Editor**, **Cloud Run Admin**, **Service Account User**, **Storage Admin**.
4. Create a new (JSON) key for the service account (make sure to persist it temporarily, as you need it during the installation of the workflow).

The script below will ask you for the required information during the installation.
