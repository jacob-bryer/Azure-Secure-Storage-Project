# Step 9 – Solution Architecture Overview

## Objective

This document provides a high-level overview of the Azure Secure Storage & IAM Project architecture. The solution demonstrates how Microsoft Entra ID, Azure Role-Based Access Control (RBAC), Azure Storage, and Azure Activity Logs work together to provide secure, identity-based access to cloud resources.

---

## Architecture Summary

The solution was designed using Microsoft Azure security best practices. User authentication is managed through Microsoft Entra ID, authorization is enforced using Azure RBAC, and organizational files are securely stored within a private Azure Blob Container. Administrative actions are recorded through Azure Activity Logs to provide auditing and operational visibility.

---

## Components

### Microsoft Entra ID

Provides centralized identity management and user authentication.

### Security Group

Groups users with similar job responsibilities to simplify permission management.

### Azure RBAC

Grants permissions based on roles rather than assigning broad administrative access.

### Azure Storage Account

Provides secure cloud storage for organizational files.

### Private Blob Container

Stores files while preventing anonymous public access.

### Azure Activity Logs

Records administrative actions for auditing, monitoring, and compliance purposes.

---

## Security Architecture

The project follows several cloud security best practices:

* Identity-based authentication using Microsoft Entra ID.
* Group-based authorization through Azure RBAC.
* Principle of Least Privilege.
* Secure communication using HTTPS and TLS 1.2.
* Anonymous Blob access disabled.
* Activity logging enabled for auditing and governance.

---

## Screenshot

The following diagram illustrates the overall architecture of the Azure Secure Storage & IAM Project.

![Azure Architecture Diagram](../architecture/architecture-diagram.png)

*Figure 9. High-level architecture showing authentication, authorization, secure storage, and monitoring components.*

---

## Skills Demonstrated

* Microsoft Azure
* Cloud Architecture
* Microsoft Entra ID
* Azure RBAC
* Azure Storage
* Cloud Security
* Identity and Access Management (IAM)
* Governance, Risk, and Compliance (GRC)

---

## Key Takeaways

This architecture demonstrates a secure, identity-driven cloud storage solution that aligns with Azure security best practices. By combining Microsoft Entra ID, RBAC, secure storage, and centralized monitoring, the solution provides a scalable and governable approach to managing access to cloud resources.
