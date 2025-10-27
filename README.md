# Mastodon Deployment Guide
_An open-source, federated microblogging platform (Twitter Alternative)_

Deploy a production‑grade Mastodon instance on a Linode VM behind Cloudflare DNS, managed through Cloudron.

## Overview
- **Cloudflare** – DNS & SSL termination  
- **Linode** – Linux virtual server (Ubuntu‑based)  
- **Cloudron** – Container platform that runs Mastodon (web, streaming, sidekiq, DB, Redis)

## Prerequisites
- Cloudflare account with an API token that has read/write DNS permissions  
- Linode account (API key or SSH access to a new VM)  
- A domain you control (to point at the VM)  

## High‑level steps
1️⃣ Provision a Linux VM (Ubuntu‑based).  
2️⃣ Create DNS records for your domain in Cloudflare that point to the VM’s public address.  
3️⃣ Run the official Cloudron installer on the VM (see Cloudron docs for the latest command).  
4️⃣ Deploy Mastodon via Cloudron’s Marketplace UI or CLI (refer to Cloudron docs for the exact command).  
5️⃣ Populate the required environment variables.

## License
MIT – feel free to reuse or improve.

## Contact
Questions? Reach me at `JunDocs@pm.me`.
