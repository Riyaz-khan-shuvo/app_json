# app_json

Centralized Cloud JSON repository for dynamic content management across multiple mobile & web applications.

Allows adding, updating, and managing app data in real time **without publishing new APK/app updates to the Google Play Store or Apple App Store**.

---

## 📁 Repository Structure (Folder-Wise by App Name)

Each application has its own dedicated folder matching the app name:

```
app_json/
├── viral_ai_prompts/
│   └── prompts.json
├── <next_app_name>/
│   └── data.json
└── README.md
```

---

## 📱 Registered Application Endpoints

### 1. Viral AI Prompts (`viral_ai_prompts`)
- **Folder**: [`viral_ai_prompts/`](./viral_ai_prompts/)
- **Data File**: [`viral_ai_prompts/prompts.json`](./viral_ai_prompts/prompts.json)
- **Raw URL**: 
  ```
  https://raw.githubusercontent.com/Riyaz-khan-shuvo/app_json/main/viral_ai_prompts/prompts.json
  ```
- **Description**: Curated viral AI prompt catalog, aspect ratios, target tools, and categories.

---

## ➕ Adding a New App to this Repository
To support a new app:
1. Create a new folder named after your app (e.g., `media_parlour/`, `sohoj_ide/`, etc.).
2. Put your JSON data file inside that folder (e.g., `media_parlour/data.json`).
3. Commit and push to `main`.
4. Your new app can fetch from:
   ```
   https://raw.githubusercontent.com/Riyaz-khan-shuvo/app_json/main/<app_name>/<file_name>.json
   ```

---

## 📜 Maintenance
Published and maintained by **SOHOJ MEDIA**.
