# Awesome-Cloud-Native-Application-Protection-Cnapp

# Awesome-Cloud-Native-Application-Protection-Cnapp

**Top Cloud Native Application Protection Cnapp (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on CSPM, CWPP, CIEM, Runtime Security & Attack Path Analysis*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Native Application Protection (CNAPP)**. These tools enable organizations to secure cloud-native workloads across the full lifecycle—from code to runtime—by combining posture management, workload protection, identity entitlements, and attack path analysis into a unified security posture.



**Examples** include Wiz, CrowdStrike Falcon Cloud Security, Palo Alto Prisma Cloud, Orca Security, Microsoft Defender for Cloud, Sysdig Secure, Aqua Security, Lacework, Tenable Cloud Security, and SentinelOne Singularity Cloud (the category leaders in commercial space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosted cloud-native security, runtime protection, and open posture management. **Critical note**: No single open-source project replicates the full CNAPP scope. The landscape is **composable**—you assemble CSPM scanners (Prowler, CloudRec), runtime sensors (Falco, Tetragon, Tracee), IaC scanners (Checkov, Trivy), and policy engines (OPA) into a CNAPP-like stack. **Deepfence ThreatMapper** is the closest single-project approximation, offering CNAPP-style visibility with runtime threat mapping.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

| Platform | Valuation / Company Size | Pricing (Starting Tier) | Free Tier / Trial Limits | Key Capabilities & Best For |
| :--- | :--- | :--- | :--- | :--- |
| **[Microsoft Defender for Cloud](https://azure.microsoft.com/en-us/products/defender-for-cloud)** | ~$3.13T Market Cap ($245B+ revenue) | **$0.0066/server/hr** (~$4.91/server/mo for Plan 1) or **$0.0196/server/hr** (~$14.60/server/mo for Plan 2) | **Free tier available forever** (Foundational CSPM included with Azure: secure score, continuous posture assessments & basic recommendations at no cost); **30-day free trial** per plan for paid Defender for Servers/Containers. | Native Azure CNAPP with CSPM, CWPP, and DevSecOps capabilities. Best for Azure-centric and multi-cloud environments wanting native cloud security. |
| **[Palo Alto Prisma Cloud](https://www.paloaltonetworks.com/prisma/cloud)** | ~$119.4B Market Cap ($8.0B+ revenue) | **~$18,000/year** base CSPM (~2 credits/VM); **~$45,000/year** full CNAPP suite (~5 credits/VM) via AWS Marketplace | **No perpetual free tier**; **15 to 30-day free trial** or structured PoC via AWS Marketplace / direct sales. Underlying cloud compute costs apply during trial. | Comprehensive CNAPP covering code security, CSPM, CWPP, and CIEM with credit-based flexible licensing. |
| **[CrowdStrike Falcon Cloud Security](https://www.crowdstrike.com/)** | ~$76.6B Market Cap ($3.9B+ revenue) | **$0.023/host-hour** (EC2/Workspaces runtime), **$0.054/worker node-hour** (K8s containers), **$0.01/Fargate hour** on AWS Marketplace PAYG | **No perpetual free tier**; **15-day free trial** (covers full Falcon Cloud Security platform evaluation; no credit card required, extensions upon request). | CNAPP deeply integrated with Falcon platform, uniting runtime protection, CWPP, CSPM, and CIEM with endpoint security. |
| **[Lacework](https://www.lacework.com/)** (Fortinet) | ~$72.4B Market Cap ($5.96B Fortinet revenue; acquired for $152.3M) | **~$22,000 to $26,000/year** starter bundles on AWS Marketplace (unit packages based on ~200 cloud asset blocks) | **No perpetual free tier**; **No self-service free trial** (Evaluation access strictly via guided sales engineer Proof of Concept / PoC evaluation license). | Behavioral anomaly detection, automated baseline modeling, and CNAPP capabilities under Fortinet FortiCNAPP suite. |
| **[Wiz](https://www.wiz.io/)** | ~$12B - $32B Valuation ($500M+ ARR) | **$24,000/year** (Wiz Essential tier, min. block of 100 workloads / ~$240/workload/yr) on AWS Marketplace | **No perpetual free tier**; **14-day free trial** (includes initial agentless risk assessment scan and guided PoC). | Unified security graph correlating cloud infrastructure, workloads, identities, and code. Category leader for full-stack agentless posture and risk correlation. |
| **[SentinelOne Singularity Cloud](https://www.sentinelone.com/)** | ~$7.1B Market Cap ($800M+ revenue) | **$36/VM or node/month** (~$432/node/yr) for Cloud Workload Security; Endpoint tiers start from **$60/agent/yr** (Core) | **No perpetual free tier**; **14-day free trial** available via AWS Marketplace / direct proof-of-concept evaluation. | AI-native CNAPP and CWPP offering high-speed kernel-level behavioral prevention, detection, and autonomous remediation. |
| **[Tenable Cloud Security](https://www.tenable.com/)** | ~$4.7B Market Cap ($850M+ revenue) | **~$15,000 to $18,000/year** enterprise starting baseline for cloud resource exposure modules (metered per billable cloud resource) | **No perpetual free tier**; **No self-serve free trial** (requires vendor sales engagement and guided enterprise PoC). | CNAPP with identity-first risk assessment and CIEM depth; maps entitlement graphs and effective permissions across multi-cloud. |
| **[Sysdig Secure](https://sysdig.com/)** | ~$2.5B Valuation ($150M+ ARR) | **$0.13/host-hour** metered rate on AWS Marketplace (or ~$1,500/host/year baseline enterprise commitment packages) | **No perpetual free tier**; **30-day free trial** available on AWS Marketplace and direct SaaS (full CNAPP features enabled; cloud compute costs apply). | CNAPP with runtime insight built on Falco lineage; container-focused detection, drift control, and posture management. |
| **[Orca Security](https://orca.security/)** | ~$1.8B Valuation ($64M+ ARR) | **$7,000/month** (~$84,000/year) entry starter packs on AWS Marketplace covering baseline concurrent cloud workloads | **No perpetual free tier**; **30-day free trial** / complimentary cloud risk assessment available via AWS Marketplace. | Agentless CNAPP with patented SideScanning technology for cloud workload, container, and sensitive data discovery. |
| **[Aqua Security](https://www.aquasec.com/)** | ~$1.0B+ Valuation ($90M+ ARR) | **~$15,000 to $20,000/year** starting enterprise entry tier (metered by workload units, e.g. VMs/nodes/repos) via AWS Marketplace | **No perpetual free tier** (Open-source Trivy scanner is free forever); **14 to 30-day free trial** / proof-of-concept evaluation for the Aqua Enterprise CNAPP platform. | Cloud-native application protection covering container image scanning, supply chain pipeline security, K8s runtime, and CSPM. |

## Open-Source GitHub Projects



- **[Deepfence ThreatMapper](https://github.com/deepfence/ThreatMapper)**

  **Open-source cloud native application protection platform (CNAPP)** (Apache 2.0, ~5,300 stars) — **the closest single-project approximation to a full CNAPP**, with runtime threat mapping and posture visibility. **Features**: **Agentless and agent-based scanning** for hosts, containers, Kubernetes, and serverless; **vulnerability scanning** for images and workloads; **runtime threat detection** via eBPF; **secrets scanning**; **compliance posture** checks; **attack path visualization**—maps how vulnerabilities chain to sensitive data. **Tech stack**: TypeScript, Go, eBPF. **Deploy**: Self-hosted (Docker, Kubernetes). **Trade-off**: **Not a complete CNAPP**—lacks deep CIEM and full code-to-runtime correlation. UI and architecture are heavier than lightweight scanners. **Best for**: teams wanting a single open-source project that covers vulnerability scanning, runtime detection, and attack path visualization—without assembling five separate tools.



- **[Prowler](https://github.com/prowler-cloud/prowler)**

  **Open-source multi-cloud security posture management** (Apache 2.0) — **the most widely adopted open-source CSPM tool**, with **hundreds of checks** across AWS, Azure, GCP, Kubernetes, and Microsoft 365 . **Features**: Checks mapped to **CIS, NIST 800, NIST CSF, PCI-DSS, GDPR, HIPAA, SOC 2, FedRAMP**, and more; scan completes in 5–15 minutes; exports to JSON, CSV, HTML, or AWS Security Hub format; **Prowler App** adds a dashboard and attack-path graph via Cartography for AWS; hosted SaaS version available . **Tech stack**: Python. **Deploy**: Self-hosted (CLI, Docker) or Prowler Cloud. **Trade-off**: **CSPM only**—no runtime detection, workload protection, or CIEM. Findings are lists, not graph-correlated attack paths (except via App integration). **Best for**: security teams wanting production-ready open-source CSPM with broad compliance coverage and CI/CD integration.



- **[Falco](https://github.com/falcosecurity/falco)**

  **Cloud-native runtime security** (Apache 2.0, CNCF graduated) — **the de facto standard for container runtime threat detection**, with the largest community rule library . **Features**: Userspace rule engine reads from kernel module or eBPF probe; detects container escapes (T1611), container deployment (T1610), API discovery (T1613), and more; YAML-based rules; Kubernetes audit log integration. **Tech stack**: C++, Go. **Deploy**: Self-hosted (DaemonSet on Kubernetes). **Trade-off**: **Runtime detection only**—no posture management, vulnerability scanning, or CIEM. Requires tuning and rule maintenance. **Best for**: teams needing runtime threat detection for Kubernetes and containers—the foundation of the runtime layer.



- **[Kubescape](https://github.com/kubescape/kubescape)**

  **Comprehensive Kubernetes security platform** (Apache 2.0, CNCF incubating) — **the most complete open-source Kubernetes security tool**, covering posture, vulnerability, and runtime . **Features**: **Misconfiguration scanning** against NSA-CISA, MITRE ATT&CK, and CIS Benchmarks; **image vulnerability scanning** via Grype; **image patching** via Copacetic; **auto-remediation** of manifest misconfigurations; **admission control** with Validating Admission Policies; **eBPF runtime monitoring** via Inspektor Gadget; **MCP server** for AI assistant integration. **Tech stack**: Go. **Deploy**: Self-hosted (CLI, operator, Helm). **Trade-off**: **Kubernetes-only**—not multi-cloud CSPM or workload protection outside K8s. **Best for**: teams running Kubernetes wanting a single tool for posture, vulnerability, and runtime security within their clusters.



- **[Trivy](https://github.com/aquasecurity/trivy)**

  **Comprehensive open-source scanner** (Apache 2.0) — **the most widely used multi-purpose scanner** for containers, IaC, and SBOMs . **Features**: Vulnerability scanning (OS packages, language dependencies), **IaC misconfiguration detection** (Terraform, CloudFormation, Kubernetes, Dockerfile), **secrets scanning**, **SBOM generation** (CycloneDX, SPDX); CI/CD native. **Tech stack**: Go. **Deploy**: CLI, CI/CD, Docker. **Trade-off**: **Scanner only**—no runtime detection, cloud posture, or CIEM. **Best for**: shift-left security in CI/CD pipelines—the most practical entry point for container and IaC scanning.



- **[OWASP OpenShield](https://github.com/OWASP/openshield)**

  **Open-source CSPM for Azure** (OWASP project) — **the most focused open-source Azure posture scanner** with remediation playbooks . **Features**: Azure misconfiguration scanning; **quantum-unsafe cryptography detection**; compliance mapping to **CIS, NIST, ISO 27001, SOC 2**; **remediation via Azure CLI playbooks**; React security dashboard; **Microsoft Sentinel integration** with KQL rules. **Tech stack**: Python (Flask), React, PostgreSQL, Azure SDK. **Deploy**: Docker or manual (requires Azure credentials). **Trade-off**: **Azure-only**—no AWS or GCP support. Newer OWASP project with limited production validation. **Best for**: Azure-centric organizations wanting an OWASP-backed, self-hosted CSPM with one-command remediation.



- **[CloudRec](https://github.com/antgroup/CloudRec)**

  **Multi-cloud security posture management (CSPM) platform** (Apache 2.0) — **the most mature open-source CSPM with full server deployment and a lightweight Lite edition** . **Features**: **Resource discovery** across 30+ cloud services and 200+ resource types on Alibaba Cloud, AWS, GCP; **OPA-based policy engine** for declarative rules; risk detection across network, identity, data, and logs; **CloudRec Lite** single-binary CLI for local-first checks without server stack. **Tech stack**: Java, Docker. **Deploy**: Full server via Docker Compose; Lite via CLI binary. **Trade-off**: **Alibaba Cloud origin**—strongest support for Alibaba, AWS/GCP less mature. Full deployment requires MySQL and operational overhead. **Best for**: teams running multi-cloud (especially Alibaba/AWS) wanting a self-hosted CSPM with OPA policy flexibility—or CloudRec Lite for quick local posture checks.



### Additional Strong Open-Source Options



- **Tetragon** — eBPF-native runtime security from Isovalent (Apache 2.0). In-kernel enforcement can kill processes before syscalls complete; lower p99 CPU overhead than Falco . **Note**: Runtime only—no posture or vulnerability scanning. **Best for**: teams wanting eBPF-native enforcement alongside Falco's detection.

- **Tracee** — eBPF runtime security from Aqua (Apache 2.0). Built-in signature library plus Rego policy support . **Note**: Runtime only. **Best for**: teams already in Aqua ecosystem wanting eBPF runtime detection.

- **KubeArmor** — LSM-based runtime enforcement (Apache 2.0). AppArmor, SELinux, BPF-LSM enforcement at kernel level . **Note**: Runtime enforcement only. **Best for**: teams needing policy enforcement (not just detection) for container workloads.

- **Checkov** — IaC security scanner (Apache 2.0). 1000+ policies for Terraform, CloudFormation, Kubernetes, Dockerfile . **Note**: Pre-deploy only—no runtime or cloud posture. **Best for**: shift-left IaC security in CI/CD.

- **Steampipe** — SQL-based cloud API querying (AGPL-3.0). Query AWS, Azure, GCP as SQL tables; compliance mods for CIS, SOC 2 . **Note**: Posture and reporting layer only—no runtime, no remediation. **Best for**: teams comfortable with SQL wanting custom posture queries.



**Frameworks for building custom systems**: Combine **Prowler** or **CloudRec** for CSPM, **Falco** or **Tetragon** for runtime detection, **Trivy** or **Checkov** for shift-left scanning, and **Deepfence ThreatMapper** for attack path visualization—creating a composable open-source CNAPP stack. **None of these match Wiz's unified graph or Orca's agentless depth**; those require commercial platforms or significant integration engineering.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- CNAPP platforms handling cloud credentials and security findings must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls for security data.

- **The "unified CNAPP" vs. "CSPM" vs. "runtime security" vs. "scanner" distinction is critical.** **Wiz, CrowdStrike, Prisma Cloud, Orca, Defender for Cloud, Sysdig, Aqua, Lacework, Tenable, and SentinelOne** are **commercial CNAPP platforms**—they bundle CSPM, CWPP, CIEM, and often attack path analysis. **Deepfence ThreatMapper** is the **closest open-source CNAPP**—it covers vulnerability, runtime, and attack paths but lacks full CIEM and code correlation . **Prowler and CloudRec** are **CSPM**—posture only. **Falco, Tetragon, Tracee, and KubeArmor** are **runtime security**—detection or enforcement only. **Trivy and Checkov** are **scanners**—shift-left only. **No single open-source project replaces a commercial CNAPP.** Compose the stack based on your gaps.

- **Deepfence ThreatMapper is the strongest starting point** for teams wanting CNAPP-style visibility from one project—it combines vulnerability scanning, runtime eBPF detection, secrets scanning, and attack path visualization . **The trade-off**: heavier deployment than single-purpose tools; CIEM depth is limited.

- **Prowler is the most production-ready open-source CSPM**—broad compliance coverage, CI/CD integration, and a hosted option for teams wanting a dashboard . **The trade-off**: CSPM only—pair with Falco for runtime and Trivy for shift-left.

- **Falco is the runtime detection standard**—CNCF graduated with the largest rule library . **Tetragon adds in-kernel enforcement**; **KubeArmor adds LSM-based policy enforcement**. Choose based on whether you need detection, enforcement, or both.

- **Kubescape is the most complete Kubernetes-specific tool**—it covers posture, vulnerability, and runtime within K8s clusters . **The trade-off**: Kubernetes-only—not multi-cloud posture or non-K8s workload protection.

- **Pricing opacity is universal across commercial CNAPP vendors.** Wiz, CrowdStrike, Prisma Cloud, Orca, Defender for Cloud (enterprise), Sysdig, Aqua, Lacework, Tenable, and SentinelOne all require sales contact. Prowler offers a hosted SaaS version with usage-based pricing . **Validate with direct vendor conversations against your cloud footprint and workload count.**

- Self-hosted open-source solutions require proper infrastructure (Kubernetes for Falco/Kubescape, databases for CloudRec/Prowler), security hardening for scanner credentials, and ongoing maintenance. **CNAPP tools have privileged access to cloud environments**—ensure your deployment meets your organization's security standards before connecting production accounts.



---



**Made for cloud security engineers, DevSecOps teams, and organizations building transparent CNAPP solutions.**

Let's make Cloud Native Application Protection more open, data-driven, and runtime-aware.
