# Cloud Platform Comparison & Architectural Mapping

## Core Cloud Services Comparison Matrix

| Cloud Functionality | AWS Equivalent Service | Azure Equivalent Service | GCP Equivalent Service |
| :--- | :--- | :--- | :--- |
| **Virtual Servers (Compute)** | Amazon EC2 | Azure Virtual Machines | Compute Engine |
| **Object Storage** | Amazon S3 | Azure Blob Storage | Cloud Storage |
| **Virtual Private Network** | Amazon VPC | Azure Virtual Network (VNet) | VPC Network |
| **Identity & Access Control** | AWS IAM | Microsoft Entra ID | Cloud IAM |

---

## Technical Architectural Comparison

### 1. Compute Services
- **AWS (EC2)**: Highly customizable instance types with extensive scaling options and AMI ecosystem.
- **Azure (VMs)**: Deep enterprise integration with Windows Server licensing and hybrid connectivity via Azure Arc.
- **GCP (Compute Engine)**: Fast boot times, custom machine configurations, and native optimization for containerized microservices.

### 2. Storage Systems
- **AWS (S3)**: Industry standard for object storage offering extensive tiering policies (Glacier, Standard-IA).
- **Azure (Blob)**: Seamless integration with enterprise data lakes and Windows file systems.
- **GCP (Cloud Storage)**: Single unified API across storage classes with high global network performance.

### 3. Networking Models
- **AWS (VPC)**: Region-bound virtual private cloud with detailed subnet and security group configurations.
- **Azure (VNet)**: Region-bound network isolated per subscription with strong hybrid ExpressRoute support.
- **GCP (VPC)**: Global resource span by default, allowing cross-region subnets in a single VPC.

---

## Linux Systems to Cloud Architecture Mapping

| Local Linux Primitive | Cloud Architectural Equivalent | Operational Function |
| :--- | :--- | :--- |
| **Local OS Instance / Shell** | Compute Instance (EC2 / Azure VM / GCP CE) | Executing workloads, hosting services, and running applications. |
| **`/etc/passwd` / `useradd`** | IAM Services (AWS IAM / Entra ID / GCP IAM) | Managing user identities, authentication, and access control. |
| **`iptables` / `nftables`** | Security Groups / Network ACLs | Filtering network traffic and controlling inbound/outbound rules. |
| **Local File System (`/var`, `/home`)** | Block / Object Storage (EBS, S3, Blob, Cloud Storage) | Persisting state, system files, media, and backups. |
