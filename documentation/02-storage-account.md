# Step 2 – Create an Azure Storage Account

## Objective

The second phase of the project was to deploy an Azure Storage Account to provide secure cloud storage for organizational data. Azure Storage Accounts serve as the foundation for multiple storage services, including Blob Storage, File Shares, Queues, and Tables. For this project, the Storage Account will be used to securely store files while implementing identity-based access controls and cloud security best practices.

---

## Background

Organizations frequently rely on Azure Storage Accounts to store sensitive business data such as financial documents, backups, application data, images, videos, and audit logs. Proper configuration is essential to ensure confidentiality, integrity, and availability while reducing the risk of unauthorized access.

---

## Configuration

| Setting             | Value                             |
| ------------------- | --------------------------------- |
| Subscription        | Azure Subscription 1              |
| Resource Group      | `rg-family-media-dev-1`           |
| Storage Account     | `stfamilymedia8241_1781658961706` |
| Performance         | Standard                          |
| Redundancy          | Locally Redundant Storage (LRS)   |
| Secure Transfer     | Enabled                           |
| Minimum TLS Version | TLS 1.2                           |
| Public Blob Access  | Disabled                          |

---

## Implementation

A new Azure Storage Account was deployed within the project Resource Group using Microsoft's recommended secure default configuration. The account was configured to require encrypted connections and to prevent anonymous public access to Blob Storage.

The Storage Account will serve as the central repository for the remaining project components, including Blob Containers, Microsoft Entra ID integration, and Azure Role-Based Access Control (RBAC).

---

## Security Considerations

The Storage Account was configured with several security best practices:

* Secure transfer (HTTPS) is required for all client connections.
* Public Blob access is disabled to prevent anonymous access.
* TLS 1.2 is enforced to provide modern encryption during data transmission.
* Locally Redundant Storage (LRS) was selected as a cost-effective redundancy option appropriate for a development environment.
* Identity-based access will be managed through Microsoft Entra ID and Azure RBAC rather than shared access keys whenever possible.

---

## Business Justification

A centralized Storage Account provides a secure location for storing organizational data while allowing administrators to apply consistent access controls, monitor activity, and manage permissions from a single location. This approach aligns with the principle of least privilege and supports common cloud governance practices.

---

## Screenshot

The following screenshot shows the deployment of the Azure Storage Account within the project Resource Group.

![Azure Storage Account Deployment](../screenshots/02-storage-account-created.png)

*Figure 2. Azure Storage Account deployment in progress within the project Resource Group.*

---

## Skills Demonstrated

* Microsoft Azure
* Azure Storage Accounts
* Cloud Storage
* Secure Configuration
* Microsoft Entra ID
* Azure RBAC
* Cloud Governance
* Cloud Security
* Identity and Access Management (IAM)

---

## Key Takeaways

Deploying a properly configured Azure Storage Account establishes the foundation for secure cloud storage. By enforcing encrypted communication, disabling anonymous access, and preparing the environment for identity-based authorization, the deployment follows industry best practices for cloud security and governance.
