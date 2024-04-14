---
title: "fly.io"
description: "You only need a Dockerfile and this workflow ships your application to fly.io"
---

The deployment story of [Fly.io](https://fly.io) is astonishing, and with this workflow, you can deploy your application to the platform with ease. When your application was [initially setup](https://fly.io/docs/speedrun/) on Fly, you can use this workflow to ship your application whenever you have pushed to the `main` branch.

**Important:** Please make sure to remove your app name from your `fly.toml` and instead pass it as a secret to this workflow. This is to ensure that you don't accidentally expose your app name in your repository (which results in an easily guessable URL for your application).
