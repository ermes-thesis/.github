# Ermes Framework - Thesis Project

This organization gathers all the repositories associated with the thesis project focusing on the development and evaluation of Ermes, a novel framework for stateful serverless computing designed to operate across the edge-cloud continuum.

Built with Go and WebAssembly, Ermes addresses the limitations of traditional, stateless cloud-centric FaaS platforms. It natively integrates state management into the serverless paradigm, utilizing a decentralized, locality-aware scheduling policy that co-locates computation and state to minimize latency in resource-constrained edge environments.

![Architecture diagram](../images/SystemArchitectureComp.svg)

## 📂 Organization Structure

The repositories are divided into logical categories based on their role within the framework to make navigation easier.

### 🏗️ Core Infrastructure
* **[ermes-generic-node](https://github.com/ermes-thesis/ermes-generic-node):** Repository containing the source code to run a standard Ermes Node.
* **[ermes-function-registry](https://github.com/ermes-thesis/ermes-function-registry):** The Function Registry node of the framework, allowing functions to be cataloged and retrieved.
* **[ermes-central-repo](https://github.com/ermes-thesis/ermes-central-repo):** The Group Token Provider node of the Ermes framework, essential for managing permissions and authentication.
* **[ermes-common](https://github.com/ermes-thesis/ermes-common):** Contains the Ermes framework's common code and utilities shared across various nodes.

### 🛠️ Developer Tools & Client
* **[ermes-sdk-go](https://github.com/ermes-thesis/ermes-sdk-go):** The Software Development Kit (SDK) used to develop Go functions compatible with Ermes and its state management API.
* **[ermes-function-template](https://github.com/ermes-thesis/ermes-function-template):** A ready-to-use template for Go functions that integrates the Ermes SDK, providing a quick starting point.
* **[ermes-cli](https://github.com/ermes-thesis/ermes-cli):** The developer Command Line Interface (CLI) used to build and deploy functions and query templates.
* **[ermes-client-library](https://github.com/ermes-thesis/ermes-client-library):** The interface used by client applications to seamlessly interact with the Ermes infrastructure.

### 🚀 Deployment & Research
* **[ermes-deploy](https://github.com/ermes-thesis/ermes-deploy):** Repository containing Ansible playbooks and configuration files needed to deploy and manage the Ermes framework.
* **[ermes-benchmark](https://github.com/ermes-thesis/ermes-benchmark):** This repository contains the comprehensive benchmarking suite developed to test the performance, stress, and scalability of the Ermes Framework under dynamic mobility and high-concurrency scenarios.
<!-- * **[model_solver](https://github.com/ermes-thesis/model_solver):** A C++ repository containing the code to run the solver for the mathematical model presented and discussed in the thesis.-->