<p align="center">
  <a href="https://getactions.dev">
    <img alt="getactions.dev logo" src="https://res.cloudinary.com/drfaodoe5/image/upload/v1712678223/logo-getactions.dev.png" width="60" />
  </a>
</p>
<h1 align="center">
  getactions.dev
</h1>

<h3 align="center">
  Start with GitHub Actions easily.
</h3>
<p align="center">
  <a href="https://getactions.dev">getactions.dev</a> helps you kickstarting your projects with pre-defined starter workflows for GitHub Actions.
</p>

<h3 align="center">
 🤖 🚀
</h3>

<img alt="screenshot of the getactions.dev app" src="https://res.cloudinary.com/drfaodoe5/image/upload/v1712677753/getactions.dev.png" />

<br>

<br /><br />

## ✨ Features

### Turnkey GitHub Actions workflows 

Tired of wasting hours configuring your GitHub Actions workflows? We provide a catalog of starter workflows to kick-start your GitHub Actions journey.

### Easily installable

There is no need to copy and paste workflow definitions files anymore. Just run one command to install your workflow into your project. The installation process guides you through the configuration of variables within the workflow and guides you through which secrets need to be configured in your repository.

The best? You don't have to install any tools on your system.

### Community-driven

[getactions.dev's](https://getactions.dev) aim is to grow an extensive catalog of starter workflows for GitHub Actions. Therefore, contributions are highly appreciated. Are you missing a workflow but want to help out by contributing it? Superb! We're super curious to review and merge it!

<br /><br />

## 🚀 Usage

On [getactions.dev](https://getactions.dev), you can find a catalog of ready-to-use GitHub Action starter workflows that can be installed via a simple `cURL` execution. Would you like a taste?

```sh
curl -s https://getactions.dev/deployment/vercel-preview | sh
```

This enables your project to utilize [Vercel Preview Deployments](https://vercel.com/docs/deployments/preview-deployments). This is just one workflow in the `deployment` category. Right now, we maintain the following categories of workflows:

- 🏗️ **Build**: Workflows for building apps, like building a [Go](https://go.dev) project.
- ✅ **Continuous Integration**: Workflows for continuously performing certain tasks, like formatting and linting or performing schema checks when using [GraphQL Federation](https://graphql.com/learn/federated-architecture/) (just to name a few).
- 🛳️ **Deployment**: Workflows for deploying your apps.

<br /><br />

## 🫶 How do I contribute?

In order to contribute a workflow, you have to fork this repository and create a pull request when you're ready.

Let's jump into the interesting part. How to actually write a workflow?

The templates are basically conventional GitHub Action workflows sprinkled with [frontmatter](https://assemble.io/docs/YAML-front-matter.html) on top.

The frontmatter structure is specified and follows a schema specification so that the web application can use it. It consists of:

- `title`: Title of the workflow which gets displayed in the UI.
- `description`: An introduction which gets displayed in the UI.
- `readme`: The readme of the workflow which gets rendered in the detail view of the workflow in the UI.
- `logo`: The name of the logo (which you can find under `./assets/logos` in this repository).
- `secrets`: The repository secret which gets used by this action. The install script summarizes these values after installing the workflow so that the user can easily add the secrets without searching around.
- `parameters`: Values that get asked by the script during installing the workflow. Parameters are useful for asking the user about certain static values (which are not sensitive). The parameters can be referenced in the template by using the `getactions` prefix (e.g. `getactions.MY_PARAMETER`). The install script will ask the user and then substitute the value during rendering the final template.

## Where can I find the sources of the web application?

Glad that you asked! This application is also open source: [getactions/app](https://github.com/getactions/app).

## 📝 License

**getactions** is open-source, licensed as MIT.
