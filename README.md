# Nexa CRM — Monorepo

```
nexa-crm/
├── flask-backend/     → Python Flask API
│   ├── app.py
│   ├── wa_cloud.py
│   ├── a.py
│   ├── requirements.txt
│   └── service-account.json  ← .gitignore'da, commit etme
│
├── wa-bot/            → Node.js Baileys WA Bot
│   ├── index.js
│   └── package.json
│
├── render.yaml        ← Render deploy konfigürasyonu
└── .gitignore
```

## Render Deploy

render.yaml sayesinde otomatik. Dashboard'da:
- nexa-flask → Root Dir: `flask-backend`
- nexa-wa-bot → Root Dir: `wa-bot`

## Env Variables (Render Dashboard'dan gir)

```
TELEGRAM_BOT_TOKEN
TELEGRAM_CHAT_ID
WA_PHONE_NUMBER_ID
WA_ACCESS_TOKEN
WA_VERIFY_TOKEN
WA_ADVISOR_PHONE
FIREBASE_SERVICE_ACCOUNT   ← service-account.json içeriği (JSON string)
```
