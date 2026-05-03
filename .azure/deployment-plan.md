# Deployment Plan: University SMS Django on Azure App Service

## Phase 1: Planning

### Step 1: Workspace Analysis

- **Mode**: MODIFY (existing Django project)
- **Framework**: Django 6.0.4
- **Language**: Python 3.14.4
- **Current Status**: Running locally, pushed to GitHub

### Step 2: Azure Services Selection

- [ ] Azure App Service (Web App) - Primary compute
- [ ] Azure Database for PostgreSQL - Database service
- [ ] Azure Storage Account - Static/media files
- [ ] Azure Key Vault - Secrets management

### Step 3: Infrastructure as Code Format

- [ ] Bicep (selected)
- [ ] Terraform

### Step 4: Recipe/Template Selection

- Selected: **Python/Django Web App with Database**
- Deployment target: Azure App Service (Windows or Linux)
- Database: Azure Database for PostgreSQL

### Step 5: Configuration Parameters

- **Subscription ID**: [To be confirmed]
- **Resource Group**: [To be created]
- **Location**: [To be selected]
- **App Name**: cavendish-university-sms
- **Database Name**: universitysms_db

### Step 6: Final Plan Approval

- [ ] User approved plan

## Phase 2: Preparation (Pending Approval)

### Step 1: Create Infrastructure Files

- [ ] `.azure/config.json` - azd configuration
- [ ] `infra/main.bicep` - Infrastructure definition
- [ ] `infra/main.parameters.json` - Parameters
- [ ] `azure.yaml` - azd project configuration

### Step 2: Containerization

- [ ] `Dockerfile` - Container image for deployment

### Step 3: Update Django Settings

- [ ] Configure production settings
- [ ] Set up database connections
- [ ] Configure static files handling

### Step 4: CI/CD Configuration

- [ ] GitHub Actions workflow (optional)

## Phase 3: Validation (Pending Preparation)

- [ ] Validate Bicep templates
- [ ] Verify configuration

## Phase 4: Deployment (Pending Validation)

- [ ] Deploy to Azure
- [ ] Run database migrations
- [ ] Test application

---

## Status

**Current**: ⏳ Awaiting Phase 1 Approval
