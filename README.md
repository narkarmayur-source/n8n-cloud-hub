# 🚀 My 24/7 n8n Cloud Hub (7 GB RAM)

This repository automatically runs n8n inside GitHub Actions on a dedicated Ubuntu runner with **7 GB of RAM** and connects directly to your **Neon PostgreSQL** database.

## 🔐 Required GitHub Secrets
Go to your repository **Settings** -> **Secrets and variables** -> **Actions** -> **New repository secret**:

| Secret Name | Value |
| :--- | :--- |
| `DB_HOST` | `ep-holy-fire-be1osazl.c-9.us-east-2.aws.neon.tech` |
| `DB_NAME` | `n8n` |
| `DB_USER` | `neondb_owner` |
| `DB_PASSWORD` | `<your-neon-database-password>` |
| `N8N_ENCRYPTION_KEY` | `oHpKHdHx6iuL9lGNK0FDPITo9SIhzAoF` |

*(Optional: If you use a custom domain on Cloudflare, add `CLOUDFLARE_TUNNEL_TOKEN`. Otherwise, a free `trycloudflare.com` URL is generated automatically!).*

## ⚡ How to Start
1. Go to the **Actions** tab in this repository.
2. Click **🚀 n8n 24/7 Cloud Runner (7 GB RAM)** on the left.
3. Click **Run workflow** -> **Run workflow**.
4. Click on the running job — your live **`https://...trycloudflare.com`** URL will appear right at the top of the job summary!
