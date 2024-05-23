# Awesome Platform Engineering

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)

A curated list of amazingly awesome Platform tools, resources and various shiny things.

- [Awesome Platform Engineering](#awesome-platform-engineering)
  - [Analytics](#analytics)
  - [Application Security](#application-security)
    - [API Fuzzing](#api-fuzzing)
    - [DAST](#dast)
      - [Language \& Framework-specific DAST](#language--framework-specific-dast)
    - [SAST](#sast)
    - [SCA](#sca)
    - [Secrets detection](#secrets-detection)
    - [Supply chain security](#supply-chain-security)
    - [Threat modelling](#threat-modelling)
  - [API Linting](#api-linting)
  - [Artifact signing and attestation](#artifact-signing-and-attestation)
  - [Bug tracking](#bug-tracking)
  - [Chaos engineering](#chaos-engineering)
  - [Chat and ChatOps](#chat-and-chatops)
  - [Cloud cost management](#cloud-cost-management)
  - [Cloud asset inventory](#cloud-asset-inventory)
  - [Continuous deployment](#continuous-deployment)
  - [Continuous integration](#continuous-integration)
  - [Dashboards as code](#dashboards-as-code)
  - [Dependency management](#dependency-management)
    - [Build systems](#build-systems)
  - [Diagrams as code](#diagrams-as-code)
  - [Docker](#docker)
    - [Shell into containers](#shell-into-containers)
  - [Documentation as code](#documentation-as-code)
  - [Endpoint validation](#endpoint-validation)
  - [Git Tools](#git-tools)
    - [Polyrepo operations tools](#polyrepo-operations-tools)
    - [Repository management tools](#repository-management-tools)
    - [Hook management tools](#hook-management-tools)
  - [Identity and access management](#identity-and-access-management)
  - [Infrastructure as code](#infrastructure-as-code)
    - [Infrastructure as code generation](#infrastructure-as-code-generation)
    - [Infrastructure from code](#infrastructure-from-code)
  - [Internal developer platform](#internal-developer-platform)
  - [Kafka](#kafka)
  - [Kubernetes](#kubernetes)
    - [Kubernetes IAM](#kubernetes-iam)
    - [Kubernetes local development](#kubernetes-local-development)
    - [Kubernetes runtime security](#kubernetes-runtime-security)
    - [Kubernetes security posture management](#kubernetes-security-posture-management)
    - [Kubernetes static analysis](#kubernetes-static-analysis)
    - [Kubernetes templating](#kubernetes-templating)
    - [Kubernetes testing](#kubernetes-testing)
  - [Linting](#linting)
    - [Terraform](#terraform)
    - [Regex](#regex)
  - [Observability](#observability)
  - [Platform as a Service](#platform-as-a-service)
  - [Policy as code](#policy-as-code)
  - [Secrets management](#secrets-management)
  - [Service catalogue](#service-catalogue)
  - [Sharing](#sharing)
  - [Status pages](#status-pages)
  - [Testing](#testing)
    - [A/B testing](#ab-testing)
    - [Load, stress \& soak testing](#load-stress--soak-testing)
  - [Usage-based pricing](#usage-based-pricing)

## Analytics

*Product and customer analytic platforms.*

- [June](https://june.so) - Product usage analytics platform
- [Amplitude](https://amplitude.com) -  Product usage analytics platform

## Application Security

### API Fuzzing

*API testing tools that use a fuzzing engine to generate various test inputs and possible request sequences.*

- [OWASP ZAP](https://www.zaproxy.org/) - dynamic security testing and web app scanner
- [Burpsuite](https://portswigger.net/burp) - The enterprise-enabled dynamic web vulnerability scanner
- [Cherrybomb](https://github.com/blst-security/cherrybomb) - CLI tool that helps you avoid undefined user behaviour by validating your API specifications
- [Restler](https://github.com/microsoft/restler-fuzzer) - stateful REST API fuzzing tool for automatically testing cloud services through their REST APIs and finding security and reliability bugs
- [Dredd](https://github.com/apiaryio/dredd) - Language-agnostic HTTP API Testing Tool
- [Schemathesis](https://github.com/schemathesis/schemathesis) - Specification-centric API testing tool for Open API and GraphQL-based applications
- [Snapchange](https://github.com/awslabs/snapchange) - Lightweight fuzzing of a memory snapshot using KVM
- [Onefuzz](https://github.com/microsoft/onefuzz) - A self-hosted Fuzzing-As-A-Service platform
- [OSS-Fuzz](https://github.com/google/oss-fuzz) - continuous fuzzing for open source software

### DAST

*Dynamic application security testing tools.*

- [OWASP ZAP](https://github.com/zaproxy/zaproxy) - automatically find security vulnerabilities in your web applications while you are developing and testing your applications
- [Nikto2](https://github.com/sullo/nikto) - web server scanner
- [Wapiti](https://github.com/wapiti-scanner/wapiti) - Web vulnerability scanner written in Python3
- [Skipfish](https://github.com/spinkham/skipfish) - Web application security scanner created by lcamtuf for google - Unofficial Mirror [Deprecated]
- [Jazzer](https://github.com/CodeIntelligenceTesting/jazzer/) - Coverage-guided, in-process fuzzing for the JVM
- [CI Fuzz](https://www.code-intelligence.com/cli-tool) - CI Fuzz CLI is an open-source solution that lets you run feedback-based fuzz tests from your command line

#### Language & Framework-specific DAST

- [paulveillard/cybersecurity-dynamic-analysis](https://github.com/paulveillard/cybersecurity-dynamic-analysis)
- [analysis-tools-dev/dynamic-analysis](https://github.com/analysis-tools-dev/dynamic-analysis)

### SAST

*Static application security testing tools.*

- [Shisho](https://github.com/flatt-security/shisho) - Lightweight static analyser
- [Purple panda](https://github.com/carlospolop/PurplePanda) - identify privilege escalation paths within and across different clouds
- [opensourcesecurityindex.io](https://opensourcesecurityindex.io/)
- [Privado](https://github.com/Privado-Inc/privado) - Open Source Static Scanning tool to detect data flows in your code, find data security vulnerabilities & generate accurate Play Store Data Safety Report
- [static-analysis](https://github.com/analysis-tools-dev/static-analysis) - A curated list of static analysis (SAST) tools and linters for all programming languages, config files, build tools, and more. The focus is on tools which improve code quality

### SCA

*Software composition analysis tools.*

- [DependencyCheck](https://github.com/jeremylong/DependencyCheck) - software composition analysis utility that detects publicly disclosed vulnerabilities in application dependencies
- [OpenSCA](https://github.com/XmirrorSecurity/OpenSCA-cli) - supports detection of open source component dependencies and vulnerabilities
- [Dependency-track](https://github.com/DependencyTrack/dependency-track) - Dependency-Track is an intelligent Component Analysis platform that allows organizations to identify and reduce risk in the software supply chain
- [OSV scanner](https://github.com/google/osv-scanner) - Dependency vulnerability scanner written in Go which uses the data provided by [https://osv.dev](https://osv.dev)
- [packj](https://github.com/ossillate-inc/packj) - Packj stops ⚡ Solarwinds-, ESLint-, and PyTorch-like attacks by flagging malicious/vulnerable open-source dependencies ("weak links") in your software supply-chain
- [socket.dev](https://socket.dev/) - Socket fights vulnerabilities and provides visibility, defense-in-depth, and proactive supply chain protection for JavaScript and Python dependencies
- [nancy](https://github.com/sonatype-nexus-community/nancy) - A tool to check for vulnerabilities in your Golang dependencies, powered by Sonatype OSS Index
- [deps.dev](https://deps.dev/) - Google project for rating dependencies
- [dep-scan](https://github.com/owasp-dep-scan/dep-scan) - OWASP dep-scan is a next-generation security and risk audit tool based on known vulnerabilities, advisories, and license limitations for project dependencies

### Secrets detection

*Find leaked secrets in your git repositories, container images and filesystems.*

- [Trufflehog](https://github.com/trufflesecurity/trufflehog) - Find leaked credentials
- [Detect-secrets](https://github.com/Yelp/detect-secrets) - Yelp: An enterprise friendly way of detecting and preventing secrets in code
- [Bridgecrew detect-secrets](https://github.com/bridgecrewio/detect-secrets) - Bridgecrew fork of yelp/detect-secrets
- [Gitleaks](https://github.com/zricethezav/gitleaks) - SAST tool for detecting and preventing hardcoded secrets like passwords, api keys, and tokens in git repos
- [git-secrets](https://github.com/awslabs/git-secrets) - AWSLabs tool for detecting secrets in git. No longer maintained
- [ggshield](https://github.com/GitGuardian/ggshield) - GitGuardian secrets detection.
- [SecretScanner](https://github.com/deepfence/SecretScanner) - Deepfence SecretScanner can find unprotected secrets in container images or file systems. Integrated into [ThreatMapper 1.3.0](https://github.com/deepfence/ThreatMapper)
- [DumpsterDiver](https://github.com/securing/DumpsterDiver) - Tool to search secrets in various filetypes. No longer maintained
- [keyscope](https://github.com/SpectralOps/keyscope) - SpectralOps tool for secrets validation
- [leaky-repo](https://github.com/Plazmaz/leaky-repo) - benchmarking repo with secrets in it to test and evaluate detection tools
- [Skyscanner/whispers](https://github.com/Skyscanner/whispers) - Identify hardcoded secrets in static structured text
- [auth0/repo-supervisor](https://github.com/auth0/repo-supervisor) - Scan your code for security misconfiguration, search for passwords and secrets
- [Ocotopii](https://github.com/redhuntlabs/Octopii) - An AI-powered Personal Identifiable Information (PII) scanner
- [secretlint](https://github.com/secretlint/secretlint) - Pluggable linting tool to prevent committing credentials.

### Supply chain security

*Supply chain security tools.*

- [awesome supply chain security](https://github.com/bureado/awesome-software-supply-chain-security)
- [chain-bench](https://github.com/aquasecurity/chain-bench) - open-source tool for auditing your software supply chain stack for security compliance based on a new CISs Software Supply Chain benchmark
- [legitify](https://github.com/Legit-Labs/legitify) - Detect and remediate misconfigurations and security risks across all your GitHub assets
- [steampipe (GitHub compliance mod)](https://github.com/turbot/steampipe-mod-github-compliance)
- [OWASP dependency-check](https://github.com/jeremylong/DependencyCheck) - software composition analysis utility that detects publicly disclosed vulnerabilities in application dependencies
- [harden-runner](https://github.com/step-security/harden-runner)- Security agent for GitHub-hosted runner: block egress traffic & detect code overwrite to prevent breaches
- [scorecard](https://github.com/ossf/scorecard) - OpenSSF Scorecard - Security health metrics for Open Source
- [CVE Prioritizer](https://github.com/TURROKS/CVE_Prioritizer)- Streamline vulnerability patching with CVSS, EPSS, and CISA's Known Exploited Vulnerabilities
- [ossf/allstar](https://github.com/ossf/allstar) - GitHub App to set and enforce security policies
- [OSSGadget](https://github.com/microsoft/OSSGadget/tree/main) - Collection of tools for analyzing open source packages

### Threat modelling

- [Deciduous](https://www.deciduous.app/) - security decision tree generator that serves as a threat modelling tool

## API Linting

- [Vacuum](https://github.com/daveshanley/vacuum) - vacuum is the worlds fastest OpenAPI 3, OpenAPI 2 / Swagger linter and quality analysis tool. Built in go, it tears through API specs faster than you can think. vacuum is compatible with Spectral rulesets and generates compatible reports
- [Spectral](https://github.com/stoplightio/spectral) - A flexible JSON/YAML linter for creating automated style guides, with baked in support for OpenAPI v3.1, v3.0, and v2.0 as well as AsyncAPI v2.x.
- [SwaggerHub](https://swagger.io/tools/swaggerhub/)
- [oasdiff](https://github.com/Tufin/oasdiff) - OpenAPI Diff and Breaking Changes
- [openapi-diff](https://github.com/OpenAPITools/openapi-diff) - Utility for comparing two OpenAPI specifications.
- [openapi-generator](https://github.com/openapitools/openapi-generator)- OpenAPI Generator allows generation of API client libraries (SDK generation), server stubs, documentation and configuration automatically given an OpenAPI Spec (v2, v3)

## Artifact signing and attestation

*Sign, attest and verify artifacts to protect your software supply chain.*

See: [SLSA - Software Attestations](https://slsa.dev/attestation-model)

- [Cosign](https://github.com/sigstore/cosign) - code signing and transparency for containers and binaries
- [grafeas](https://github.com/grafeas/grafeas) - Artifact Metadata API to audit and govern software supply chains
- [in-toto](https://github.com/in-toto/in-toto) -  a framework to protect supply chain integrity
- [notary](https://github.com/notaryproject/notary) - project that allows anyone to have trust over arbitrary collections of data

## Bug tracking

*Bug tracking, triage and remediation tools.*

- [Bugasura](https://bugasura.io/) - AI-powered issue tracker

## Chaos engineering

*The discipline of experimenting on a distributed system in order to build confidence in the system's capability to withstand turbulent conditions in production.*

- [Chaos Toolkit](https://github.com/chaostoolkit) - the Open Source Platform for Chaos Engineering
- [Chaos Monkey](https://github.com/Netflix/chaosmonkey) - a resiliency tool that helps applications tolerate random instance failures
- [Toxiproxy](https://github.com/Shopify/toxiproxy) - simulate network and system conditions for chaos and resiliency testing
- [Pumba](https://github.com/alexei-led/pumba) - chaos testing, network emulation and stress testing tool for containers
- [Litmus](https://litmuschaos.io/ ) - Cloud Native Chaos Engineering platform
- [KubeInvaders](https://kubernetes.io/blog/2020/01/22/kubeinvaders-gamified-chaos-engineering-tool-for-kubernetes/) - Chaotic fun

## Chat and ChatOps

*Chat and ChatOps.*

- [Rocket](https://rocket.chat/) - open source team communication
- [Mattermost](https://mattermost.com/) - messaging platform that enables secure team collaboration
- [Zulip](https://zulipchat.com/) - real-time chat with an email threading model
- [Riot](https://about.riot.im/) - a universal secure chat app entirely under your control
- ChatOps:
  - [CloudBot](https://github.com/CloudBotIRC/CloudBot) - simple, fast, expandable, open-source Python IRC Bot
  - [Hubot](https://hubot.github.com/) - a customizable life embetterment robot
  - [Lita](https://www.lita.io/) - a robot companion for your company's chat room
  - [Botkube](https://github.com/kubeshop/botkube) - chat bot for Kubernetes
  - [Rootly](https://rootly.com/) - Incident management in Slack

## Cloud cost management

*Automated cost management and cost visibility tools that offer deep insight into your cloud expenditure.*

- [Infracost](https://www.infracost.io/) - Predict cost of infrastructure from Terraform code
- [Terracost](https://github.com/cycloidio/terracost) - Cloud cost estimation for Terraform in your CLI
- [Zesty](https://zesty.co/) - Automated cloud cost optimisation
- [Vantage](https://vantage.sh/) - Automated cloud cost optimisation
- [Scalr](https://www.scalr.com/blog/terraform-cost-estimation) - Terraform platform that has cost-optimisation features
- [Finout](https://www.finout.io/) - Cloud cost monitoring platform
- [Opencost](https://github.com/opencost/opencost) - Cross-cloud cost allocation models for Kubernetes workloads
- [Harness Cloud Cost Management](https://harness.io/products/cloud-cost) - Detect and stop cloud cost anomalies as they occur
- [Loft](https://loft.sh/features/sleep-mode-for-namespaces/) - Kubernetes automated cost savings

## Cloud asset inventory

*Cloud asset inventory and Cloud Security Posture Management tools.*

- [Steampipe](https://steampipe.io/) - `# select * from cloud;`
- [Resoto](https://github.com/someengineering/resoto) -  Resoto creates an inventory of your cloud, provides deep visibility, and reacts to changes in your infrastructure
- [Cloudquery](https://www.cloudquery.io/) - Sync cloud assets to any database, transform and visualize
- [Cloudgraph](https://github.com/cloudgraphdev/cli) - The universal GraphQL API and CSPM tool for AWS, Azure, GCP, K8s, and tencent
- [Cloudmapper](https://github.com/duo-labs/cloudmapper) - CloudMapper helps you analyze your AWS environments
- [AWS ClickOps notifier](https://github.com/cloudandthings/terraform-aws-clickops-notifier) - Get notified when users are taking actions in the AWS Console
- [driftctl](https://github.com/snyk/driftctl) - Detect, track and alert on infrastructure drift
- [Scoutsuite](https://github.com/nccgroup/ScoutSuite) - Multi-Cloud Security Auditing Tools
- [prowler](https://github.com/prowler-cloud/prowler) - perform AWS security best practices assessments, audits, incident response, continuous monitoring
- [saw](https://github.com/TylerBrock/saw) - Fast, multi-purpose tool for searching AWS CloudWatch Logs
- [magpie](https://github.com/openraven/magpie) - Magpie is a free, open-source framework and a collection of community developed plugins that can be used to build complete end-to-end security tools such as a CSPM

## Continuous deployment

*Tools that enable declarative continuous deployment aka GitOps.*

- [ArgoCD](https://github.com/argoproj/argo-cd) - Declarative continuous deployment for Kubernetes
- [Flux](https://github.com/fluxcd/flux2) - Open and extensible continuous delivery solution for Kubernetes
- [dagger](https://dagger.io/) - programmable CI/CD engine that runs your pipelines in containers

## Continuous integration

*CI platforms and release management tools.*

- [Spacelift](https://spacelift.io/) - Spacelift is a sophisticated CI/CD platform for Terraform, CloudFormation, Pulumi, and Kubernetes
- [atlantis](https://www.runatlantis.io/) - Terraform Pull Request Automation
- [scalr](https://www.scalr.com/) - Terraform Cloud alternative
- [env0](https://www.env0.com/) - Manage, deploy, scale, and control all your Terraform, Terragrunt, Pulumi, and related frameworks
- [batect](https://github.com/batect/batect) - Build And Testing Environments as Code Tool
- [autorelease](https://github.com/intuit/auto) - Release automation for GitHub
- [cashapp/hermit](https://github.com/cashapp/hermit) - consistent tooling across environments
- [meta/hermit](https://github.com/facebookexperimental/hermit) - hermetically isolated sandboxes to control program execution
- [semantic-release](https://github.com/semantic-release/semantic-release) - Fully automated version management and package publishing
- [release-please](https://github.com/googleapis/release-please) - generate release PRs based on the conventionalcommits.org spec
- [git-cliff](https://github.com/orhun/git-cliff) - A highly customizable Changelog Generator that follows Conventional Commit specifications ⛰️

## Dashboards as code

*Tools that allow you to define and manage your observability dashboards in code.*

- [Grafanalib](https://github.com/weaveworks/grafanalib) - Write Grafana dashboards in Python
- [Grafonnet](https://github.com/grafana/grafonnet-lib) - Jsonnet library for generating Grafana dashboard files
- [Steampipe - AWS Insights Mod](https://hub.steampipe.io/mods/turbot/aws_insights) - Create dashboards and reports for your AWS resources using Steampipe
- [kennel](https://github.com/grosser/kennel) - Datadog monitors/dashboards/slos as code, avoid chaotic management via UI

## Dependency management

*Manage development environments, software dependencies and package versions.*

- [Poetry](https://python-poetry.org/) - Python packaging and dependency management
- [Renovate](https://github.com/renovatebot/renovate) - Universal dependency update tool that fits into your workflows
- [Dependabot](https://github.com/dependabot/dependabot-core) - Automating dependency updates in multiple languages
- [configrd](https://configrd.io/) - Sync configurations such as environment variables, application properties and secrets across build pipelines, services and environments
- [tfenv](https://github.com/tfutils/tfenv) - Terraform version manager based on rbenv
- [asdf](https://github.com/asdf-vm/asdf) - Extendable version manager with support for Ruby, Node.js, Elixir, Erlang & more
- [mise](https://github.com/jdx/mise) - development environment setup tool that manages dev tools, runtimes, envvars and task runners
- [Devbox](https://github.com/jetpack-io/devbox) - command-line tool that lets you easily create isolated shells for development
- [spack](https://github.com/spack/spack) - A flexible package manager that supports multiple versions, configurations, platforms, and compilers
- [Lerna](https://lerna.js.org/) - Lerna is a tool for managing JavaScript projects with multiple packages, built on Yarn
- [chezmoi](https://github.com/twpayne/chezmoi) - Manage your dotfiles across multiple diverse machines, securely
- [knip](https://github.com/webpro/knip) - Find unused files, dependencies and exports in your JavaScript and TypeScript projects

### Build systems

- [Bazel](https://bazel.build/) - Bazel is Google's monorepo-oriented build system
- [buck2](https://github.com/facebook/buck2) - Buck2 is a fast, hermetic, multi-language build system designed by Meta
- [pants](https://github.com/pantsbuild/pants) - a monorepo-oriented build system, used by Twitter, Foursquare and multiple other companies
- [Nx](https://github.com/nrwl/nx) - Nx is a build system with built-in tooling and advanced CI capabilities. It helps you maintain and scale monorepos, both locally and on CI

## Diagrams as code

*Tools that allow you to draw system architecture diagrams in code, allowing you to track and share your diagrams in any SCM.*

- [structurizr](https://structurizr.org/) - Diagrams as code 2.0
- [Brainboard](https://www.brainboard.co/features/from-design-to-code) - Diagrams to Terraform code
- [Pluralith](https://github.com/Pluralith/pluralith-cli) - Terraform to diagrams
- [cdk-dia](https://github.com/pistazie/cdk-dia)- CDK to diagrams
- [cfn-diagram](https://github.com/mhlabs/cfn-diagram) - CFN to diagrams
- [mingrammer/diagrams](https://github.com/mingrammer/diagrams) - Draw diagrams in Python code
- [Mermaid](https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/) - simple diagrams and flowcharts in Markdown
- [ascii flow](https://asciiflow.com/#/) - ASCII editor
- [PlantUML](https://github.com/plantuml/plantuml) - Create diagrams from plaintext language
- [Markmap](https://markmap.js.org/rep) - visualise your Markdown as minimaps
- [Go diagrams](https://github.com/blushft/go-diagrams) - create system diagrams with Go
- [GraphViz](https://dreampuf.github.io/GraphvizOnline) - create system diagrams in DOT language
- [Cloudcraft](https://www.cloudcraft.co/) - Create AWS diagrams from deployed infrastructure
- [Inframap](https://github.com/cycloidio/inframap) - Read your tfstate or HCL to generate a graph specific for each provider

## Docker

*Docker and general container tools.*

- [Dockle](https://github.com/goodwithtech/dockle) - Docker image linting
- [Container-scan](https://github.com/Azure/container-scan) - Dockle + Trivy [Deprecated]
- [HadoLint](https://github.com/hadolint/hadolint) - Dockerfile linter, validate inline bash, written in Haskell
- [docker-bench](https://github.com/docker/docker-bench-security) - checks for dozens of common best-practices
- [aquasecurity/docker-bench](https://github.com/aquasecurity/docker-bench)
- [Dive](https://github.com/wagoodman/dive) - A tool for exploring a docker image, layer contents, and discovering ways to shrink the size of your Docker/OCI image
- [cadvisor](https://github.com/google/cadvisor) - Analyzes resource usage and performance characteristics of running containers
- [Docker-slim](https://github.com/docker-slim/docker-slim) - Don't change anything in your Docker container image and minify it by up to 30x
- [dfimage](https://github.com/LanikSJ/dfimage) - Reverse-engineer a Dockerfile from a Docker image
- [Whaler](https://github.com/P3GLEG/Whaler) - Go program to reverse Docker images into Dockerfiles
- [anchore-engine](https://github.com/anchore/anchore-engine) - A service that analyzes docker images and scans for vulnerabilities
- [grype](https://github.com/anchore/grype) - image vulnerability scanner
- [docker-trim](https://github.com/tzickel/docker-trim) - create a trimmed docker image that contains only parts of the original file system of an existing docker image
- [diffoci](https://github.com/reproducible-containers/diffoci) - diffoci compares Docker and OCI container images for helping reproducible builds

### Shell into containers

- [cdebug](https://github.com/iximiuz/cdebug) - cdebug - a swiss army knife of container debugging
- [docker-opener](https://github.com/artemkaxboy/docker-opener) - Shell-in to any docker container easily
- [debug-ctr](https://github.com/felipecruz91/debug-ctr) - Command-line tool for interactive container troubleshooting
- [docker-debug](https://github.com/zeromake/docker-debug) - troubleshooting running docker containers

## Documentation as code

*Generate documentation automatically from code.*

- [Doxygen](https://doxygen.nl/) - generate docs from annotated C++ code
- [JavaDoc](https://dev.java/learn/javadoc---the-documentation-generator/) - generate docs from Java code
- [terraform docs](https://terraform-docs.io/) - generate docs from Terraform code
- [glow](https://github.com/charmbracelet/glow) -  terminal based markdown reader designed for the CLI
- [runme](https://github.com/stateful/runme) - Execute your runbooks, docs, and READMEs

## Endpoint validation

*Is it up or not?*

- [Goss](https://github.com/aelsabbahy/goss) - quick and easy server validation
- [Prometheus Blackbox exporter](https://github.com/prometheus/blackbox_exporter) - Blackbox prober exporter

## Git Tools

*Tools that can help you do stuff in Git.*

### Polyrepo operations tools

- [git-xargs](https://github.com/gruntwork-io/git-xargs)
- [microplane](https://github.com/Clever/microplane)
- [all-repos](https://github.com/asottile/all-repos)
- [mu-repo](https://github.com/fabioz/mu-repo)
- [multi-gitter](https://github.com/lindell/multi-gitter)

### Repository management tools

- [pull](https://github.com/wei/pull) - Keep your forks up-to-date via automated PRs
- [git-of-theseus](https://github.com/erikbern/git-of-theseus) - Analyze how a Git repo grows over time
- [bash-git-prompt](https://github.com/magicmonty/bash-git-prompt) - An informative and fancy bash prompt for Git users

### Hook management tools

- [pre-commit](http://pre-commit.com/) - a framework for managing and maintaining multi-language pre-commit hooks from Yelp
- [Overcommit](https://github.com/brigade/overcommit/) - an extendable Git hook manager written with Ruby
- [quickhook](https://github.com/dirk/quickhook/) - a fast, Unix'y, opinionated Git hook runner
- [husky](https://github.com/typicode/husky) - Git hooks for Node.js, manage your hooks from your package.json
- [Mookme](https://github.com/Escape-Technologies/mookme) - A simple and easy-to-use, yet powerful and language agnostic git hook for monorepos
- [lint-staged](https://github.com/lint-staged/lint-staged) - run linters on git staged files
- [lefthook](https://github.com/evilmartians/lefthook) - Fast and powerful Git hooks manager for any type of projects

## Identity and access management

*IAM platforms, tools and systems.*

- [Teleport](https://goteleport.com/)
- [IAMAlive](https://github.com/iann0036/iamlive) - Generate an IAM policy from AWS calls using client-side monitoring (CSM) or embedded proxy
- [Ermetic](https://ermetic.com/) - Holistic IAM protection for AWS, Azure and Google Cloud
- [Pike](https://github.com/jamesWoolfenden/pike) - Pike is a tool for determining the permissions or policy required for IAC code
- [AirAM](https://github.com/bridgecrewio/AirIAM) - Least privilege AWS IAM Terraformer
- [IAM Floyd](https://github.com/udondan/iam-floyd) - AWS IAM policy statement generator with fluent interface
- [repokid](https://github.com/Netflix/repokid) -  AWS IAM usage monitor
- [aardvark](https://github.com/Netflix-Skunkworks/aardvark) - Aardvark is a multi-account AWS IAM Access Advisor API (and caching layer)
- [Trailscraper](https://github.com/flosell/trailscraper/) - A command-line tool to get valuable information out of AWS CloudTrail
- [CloudTracker](https://github.com/duo-labs/cloudtracker) - CloudTracker helps you find over-privileged IAM users and roles by comparing CloudTrail logs with current IAM policies
- [Cloudsplaining](https://github.com/salesforce/cloudsplaining) - AWS IAM Security Assessment tool that identifies violations of least privilege and generates a risk-prioritized report
- [Parliament](https://github.com/duo-labs/parliament) - AWS IAM policy linter
- [PMapper](https://github.com/nccgroup/PMapper) - AWS IAM privilege escalation mapping
- [Policy Sentry](https://github.com/salesforce/policy_sentry) - IAM Least Privilege Policy Generator

## Infrastructure as code

- [Terraform](https://github.com/hashicorp/terraform) - Terraform is a tool for building, changing, and versioning infrastructure
- [OpenTofu](https://github.com/opentofu/opentofu) - OSS Terraform fork that lets you declaratively manage your cloud infrastructure
- [AWS CDK](https://github.com/aws/aws-cdk) - The AWS Cloud Development Kit is a framework for defining cloud infrastructure in code
- [Pulumi](https://github.com/pulumi/pulumi) - Infrastructure as Code in any programming language
- [sst](https://github.com/sst/sst) - Build modern full-stack applications on AWS
- [ion](https://github.com/sst/ion) - ❍ — an experimental new engine for SST
- [Sceptre](https://github.com/Sceptre/sceptre) - sceptre is a tool to drive AWS CloudFormation

### Infrastructure as code generation

*Generate infrastucture code from existing manually-created cloud resources.*

- [Former2](https://github.com/iann0036/former2) - generate CloudFormation/Terraform from existing AWS resources
- [Terraformer](https://github.com/GoogleCloudPlatform/terraformer) - CLI tool to generate terraform files from existing infrastructure
- [Terracognita](https://github.com/cycloidio/terracognita) - generates Terraform from existing AWS resources
- [Firefly](https://www.gofirefly.io/pricing) - Cloud asset management solution
- [k2tf](https://github.com/sl1pm4t/k2tf) - Kubernetes YAML to Terraform HCL converter

### Infrastructure from code

*Generate infrastructure code from application code or runtime.*

- [nitric](https://www.github.com/nitrictech/nitric) - multi-language framework for cloud applications with infrastructure from code

## Internal developer platform

*Tools that contribute to an internal developer platform (IDP), a self-service layer of tools, services and processes that supports and accelerates your software development.*

- [Drone](https://www.drone.io/) - self-service Continuous Integration platform
- [Shipa](https://shipa.io/) - modern application delivery platform
- [KubeVela](https://github.com/kubevela/kubevela) - modern application delivery platform
- [Ketch](https://www.theketch.io/) - Kubernetes application delivery platform
- [Humanitec](https://humanitec.com/) - Internal developer platform orchestrator
- [Nais](https://nais.io/) - application delivery platform
- [Garden](https://github.com/garden-io/garden) - simplify Kubernetes delivery
- [Massdriver](https://www.massdriver.cloud/) - visual IDP that enables engineers to deploy production-ready cloud infrastructure and applications in minutes

## Kafka

*Apache Kafka management tools.*

- [burrow](https://github.com/linkedin/Burrow) - Kafka Consumer Lag Checking
- [schema-registry](https://github.com/confluentinc/schema-registry) - Confluent Schema Registry for Kafka
- [topicctl](https://github.com/segmentio/topicctl) - Tool for declarative management of Kafka topics
- [kaf](https://github.com/birdayz/kaf) - Modern CLI for Apache Kafka, written in Go
- [franz-go](https://github.com/twmb/franz-go) - franz-go contains a feature complete, pure Go library for interacting with Kafka from 0.8.0 through 3.6+. Producing, consuming, transacting, administrating, etc.

## Kubernetes

*Kubernetes management tools.*

- [lens](https://github.com/lensapp/lens) - IDE for kubernetes
- [kubestack](https://www.kubestack.com/) - a collection of Terraform modules and a dedicated Terraform provider to maintain both infra and services together
- [Keda](https://keda.sh/) - Event Driven Autoscaler
- [ket](https://github.com/apprenda/kismatic) - Kismatic Enterprise Toolkit: a set of production-ready defaults and best practice tools for creating enterprise-tuned Kubernetes clusters
- [flagger](https://flagger.app/) - Progressive delivery Kubernetes operator (Canary, A/B Testing and Blue/Green deployments)
- [cdk8s](https://github.com/cdk8s-team/cdk8s) - Define Kubernetes native apps and abstractions using object-oriented programming

### Kubernetes IAM

- [Kubiscan](https://github.com/cyberark/KubiScan) - A tool to scan Kubernetes cluster for risky permissions
- [rbac-police](https://github.com/PaloAltoNetworks/rbac-police) - Evaluate the RBAC permissions of Kubernetes identities through policies written in Rego

### Kubernetes local development

- [Oktekto](https://github.com/okteto/okteto) - Develop your applications directly in your Kubernetes Cluster
- [Tilt](https://github.com/tilt-dev/tilt) - Define your dev environment as code. For microservice apps on Kubernetes
- [Garden](https://github.com/garden-io/garden) - Spin up production-like environments for development, testing, and CI on demand
- [Telepresence](https://github.com/telepresenceio/telepresence) - Local development against a remote Kubernetes or OpenShift cluster
- [Skaffold](https://github.com/GoogleContainerTools/skaffold) - Easy and Repeatable Kubernetes Development

### Kubernetes runtime security

- [tracee](https://github.com/aquasecurity/tracee) - Linux Runtime Security and Forensics using eBPF
- [falco](https://github.com/falcosecurity/falco) - Cloud Native Runtime Security
- [kubespy](https://github.com/pulumi/kubespy) - Tools for observing Kubernetes resources in real time, powered by Pulumi
- [inspektor-gadget](https://github.com/inspektor-gadget/inspektor-gadget) - eBPF security inspection tool
- [Mizu](https://github.com/up9inc/mizu/tree/main) - API traffic viewer for Kubernetes enabling you to view all API communication between microservices. Think TCPDump and Wireshark re-invented for Kubernetes

### Kubernetes security posture management

- [pluto](https://github.com/FairwindsOps/pluto) - A cli tool to help discover deprecated apiVersions in Kubernetes
- [kubent](https://github.com/doitintl/kube-no-trouble) - Easily check your clusters for use of deprecated APIs
- [Popeye](https://github.com/derailed/popeye) - A Kubernetes cluster resource sanitizer
- [kube-bench](https://github.com/aquasecurity/kube-bench) - Checks whether Kubernetes is deployed according to security best practices as defined in the CIS Kubernetes Benchmark
- [kube-no-trouble](https://github.com/doitintl/kube-no-trouble) - Easily check your clusters for use of deprecated APIs
- [nova](https://github.com/FairwindsOps/Nova) - Find outdated or deprecated Helm charts running in your cluster
- [hardeneks](https://github.com/aws-samples/hardeneks) - Runs checks to see if an EKS cluster follows EKS Best Practices
- [kbom](https://github.com/ksoclabs/kbom) - SBOM for Kubernetes
- [sealed-secrets](https://github.com/bitnami-labs/sealed-secrets) - A Kubernetes controller and tool for one-way encrypted Secrets
- [external-secrets](https://github.com/external-secrets/external-secrets) - External Secrets Operator reads information from a third-party service like AWS Secrets Manager and automatically injects the values as Kubernetes Secrets
- [namespacehound](https://github.com/wiz-sec-public/namespacehound) - tool for detecting the risk of potential namespace crossing violations in multi-tenant clusters

### Kubernetes static analysis

- [KubeLinter](https://github.com/stackrox/kube-linter) - static analysis tool that checks Kubernetes YAML files and Helm charts
- [Trivy](https://github.com/aquasecurity/trivy) - Find vulnerabilities, misconfigurations, secrets, SBOM in containers, Kubernetes, code repositories, clouds and more
- [Kubescape](https://github.com/kubescape/kubescape) - K8s open-source tool providing a multi-cloud K8s single pane of glass, including risk analysis, security compliance, RBAC visualizer and image vulnerabilities scanning
- [Kubeclarity](https://github.com/openclarity/kubeclarity) - detection and management of Software Bill Of Materials (SBOM) and vulnerabilities of container images and filesystems
- [grype](https://github.com/anchore/grype) - scan container images for CVEs

### Kubernetes templating

- [helm](https://github.com/helm/helm) - The Kubernetes Package Manager
- [kustomize](https://github.com/kubernetes-sigs/kustomize) - Customization of kubernetes YAML configurations
- [ytt](https://github.com/carvel-dev/ytt) - YAML templating tool that works on YAML structure instead of text
- [timoni](https://github.com/stefanprodan/timoni) - Timoni is a package manager for Kubernetes, powered by CUE and inspired by Helm
- [tanka](https://github.com/grafana/tanka) - Flexible, reusable and concise configuration for Kubernetes using Jsonnet
- [kluctl](https://github.com/kluctl/kluctl/) - The missing glue to put together large Kubernetes deployments, composed of multiple smaller parts (Helm/Kustomize/...) in a manageable and unified way

### Kubernetes testing

- [Testkube](https://github.com/kubeshop/testkube) - Kubernetes-native framework for test definition and execution
- [Kuberhealthy](https://github.com/kuberhealthy/kuberhealthy) - A Kubernetes operator for running synthetic checks as pods

## Linting

*Linting tools to ensure high code quality.*

- [megalinter](https://megalinter.io/latest/supported-linters/) - MegaLinter analyzes 50 languages, 22 formats, 21 tooling formats, excessive copy-pastes, spelling mistakes and security issues
- [reviewdog](https://github.com/reviewdog/reviewdog) - Automated code review tool integrated with any code analysis tools regardless of programming language
- [error-prone](https://github.com/google/error-prone) - Catch common Java mistakes as compile-time errors
- [clang-tidy](https://clang.llvm.org/extra/clang-tidy/index.html)- C++ linter
- [metabob](https://metabob.com/) - AI coding assistant that uses a combination of graph-attention networks and generative AI to facilitate code review and quality
- [Danger JS](https://github.com/danger/danger-js) - Danger runs after your CI, automating your team's conventions surrounding code review

### Terraform

- [tflint](https://github.com/terraform-linters/tflint) - Terraform linter
- [tfautomv](https://github.com/padok-team/tfautomv) - Generate Terraform moved blocks automatically for painless refactoring
- [Awesome terraform](https://github.com/shuaibiyy/awesome-terraform) - Definitive list of Terraform tools
- [terraform visual](https://github.com/hieven/terraform-visual) -  beautifies barely readable output from `terraform graph`
- [terrakube](https://terrakube.org) - OSS alternative to Terraform Cloud
- [hatchet](https://hatchet.run/) - OSS alternative to Terraform Cloud
- [OTF](https://github.com/leg100/otf) - OSS alternative to Terraform Cloud
- [digger](https://github.com/diggerhq/digger) - state aware Terraform orchestrator
- [terralist](https://github.com/terralist/terralist) -  Terraform Private Registry for modules and providers manageable from a REST API

### Regex

- [AutoRegex](https://www.autoregex.xyz/) - convert english to regex

## Observability

*Platforms and tools that help provide visibility into modern distributed applications.*

- [vector](https://github.com/vectordotdev/vector) - A high-performance observability data pipeline
- [datadog](https://www.datadoghq.com/) - leading ($$$$) monitoring and security platform
- [kiali](https://github.com/kiali/kiali) - observability for the Istio service mesh
- [cilium](https://github.com/cilium/cilium) - eBPF-based Networking, Security, and Observability
- [thanos](https://github.com/thanos-io/thanos) - Highly available Prometheus setup with long term storage capabilities
- [otelbin](https://github.com/dash0hq/otelbin) - Web-based tool to facilitate OpenTelemetry collector configuration editing and verification

## Platform as a Service

*PaaS offerings that aren't public cloud hyperscalers.*

- [Section](https://www.section.io/) - simple distributed hosting solution that automatically balances traffic across regions (control plane of control planes)
- [Netlify](https://www.netlify.com/) - cloud application platform
- [Heroku](https://www.heroku.com/) - cloud application platform
- [Kamatera](https://www.kamatera.com/) - Create servers and more, in less than 60 seconds
- [Sloppy](https://sloppy.io/en/) - Managed  Docker Hosting - fast, simple and secure
- [Vultr](https://www.vultr.com/apps/docker?ref=7283626) - Deploy Docker Apps in One-Click
- [StackPath](https://www.stackpath.com/) - run your cloud workloads at the edge
- [Otomi](https://otomi.io/) - Self-hosted PaaS for Kubernetes
- [Replicated](https://www.replicated.com/) - Distribution Platform for Customer Controlled Software

## Policy as code

*Declare policies in a high-level programming language so you can version, test and automatically deploy them.*

- [Cyral](https://cyral.com/blog/unlocking-security-as-code-by-using-github-for-managing-cyral-policies/)
- [Kyverno](https://github.com/kyverno/kyverno) - Kubernetes Native Policy Management
- [Datree](https://www.datree.io/) - Policy as code engine for Kubernetes. Enterprise support available
- [Magtape](https://github.com/tmobile/magtape) - Policy as code engine for Kubernetes
- [OPA Gatekeeper](https://github.com/open-policy-agent/gatekeeper) - Gatekeeper is a Policy Controller for Kubernetes
- [Cloud Custodian](https://github.com/cloud-custodian/cloud-custodian) - Rules engine for cloud security, cost optimization, and governance, DSL in yaml for policies to query, filter, and take actions on resources
- [Hashicorp Sentinel](https://www.hashicorp.com/sentinel) - Policy as code framework for HashiCorp Enterprise Products

## Secrets management

*Sensitive credentials and secrets that need to be managed, secured, maintained and rotated using automation.*

- [Sops](https://github.com/mozilla/sops) - simple and flexible tool for managing secrets
- [Vault](https://www.hashicorp.com/products/vault/) - manage secrets and protect sensitive data
- [Keybase](https://keybase.io/) - end-to-end encrypted chat and cloud storage system
- [Vault Secrets Operator](https://github.com/ricoberger/vault-secrets-operator) - create Kubernetes secrets from Vault for a secure GitOps based workflow
- [Git Secret](https://github.com/sobolevn/git-secret) - a bash-tool to store your private data inside a git repository
- [Keyscope](https://github.com/SpectralOps/keyscope) - a key and secret workflow (validation, invalidation, etc.) tool built in Rust
- [Teller](https://github.com/tellerops/teller) - Cloud native secrets management for developers - never leave your command line for secrets
- [sops](https://github.com/mozilla/sops) - Simple and flexible tool for managing secrets
- [deepsecrets](https://github.com/avito-tech/deepsecrets) - Secrets scanner that understands code
- [doppler](https://www.doppler.com/) - Platform for Secrets management
- [chamber](https://github.com/segmentio/chamber) - CLI for managing secrets

## Service catalogue

*Allow developers to manage their software, infrastructure and documentation in one central place.*

- [Backstage](https://backstage.io/) - Backstage is an open platform for building developer portals
- [Cortex](https://www.cortex.io/) - Cortex makes it easy for engineering organisations to gain visibility into their services
- [OpsLevel](https://www.opslevel.com/) - OpsLevel is the developer platform for teams to own, operate, and understand their production infrastructure
- [Clutch](https://clutch.sh/) - An extensible platform for infrastructure management

## Sharing

*A collection of tools to help with sharing knowledge and telling the story in Markdown, AsciiDoc or RestructuredText.*

- [Gitbook](https://github.com/GitbookIO/gitbook) - modern documentation format and toolchain using Git and Markdown
- [Mintlify](https://mintlify.com/) - modern standard for public facing documentation
- [Docusaurus](https://github.com/facebook/docusaurus) - easy to maintain open source documentation websites
- [Docsify](https://github.com/docsifyjs/docsify/) - a magical documentation site generator
- [MkDocs](https://github.com/mkdocs/mkdocs/) - project documentation with Markdown
- [Obsidian](https://obsidian.md/) - markdown knowledge base
- [Typora](https://typora.io/) - Markdown editor
- [Docz](https://github.com/doczjs/docz/tree/new) - Create MDX files showcasing your code and Docz turns them into a live-reloading, production-ready site
- [Antora](https://antora.org/) - The multi-repository documentation site generator for tech writers who write in AsciiDoc
- [tldraw](https://www.tldraw.com/) - draw things quick
- [excalidraw](https://excalidraw.com/) - hand-drawn look and feel diagrams
- [vale](https://github.com/errata-ai/vale) - A markup-aware linter for prose built with speed and extensibility in mind
- [runme](https://github.com/stateful/runme) - Runme is a tool that makes runbooks actually runnable, making it easier to follow step-by-step instructions

## Status pages

*Communication tool that helps you inform your customers or users about outages and scheduled maintenance.*

- [cachet](https://github.com/cachethq/cachet) - The open-source status page system
- [instatus](https://instatus.com/) - Get a beautiful status page in 10 seconds, without paying thousands of dollars!
- [Atlassian Statuspage](https://www.atlassian.com/software/statuspage) - the #1 status and incident communication tool
- [PagerDuty status page](https://status.pagerduty.com/)

## Testing

- [QA Wolf](https://www.qawolf.com/) - QA Wolf gets web apps to 80% automated end-to-end test coverage in weeks, not years

### A/B testing

*Feature flags and two-sample hypothesis testing.*

- [Optimizely](https://www.optimizely.com/) - A/B testing at scale
- [VWO Testing](https://vwo.com/testing/) - A/B testing
- [Split](https://www.split.io/product/feature-flags/) - managed feature flags and rollouts
- [Sitespect](https://www.sitespect.com/testing-and-experimentation/) - A/B testing and site optimisation

### Load, stress & soak testing

*Performance testing tools. Does it run? Does it scale?*

- [k6](https://k6.io/) - cloud-native load tests written in JS
- [Artillery](https://www.artillery.io/) - cloud-scale performance testing
- [Jmeter](https://jmeter.apache.org/) - 20+ years of solid Java testing
- [Gatling](https://github.com/gatling/gatling) - Java based load testing as code. Note: slower than newer alternatives
- [Tsung](https://github.com/processone/tsung) - high-performance benchmark and stress testing tool
- [Locust](https://locust.io/) - modern load testing in Python
- [LoadRunner](https://software.microfocus.com/en-us/products/loadrunner-load-testing/overview) - Load testing tool from Micro Focus
- [TCPCopy](https://github.com/session-replay-tools/tcpcopy) - TCP stream replay tool to support real testing of Internet server applications
- [Siege](https://www.joedog.org/siege-home/) - HTTP load testing and benchmarking utility
- [Wrk](https://github.com/wg/wrk) - Modern HTTP benchmarking tool
- [Web Bench](http://home.tiscali.cz/~cz210552/webbench.html) - Web Bench is very simple tool for benchmarking WWW or proxy servers

## Usage-based pricing

*Tools that help with managing usage-based pricing.*

See: [Use It or Lose It: Why Usage-Based Pricing](https://rosslazer.com/posts/use-it-or-lose-it-p1/)

- [OpenMeter](https://github.com/openmeterio/openmeter) - Usage Metering for AI, DevOps, and Billing. Built for engineers to collect and aggregate millions of events in real-time
- [Amberflo](https://www.amberflo.io/) - Amberflo provides the most advanced and comprehensive platform for building and deploying usage-based pricing
- [Stigg](https://www.stigg.io) - Instantly build any pricing plan, gauge access control, introduce paywalls and customer portals
- [Lago](https://github.com/getlago/lago) - Open Source Metering and Usage Based Billing
- [Ordway](https://ordwaylabs.com/products/usage-based-billing-software/) - Invoice based upon consumption of cloud services
- [Metronome](https://metronome.com/)
- [octane](https://www.getoctane.io/)
- [orb](https://www.withorb.com/)
- [lago](https://www.getlago.com/)
- [chargebee](https://www.chargebee.com/recurring-billing-invoicing/metered-usage-billing/?ref=navbar)
- [moesif](https://www.moesif.com/)
