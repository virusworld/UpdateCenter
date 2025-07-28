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

## 📁 Repository Structure
