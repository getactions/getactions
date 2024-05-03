---
title: "Run Test Suite"
description: "Installs dependencies and runs tests on the main branch using Composer."
---

This GitHub Actions Workflow is designed to automate the process of installing dependencies and running tests for PHP projects. It triggers on push and pull requests to the `main` branch, validating the `composer.json` and `composer.lock` files, caching [Composer](https://getcomposer.org/) packages for faster build times, installing dependencies using Composer, and executing the test suite.
