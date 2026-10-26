# app_json

Centralized Cloud JSON repository for dynamic content management across multiple mobile & web applications.

Allows adding, updating, and managing app data in real time **without publishing new APK/app updates to the Google Play Store or Apple App Store**.

---

## ⚡ Global Enterprise CDN (jsDelivr + GitHub Actions)

This repository is backed by **jsDelivr Global Edge CDN** (Cloudflare + Fastly) and has an automated **GitHub Action** (`.github/workflows/purge_cdn.yml`).

- **100% Automatic**: The instant you push changes to any `.json` file, GitHub automatically triggers a purge request.
- **Immediate Propagation**: The CDN edge flushes and pulls the new file worldwide in **under 3 seconds**.
- **Scalability**: Handles **100k+ to millions of users** at $0 cost with sub-30ms global latency.

---

## 📁 Repository Structure (Folder-Wise by App Name)

Each application has its own dedicated folder matching the app name:

```
app_json/
├── .github/workflows/
│   └── purge_cdn.yml       <-- Auto-purges CDN edge on every push
├── viral_ai_prompts/
│   └── prompts.json        <-- Curated viral prompts catalog
├── <next_app_name>/
│   └── data.json
└── README.md
```

---

## 📱 Registered Application Endpoints

### 1. Viral AI Prompts (`viral_ai_prompts`)
- **Folder**: [`viral_ai_prompts/`](./viral_ai_prompts/)
- **Data File**: [`viral_ai_prompts/prompts.json`](./viral_ai_prompts/prompts.json)
- **Primary Production CDN URL (Sub-30ms, 100k+ scalable)**:
  ```
  https://cdn.jsdelivr.net/gh/Riyaz-khan-shuvo/app_json@main/viral_ai_prompts/prompts.json
  ```
- **Direct GitHub Raw Fallback**: 
  ```
  https://raw.githubusercontent.com/Riyaz-khan-shuvo/app_json/main/viral_ai_prompts/prompts.json
  ```

---

## ➕ Adding a New App to this Repository
To support a new app:
1. Create a new folder named after your app (e.g., `media_parlour/`, `sohoj_ide/`, etc.).
2. Put your JSON data file inside that folder (e.g., `media_parlour/data.json`).
3. Commit and push to `main`.
4. Your new app can fetch with instant edge updates from:
   ```
   https://cdn.jsdelivr.net/gh/Riyaz-khan-shuvo/app_json@main/<app_name>/<file_name>.json
   ```

---

## 📜 Maintenance
Published and maintained by **SOHOJ MEDIA**.
All rights reserved.
