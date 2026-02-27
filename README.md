# ⚔ Bashira — Brawl Stars Analytics Dashboard

Dashboard d'analyse compétitif pour Brawl Stars. Connecté à Google Sheets pour le suivi automatique des scrims.

## 🚀 Déploiement (GitHub Pages)

1. Push ce repo sur GitHub
2. **Settings → Pages → Source:** `main`, dossier `/ (root)`
3. Dashboard live à `https://ton-pseudo.github.io/bashira/`

## ✨ Fonctionnalités

- **Overview** — Win rate, games, sets, période
- **Meta** — Tier list brawlers, comps, synergies
- **Brawlers** — Stats détaillées par brawler
- **Teams** — Classement par tier, roster, H2H
- **Battle Log** — 100 derniers matchs cliquables (joueurs, durée)
- **Draft Help** — Counter pick + simulateur de draft
- **Players** — Stats individuelles
- **Maps** — Stats par map avec top brawlers
- **Filtres** — Mode (6 modes) + Jours (5J/15J/30J/ALL)
- **Auto-refresh** toutes les 10 minutes

## 🔗 Google Sheets

Le sheet doit être **public en lecture** et s'appeler `TRIAAPRIME`.

Pour changer de sheet, modifier dans `index.html` :
```javascript
var GS_SHEET_ID = "VOTRE_SHEET_ID";
```
