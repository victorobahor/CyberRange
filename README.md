![CyberRange Logo](img/cyberRange_logo_v2.png "Cyber Range")
[![CircleCI](https://circleci.com/gh/secdevops-cuse/CyberRange.svg?style=svg)](https://circleci.com/gh/secdevops-cuse/CyberRange)

# Introduction

CyberRange is an open-source blueprint for creating a Cyber Range on Amazon Web Services (AWS). Its primary purpose is to provide a comprehensive, private, and customizable environment for cybersecurity training, research, penetration testing, defense strategy development, reverse engineering, and security intelligence gathering. 

This project is designed for a wide audience, including penetration testers, security developers, malware analysts, forensic investigators, reverse engineers, threat hunters, students, and professionals interested in advancing their skills in cybersecurity, cloud computing, and DevOps. 

This project represents one of the first open-source Cyber Range blueprints available, offering a unique opportunity to build and explore a state-of-the-art cybersecurity environment.

# Architecture
The CyberRange provides a bootstrap framework for a complete offensive, defensive, reverse engineering, and security intelligence tooling environment within a private research lab deployed on the AWS Cloud. It is designed to be a modular and extensible platform.

![CyberRange Architecture](img/CyberRange-architecture-v2.png)
![Estimated time for setup](img/how-long-does-it-take.png)


# Get Started

This section guides you through setting up your own CyberRange instance.

## Prerequisites

Before you begin, please ensure you have the following:

*   **An AWS Account:** You will need an active Amazon Web Services account to deploy the CyberRange resources.
*   **Access to Project AMIs:** The CyberRange utilizes custom Amazon Machine Images (AMIs). Access to these AMIs is required and can be requested as described in the setup steps below.
*   **(Optional but Recommended) Basic Familiarity:** While not strictly necessary, a basic understanding of AWS services (like EC2, VPC, S3) and [Terraform](https://www.terraform.io/) will be beneficial for advanced customization and troubleshooting.

## Setup Steps

Follow these steps to get your CyberRange operational:

1.  **Obtain AMI Access:**
    To use the CyberRange, you need access to over 30 pre-configured Amazon Machine Images (AMIs). Please request access by submitting your AWS account number via the secure FormAssembly form: [CyberRange Sign-Up Form](https://www.tfaforms.com/4729221). Access will be granted by sharing the AMIs with your account.

2.  **Follow the Detailed Setup Guide:**
    Once AMI access is confirmed, proceed with the comprehensive setup instructions detailed in our [Getting Started Guide](tutorials/getting_started.md). This guide provides step-by-step instructions to configure and deploy the CyberRange environment.

3.  **(Optional) Understand Terraform Setup:**
    The CyberRange infrastructure is provisioned and managed using Terraform. If you wish to understand the underlying infrastructure code, customize the deployment, or contribute to its development, please refer to the [Terraform Setup Guide](terraform/README.md).
<br/>

## Key Features
- **Comprehensive Tooling:** Offers a complete suite for offensive, defensive, reverse engineering, and security intelligence operations.
- **Vulnerable Systems:** Includes a variety of vulnerable systems for hands-on practice and scenario simulation.
- **Powerful Open-Source Toolkit:** Integrates a vast collection of the most effective open-source and community edition tools.
- **AWS Cloud-Based:** Leverages the scalability and flexibility of Amazon Web Services for a customizable lab environment.
- **Automation & Testing:** Features include makefile for build automation and Inspec tests for environment validation.
- **Integrated Labs:** Incorporates DetectionLab for security monitoring and CommandoVM v2 for Windows-based penetration testing.
- **Extensive Toolset:** Pre-configured with numerous tools like Kali Linux (2019.4), Metasploitable 2/3, Nessus, Terraform, Docker, and many more specialized utilities for security assessment and threat analysis.
- **CI/CD Integration:** Uses CircleCI to verify builds and ensure a stable, reliable platform.

## Range History
### Release History
 [See the changelog](changelog.md) for detailed release history.

**v2 (Released: Sept 6, 2019)**
This version brought together a collection of best-in-class and emerging toolsets, creating an integrated solution with significant potential for growth. Key additions and integrated open-source tools include:
- Build & Test: `makefile`, Inspec tests
- Core Environments: CommandoVM v2, Kali Linux 2019.4, DetectionLab integration
- AWS Security & Pentesting Tools:
    - `CyberRange`, `DetectionLab`, `IntruderPayloads`
    - `aws-credential-compromise-detection`, `aws-nuke`, `blast-radius`
    - `cloudgoat`, `cloudmapper`, `packer-windows`, `pacu`
    - `security-monkey-terraform`, `security_monkey`
    - `ScoutSuite`, `prowler`, `pacbot`
    - `terraform-aws-secure-baseline`
    - `my-arsenal-of-aws-security-tools`
- General Pentesting & Utility Tools:
    - `sites-using-cloudflare`, `net-creds`, `Reconnoitre`
    - `shell_generator.sh`, `msploitego`, `awesome-nodejs-pentest`
    - `hammer`, `joomscan`, `learning-tools`, `LetsMapYourNetwork`
    - `php-webshells`, `PowerHub`, `PowerSploit`, `snmpwn`
    - `vulhub`, `gitleaks`

## Technology Stack
CyberRange combines best practices with emerging technologies. Key components include:
- **Cloud Provider:** Amazon Web Services (AWS)
- **Operating Systems:** Kali Linux, Commando-VM (Windows-based penetration testing VM)
- **Vulnerability Scanning:** Nessus
- **Infrastructure as Code:** Terraform
- **Containerization:** Docker, docker-compose
- **Vulnerable Targets:** Open-sourced Vulnerable VMs (e.g., Metasploitable 2/3, various VulnHub VMs) - [See Asset Inventory](asset-inventory.md)
- **CI/CD:** CircleCI for build verification
- **Security & Monitoring:** DetectionLab
- **Configuration Testing:** Inspec
- **And many more tools** for setup, configuration, and experimentation.

## Labs and Tutorials
This project includes a variety of hands-on labs and detailed tutorials to help you get the most out of your CyberRange.
- Explore practical exercises and scenarios in the [labs/](labs/) directory.
- Find setup guides, operational procedures, and other documentation in the [tutorials/](tutorials/) directory.
 
## Learning Domains
This open-source research lab provides a comprehensive learning platform focusing on the intersection of Cyber Security, Cloud Computing, and DevOps. It supports skill development across several broad technical domains:

- Offensive Security
- SecDevOps
- Cloud Architecture & Engineering
- Vulnerability, Change, & Configuration Management
- Quality Assurance & Testing
- Auditing (Processes, Systems, Applications)
- Secure Software Development (Infrastructure & Web Applications)

## Contributing
We welcome contributions to the CyberRange project! If you're interested in helping, please feel free to:
*   Submit issues for bugs or feature requests.
*   Fork the repository and submit pull requests with your proposed changes.

## License
This project is currently not under a specific open-source license. Please contact the project maintainers for more information regarding permissions and usage.

# Mission Statement
 
The ultimate expectation is to emulate the quality, format, and presentation of 
the [Syracuse University Cyber SEED Labs](http://www.cis.syr.edu/~wedu/seed/Labs_16.04/) while 
creating strategic hubs of Cyber Security Center-of-Excellence Partnerships where the gap
between enterprise experience & academic learning is addressed by focusing training paths on 
people, products, and process. 

## 2020 Research Funding
- [AWS Activate](#) - AWS Activate Credits *(Note: Link requires updating by project maintainers)*
- [AWS OpenSource](#) - OpenSource Project Credits *(Note: Link requires updating by project maintainers)*
- CloudCraft License


### Credits
 - Chris Long - For the foundational work on Detection Lab.
 - Omar Santos - For contributions to websploit & docker scripts.
 - FireEye - For developing and open-sourcing CommandoVM & FlareVM.
 - The numerous open-source GitHub projects leveraged within the CyberRange. (Maintainers: Consider linking key projects if feasible).
 - Kali Linux Maintainers - For their continuous work on the Kali Linux distribution.
 - Tenable Nessus Engineers - For the Nessus vulnerability scanner.
 - This project is a fork of [a well-architected terraform AWS framework -> fedekau/terraform-with-circleci-example](https://github.com/fedekau/terraform-with-circleci-example)