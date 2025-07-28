# 🛠️ UpdateCenter

A centralized hub for managing versioned updates of multiple applications via a modular, fully configurable `Updater.exe`.

This repository hosts:
- 📦 Application update packages (.zip files)
- 📜 Manifest files describing each version
- 🗂 Organized folders for per-app version tracking

---

## 🚀 Purpose

The `UpdateCenter` serves as a backend system for a reusable, multi-tenant updater tool. It streamlines update delivery for apps deployed across different customers by separating:
- Global version metadata (per app)
- Per-customer expiry and access control logic (via Firebase Firestore)

This design enables:
- Scalable deployments for multiple applications
- Configurable update flow via remote manifests
- Versioned release management using GitHub Releases
- Secure and traceable file delivery

---


Each folder represents one app. Versions are tracked via subfolders. Manifests contain:
- Version number
- Changelog
- Download URL
- Optional integrity hashes

---

## 🧰 Updater Integration

`Updater.exe` reads:
- App-specific manifest from this repo
- Customer data from Firebase Firestore
- Local version file for comparison

Update logic follows:
1. Check app version and expiry
2. Download update ZIP if applicable
3. Replace existing binaries
4. Restart target app

---

## 📬 Contributions & License

This repository is maintained privately and not open to external contributions at the moment.

**License: None (private use only)**

---

Want to include instructions for adding a new app version or linking Firebase next? Happy to expand this into a full operational doc for your ecosystem. 🔧📘
## 📁 Repository Structure
