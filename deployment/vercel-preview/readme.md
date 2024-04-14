---
title: "Vercel Preview"
description: "This workflow deploys your application to Vercel as a preview deployment"
---

With this workflow you can deploy your application to [Vercel](https://vercel.com) as a [preview deployment](https://vercel.com/docs/deployments/preview-deployments). This is useful when you want to test your application before merging it to your production branch. This workflow gets triggered on all branches except the `main` branch. So whenever you push to your feature branch, this workflow will make sure that a corresponding preview deployment exists afterwards.