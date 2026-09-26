# onboarding

Static **GitHub Pages** site for Kinfold staff-facing forms (custom domain `onboarding.kinfoldinns.co.uk`).

| Page | URL | Posts to |
|---|---|---|
| Payroll / new-starter form | `/` (`index.html`) | Staff Hub Apps Script `doPost` (`formType: onboarding`) |
| Signed-contract upload | `/return-contract.html?token=…` | Same web app (`formType: signed-contract-upload`) |

Backend: [kinfoldstaffhub](https://github.com/charlesknew-alt/kinfoldstaffhub) Apps Script (execute as deploying user, anyone anonymous).

DNS / Pages: CNAME `onboarding.kinfoldinns.co.uk` → this repo’s `main` branch (root). No DNS change needed when adding pages under the same host.

## Deploy

Push to `main` — GitHub Pages rebuilds automatically. Then clasp-deploy Staff Hub if API handlers changed.
