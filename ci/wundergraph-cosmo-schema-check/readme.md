---
title: "WunderGraph Cosmo Schema Check"
description: "Check if your Subgraph GraphQL schema is still compatible with the rest of your federated graph."
---

When operating a federated GraphQL API with [WunderGraph Cosmo](https://wundergraph.com), it is crucial to ensure that all subgraphs are compatible with the rest of the graph.
This workflow runs for every pull request which targets the `main` branch. It checks the schema of the subgraph against the composed schema of the federated graph to ensure compatibility. If the schema is incompatible, the pull request will be blocked until the schema is fixed.