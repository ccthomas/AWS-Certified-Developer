# AWS Foundation Services
- AWS CLI & SDK
- Identify and Access Management (IAM)
- Virtual Private Cloud (VPC)
- Elastic Compute Cloude EC2
- Route 53 DNS

## AWS CLI and SDK
### CLI
[https://aws.amazon.com/cli/](https://aws.amazon.com/cli/)
- Open Source
- Built using AWS SDK for Python (Boto)
- Run commands against the AWS public APIs
- aws-shell
  - Developer preview for AWS Labs
  - Fuzzy Auto-completion for; commands, options, resource identifiers
  - Dynamic in-line documentation 
  - Execution of OS shell commands
  - `pip install aws-shell`

Confiugre Creds. CLI uses programmatic user to execute AWS API.
```bash
aws configure
```

List all AWS commands
```bash
aws help
```

### SDK
[https://aws.amazon.com/tools/](https://aws.amazon.com/tools/) List of SDKs if you scroll down.

[AWS Developer Forums: Discussion Forums](https://forums.aws.amazon.com)

* Long list of AAWS Language SDKs.
* Toolkits for popular IDEs
* Each one is developed independently.
* IAM Programmatic users are used.

## Identify and Access Management (IAM)
Identity (Who are you) Access (What can you do) Management (Administation of...)
* AWS Service Permisions
* Fine-grainded permisions
* Federated Identity
* Multi-factor Auth
* Free
* PCI Compliant
* Replicated Worldwide

### IAM Overview
- Components
  - Users (Identities)
  - Groups (Identities)
    - Groups contain Users
  - Roles (Identities)
  - Policies
  - Identidy Providers

Users
- An Individual entitiy with a defined username

Access Types
- Programmatic Access
- AWS Management Console Access

Policies
- A Set of **Permissions**
  - Effect
  - Action
  - Resource
  - Condition
- Created By
  - Copy of AWS Policy
  - Policy Wizard
  - Self-defined

Groups
- A collection of Users
- Defined by a Group Name
  - Group name can be changed at any time, HOWEVER don't do this, ARN will change
- Have a Policy attached

Roles
- AWS Identity with permissions policies
- Can be assumed by anyone/anything that needs it and with the necessaty permissions granted
- Use
  - Delegate access to users, applications, or services that don't normally have access to your AWS Resource.

Identidy Providers
- Integrate external identity database
- Can assign permission to user that external idP
- OpenID Connect supported
- SAML supported

IAM Methods
- AWS Management Console
- AWS CLI
- AWS SDK
- IAM HTTPs

## Virtual Private Cloud (VPC)
## Elastic Compute Cloude EC2
## Route 53 DNS
