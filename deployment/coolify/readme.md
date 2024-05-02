---
title: "Coolify"
description: "Deploy your application to your Coolify instance"
---

This workflow is designed to streamline the process of containerizing your application and deploying it to your [Coolify](https://coolify.io/) instance. It specifically builds a container image and subsequently publishes it to your [GitHub Container Registry](https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-container-registry). Upon completion of these steps, the workflow initiates a call to the webhook endpoint of your Coolify instance, facilitating the roll out of the newly created image.
