# GCP Deployment Manager Studio

This repository contains the target configuration and SRE runtime files compiled by the **GCP Deployment Manager Studio** dashboard module.

## 🚀 Description
Build declarative layout sheets for GCP. Generate Python/YAML templates, specify resource properties, and manage nested deployment structures.

## 🛠️ Specification Matrix
- **Primary Configuration File**: `/deploy/dm/deployment.yaml`
- **Execution Command**: `gcloud deployment-manager deployments create dep --config=deployment.yaml`
- **Validation Command**: `gcloud deployment-manager deployments list`

## 📋 How to Run & Validate

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Pradeeptalari14/tp-gcp-deployment-manager.git
   cd tp-gcp-deployment-manager
   ```

2. **Run Execution Target:**
   ```bash
   gcloud deployment-manager deployments create dep --config=deployment.yaml
   ```

3. **Verify Runtime Stability:**
   ```bash
   gcloud deployment-manager deployments list
   ```

## 🔐 Security & Best Practices
* **Secret Isolation**: Use organization-level secrets (or SSM parameter hooks) rather than hardcoded environment variables inside files.
* **Pull Request Lifecycles**: Protect default branch merges with validation checks before merging code changes.
