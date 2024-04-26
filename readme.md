<p align="center">
  <a href="https://getactions.dev">
    <img alt="getactions.dev logo" src="https://res.cloudinary.com/drfaodoe5/image/upload/v1712678223/logo-getactions.dev.png" width="60" />
  </a>
</p>
<h1 align="center">
  getactions.dev
</h1>

<h3 align="center">
  Easy to-use GitHub Actions Starter Workflows
</h3>
<p align="center">
  <a href="https://getactions.dev">getactions.dev</a> helps you to kick-start your projects with pre-defined starter workflows for GitHub Actions.
</p>

<h3 align="center">
 🤖 🚀
</h3>

<img alt="screenshot of the getactions.dev app" src="https://res.cloudinary.com/drfaodoe5/image/upload/v1712677753/getactions.dev.png" />

<br /><br /><br />

## ✨ Features

### Turnkey GitHub Actions workflows

Are you tired of wasting hours configuring your GitHub Actions workflows? We provide a catalog of starter workflows to kick-start your GitHub Actions journey.

### Easily installable

There is no need to copy and paste workflow definition files anymore. Just run one command to install your workflow into your project. The installation process guides you through the configuration of variables within the workflow and guides you through which secrets need to be configured in your repository.

The best? You don't have to install any tools on your system.

### Community-driven

[getactions.dev's](https://getactions.dev) aim is to grow an extensive catalog of starter workflows for GitHub Actions. Therefore, contributions are highly appreciated. Are you missing a workflow but want to help out by contributing it? Superb! We're super curious to review and merge it!

<br /><br />

## 🚀 Usage

On [getactions.dev](https://getactions.dev), you can find a catalog of ready-to-use GitHub Action starter workflows that can be installed via a simple `cURL` execution. Would you like a taste?

### Example: Installing a Vercel Preview Deployment workflow

```sh
curl -s https://getactions.dev/deployment/vercel-preview | sh
```

This enables your project to utilize [Vercel Preview Deployments](https://vercel.com/docs/deployments/preview-deployments). This is just one workflow in the `deployment` category. Right now, we maintain the following categories of workflows:

- 🏗️ **Build**: Workflows for building apps, like building a [Go](https://go.dev) project.
- ✅ **Continuous Integration**: Workflows for continuously performing certain tasks, like formatting and linting or performing schema checks when using [GraphQL Federation](https://graphql.com/learn/federated-architecture/) (just to name a few).
- 🛳️ **Deployment**: Workflows for deploying your apps.

<br /><br />

## 🫶 How do I contribute?

To contribute a workflow, fork this repository and create a pull request when you're ready.

Let's jump into the interesting part. How to actually write a workflow?

A workflow "package" contains three files:

- `workflow.yaml`: The actual workflow file (sprinkled with [frontmatter](https://assemble.io/docs/YAML-front-matter.html) on top).
- `readme.md`: A readme which describes the workflow.
- `logo.svg` (optional): An icon that represents the workflow. When not defined the GitHub Actions logo will be used.

This package needs to be categorized under one of the main categories. The name of the category + the name of the workflow package directory represent the ID of the workflow.

### The `workflow.yaml`

The actual GitHub Actions workflow. You can specify the following attributes in the frontmatter part of the workflow file:

- `parameters`: An object with parameters. The user will asked for the actual values when installing the script via `curl -s https://getactions.dev/<id> | bash`. You can define the places where the actual value will be placed via `getactions.<NAME_OF_PARAM>`.
- `secrets`: An object with secrets the user has to add to the respective GitHub repository. The installation script will print a table with all the secrets after installing the workflow in the repository. This will help the user easily configure the secrets without switching contexts.

Check the [WunderGraph Cosmo Schema Check](/ci/wundergraph-cosmo-schema-check) workflow to see these two attributes in action.

### The `readme.md`

Describes your workflow. The contents of this file gets displayed on [getactions.dev](https://getactions.dev). The frontmatter attributes are:

- `title`: The title of your workflow.
- `description`: A short description of your workflow.

The actual contents below the frontmatter is for describing your workflow in a detailed way.

### The `logo.svg`

The logo gets displayed on [getactions.dev](https://getactions.dev) as well. Please make sure to remove `width` and `height` attributes from the root element of the SVG.

<br /><br />

## Where can I find the sources of the web application?

Glad that you asked! This application is also open source: [getactions/app](https://github.com/getactions/app).

<br /><br />

## 📝 License

**getactions** is open-source, licensed as MIT.
