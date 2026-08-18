## Welcome to Ballerina Nutcracker 👋

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ballerina-nutcracker/ballerina/main/doc/img/logo-dark.svg" width="300">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ballerina-nutcracker/ballerina/main/doc/img/logo-light.svg" width="300">
  <img alt="Ballerina Nutcracker" src="https://raw.githubusercontent.com/ballerina-nutcracker/ballerina/main/doc/img/logo-light.svg" width="300">
</picture>

**A native interpreter for the Ballerina programming language.**

[![Release](https://img.shields.io/github/v/release/ballerina-nutcracker/ballerina)](https://github.com/ballerina-nutcracker/ballerina/releases)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/ballerina-nutcracker/ballerina/blob/main/LICENSE)

[Website](https://ballerina.io/nutcracker/) &nbsp;·&nbsp;
[Playground](https://play.ballerina.io/) &nbsp;·&nbsp;
[Interpreter](https://github.com/ballerina-nutcracker/ballerina) &nbsp;·&nbsp;
[Language spec](https://github.com/ballerina-platform/ballerina-spec) &nbsp;·&nbsp;
[Community](https://ballerina.io/community/)

</div>

---

[Ballerina](https://ballerina.io) is an open-source, cloud-native programming language optimized for integration, with built-in JSON and XML, first-class services and concurrency, and structural typing. It is developed and supported by [WSO2](https://wso2.com) and the Ballerina community.

**Ballerina Nutcracker** is a Go compiler and interpreter for Ballerina. It compiles source to **BIR** (Ballerina Intermediate Representation) and runs that BIR from one `bal` binary — no separate runtime to start — so it stays small and fast for CLIs, functions, and sidecars.

> [!IMPORTANT]
> Nutcracker is under active development and does not yet support the whole language. For production use, reach for [Ballerina Swan Lake](https://ballerina.io/downloads/) — the official distribution, which supports the full language.

## Architecture

![Ballerina Nutcracker architecture: the bal CLI (new, run, pack, build, push, version) is the entry point. parser/ produces st/; nodebuilder/ produces ast/. semantics/ resolves types; desugar/ and birgen/ lower to BIR. The runtime interprets BIR. Native stdlib uses extern calls; pure-Ballerina modules run as BIR. PAL is platform/pal; palnative is on the host OS and pal_wasm.go on the browser. Central is for package fetch; bal push writes the local repository.](https://raw.githubusercontent.com/ballerina-nutcracker/ballerina/main/doc/img/architecture.png)

How the pieces in this diagram map to source is in [ARCHITECTURE.md](https://github.com/ballerina-nutcracker/ballerina/blob/main/doc/guides/ARCHITECTURE.md).

## Get started

* [Try it in the Playground](https://play.ballerina.io/)
* [Download a release](https://github.com/ballerina-nutcracker/ballerina/releases/latest)
* [Build from source](https://github.com/ballerina-nutcracker/ballerina/blob/main/README.md#getting-started)

## Docs

* [Developing](https://github.com/ballerina-nutcracker/ballerina/blob/main/doc/guides/DEVELOPING.md)
* [Language features](https://github.com/ballerina-nutcracker/ballerina/tree/main/doc/lang)
* [Library features](https://github.com/ballerina-nutcracker/ballerina/tree/main/doc/library)
* [Milestones](https://github.com/ballerina-nutcracker/ballerina/milestones)

## Contribute

Read the [contribution guidelines](https://github.com/ballerina-nutcracker/ballerina/blob/main/CONTRIBUTING.md) and the [code of conduct](https://github.com/ballerina-nutcracker/ballerina/blob/main/CODE_OF_CONDUCT.md). New here? Start with [`good first issue`](https://github.com/ballerina-nutcracker/ballerina/labels/good%20first%20issue).

Playground source is [ballerina-nutcracker/playground](https://github.com/ballerina-nutcracker/playground).

## Report issues

- Interpreter: [ballerina-nutcracker/ballerina](https://github.com/ballerina-nutcracker/ballerina/issues)
- Playground: [ballerina-nutcracker/playground](https://github.com/ballerina-nutcracker/playground/issues)
- Security: email [security@ballerina.io](mailto:security@ballerina.io) — do not open an issue. See the [security policy](https://github.com/ballerina-nutcracker/ballerina/blob/main/SECURITY.md).

## Community

Questions belong in [GitHub Discussions](https://github.com/ballerina-nutcracker/ballerina/discussions) or on [Discord](https://discord.gg/ballerinalang). See [ballerina.io/community](https://ballerina.io/community/) for everything else.

## License

Distributed under the [Apache License 2.0](https://github.com/ballerina-nutcracker/ballerina/blob/main/LICENSE).
