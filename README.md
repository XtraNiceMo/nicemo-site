# nicemo-site

Public marketing site for **NiceMo LLC** — clinical AI for skilled nursing.

- **Production URL:** https://drmostrategists.biz (Azure Static Web Apps, free tier)
- **Fallback URL:** https://white-cliff-07bd4bb10.7.azurestaticapps.net
- **Owner:** Mo Gregory III · NiceMo LLC · Las Vegas, NV

## Architecture

Single static HTML page. No build step. Pure HTML + inline CSS + minimal JS.

## Deploy

Push to `main` triggers `.github/workflows/azure-static-web-apps.yml`, which uses the `AZURE_STATIC_WEB_APPS_API_TOKEN` repo secret to deploy via the official Azure action. No Azure CLI / Cloud Shell needed.

The deployment token was generated in Azure portal under the SWA resource `nicemo-llc-site` (resource group `nicemo-llc-site_group`, subscription `e8e37ab3-48e2-4e2a-8240-a46bf73a6333`).

## Central tenet

Every claim on the public site must trace to a verifiable source. The dashboard previews are labeled as illustrative mockups. The about-section stat boxes describe what NiceMo's clinical AI actually does (cite or refuse, audit trail) — not aspirational percentages.

Last edit (v0.2.1, 2026-05-16 PM): added "Sample data" banner above dashboards section + replaced unverifiable "100% / 0 fabricated" stat boxes with "Cite / Audit" labels.
