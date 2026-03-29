# QuantumReady365

> Instantly audit your Microsoft 365 tenant's post-quantum cryptography readiness and get a prioritized remediation roadmap before your encrypted data is at risk.

## Overview

QuantumReady365 scans an organization's M365 and Intune environment to identify legacy RSA-based cipher suites, deprecated TLS configurations, and non-PQC-compliant policies across endpoints, Exchange Online, SharePoint, and Entra ID. It generates a scored risk report aligned to NIST FIPS 203/204/205 standards and Microsoft's own PQC deprecation roadmap. The output is a board-ready PDF report plus a prioritized PowerShell remediation script pack that IT teams can execute immediately.

## Problem This Solves

IT teams have no fast, structured way to assess their current M365 cryptographic exposure to the 'store now, decrypt later' quantum threat — they lack visibility into which endpoints, policies, and services are using legacy ciphers that will eventually be cracked, and they have no remediation playbook tied to Microsoft's actual PQC migration timeline.

## Target Audience

IT admins and MSP consultants managing Microsoft 365 tenants for mid-market organizations (200–5000 seats), especially those in regulated industries like finance, healthcare, legal, and government con

## Tech Stack

PowerShell, Microsoft Graph API, PHP, Laravel, MySQL, HTML/CSS, ReportLab/FPDF

## Quick Start

```powershell
# Clone the repository
git clone https://github.com/quantumready365-m365-pqc-auditor.git
cd quantumready365-m365-pqc-auditor

# One-click install & run
.\Install.ps1

# Or run the script directly
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
.\scripts\{quantumready365-m365-pqc-auditor}.ps1
```

## Usage

Connect to a Microsoft 365 tenant via Graph API and enumerate TLS cipher suite configurations, Intune device compliance policies, Entra ID authentication method settings, and Exchange Online transport rules to flag any RSA-based or legacy cryptographic dependencies that conflict with NIST PQC standards, outputting a structured JSON risk report and auto-generated remediation commands.

## Monetization Strategy

Tiered model: (1) One-time PowerShell audit script pack sold on Gumroad or Lemon Squeezy at $79 for a single tenant license; (2) SaaS web dashboard with automated monthly re-scanning and delta reporting at $49/month per tenant sold direct or via AppSource; (3) White-label MSP license at $199/month covering up to 20 tenants. Consulting upsell at $250/hr for remediation implementation.

| Metric | Value |
|--------|-------|
| Revenue Potential | HIGH |
| Estimated Effort  | 1-3months |

## About the Author