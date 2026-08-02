# AWS Least-Privilege Compliance Checker - AWS IAM Compliance and Security Analysis 2026

> **Review AWS IAM permissions, exercise CLI-based controls, and generate evidence for least-privilege and compliance programs.**

[![Platform](https://img.shields.io/badge/Platform-AWS-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Latest-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/zack-fosterll5608/aws-least-privilege-checker?style=flat-square)](https://github.com/zack-fosterll5608/aws-least-privilege-checker)

---

<p align="center">
  <a href="https://zack-fosterll5608.github.io/aws-least-privilege-checker/">
    <img src="https://img.shields.io/badge/Download-AWS%20Least--Privilege%20Compliance%20Checker%20Latest-brightgreen?style=for-the-badge" alt="Download AWS Least-Privilege Compliance Checker">
  </a>
</p>

> **[Download AWS Least-Privilege Compliance Checker](https://zack-fosterll5608.github.io/aws-least-privilege-checker/)**

---

[Download Latest Build](https://zack-fosterll5608.github.io/aws-least-privilege-checker/)

---

## Overview

AWS Least-Privilege Compliance Checker gives GRC, cloud security, and engineering teams a single workflow for evaluating IAM users and roles. It combines policy inspection, AWS CLI control checks, effective-permission analysis, and risk-focused findings.

Built for recurring assurance activities, the project can assist with policy-as-code checks and audit evidence gathering. Findings may be exported for review, aligned with programs such as SOC 2, NIST 800-53, and CIS, and followed over time with AWS Config.

---

## Capabilities

- Automatically inspect policies attached to IAM users and roles
- Score risks and group issues for follow-up
- Produce audit evidence as JSON or CSV
- Execute AWS CLI control tests against expected outcomes
- Examine effective access during permission reviews
- Locate unused permissions to support access right-sizing
- Run policy checks within CI workflows
- Enable ongoing observation through AWS Config
- Present results through an interactive dashboard
- Operate as a static single-page application

---

## Getting Started

Retrieve the repository and move into its project directory:

```bash
git clone https://github.com/zack-fosterll5608/aws-least-privilege-checker.git
cd REPO
```

This application is built for static single-page hosting. Run it behind a local web server, or deploy it using the available Pages URL:

```text
https://zack-fosterll5608.github.io/aws-least-privilege-checker/
```

Before performing controls or gathering findings, select an AWS environment whose IAM and analysis permissions meet the needs of the review.

---

## How to Use

The following sequence provides a practical assessment flow:

1. Launch the deployed single-page application.
2. Associate the assessment with the AWS environment under review.
3. Inspect IAM users and roles for policy issues and permission breadth.
4. Execute the AWS CLI control tests and examine their findings.
5. Review effective access and unused rights to identify right-sizing candidates.
6. Export JSON or CSV evidence for compliance and engineering documentation.
7. Run policy validation in CI to assess changes before deployment.
8. Enable AWS Config monitoring when continuing checks are needed.

Use the dashboard for hands-on investigation. Teams can automate recurring checks by adding policy validation and exported evidence to their existing CI and GRC workflows.

---

## Configuration

The exact configuration is determined by how the application is deployed and how reviews are performed. Keep AWS credentials and access information outside the static application, using AWS CLI environment settings, configured profiles, or the environment in which the assessment runs.

Areas commonly configured include:

- AWS account and region
- IAM users and roles selected for review
- Policy validation and control rules
- Thresholds used for risk review
- Locations for JSON and CSV evidence
- CI validation behavior
- AWS Config monitoring boundaries

Never place credentials, access keys, or sensitive AWS account details in the repository.

---

## Requirements

- An AWS account or environment with the IAM resources being assessed
- AWS CLI access to run control tests
- Adequate permissions to inspect the chosen IAM and compliance information
- A current web browser for the interactive dashboard
- A static web server for local execution or static hosting for deployment
- CI integration capability when pipeline-based policy validation is required
- AWS Config availability for continuous monitoring use cases

The amount of storage required varies with the volume of JSON and CSV evidence exported.

---

## Frequently Asked Questions

### Who should use this project?

The tool is suited to cloud security engineers, GRC practitioners, platform engineers, and developers who manage AWS IAM reviews or prepare compliance evidence.

### Does this tool eliminate manual IAM reviews?

No. It supplies analysis, tests, findings, and evidence that complement an organization’s existing review, approval, and governance procedures.

### How can policy changes be checked before release?

Add the policy validation workflow to CI. Proposed changes can then be evaluated before they reach deployment.

### Where does configuration live?

Configuration is supplied by the deployment and execution context. AWS CLI profiles, environment settings, CI variables, and application review options should be maintained in line with the organization’s operational practices.

### What should I check if the tool returns no findings?

Verify the AWS account and region selection, confirm that the AWS CLI session is available, and make sure the reviewing identity can inspect the applicable IAM resources and controls.

### How do I access newer builds?

Open the latest deployed build at [https://zack-fosterll5608.github.io/aws-least-privilege-checker/](https://zack-fosterll5608.github.io/aws-least-privilege-checker/) and review the repository for source changes and deployment updates.

### Can exported results support audit retention?

Yes. Findings and review evidence can be exported in JSON or CSV format and retained according to the organization’s access-control and retention policies.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
