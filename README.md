# ⚡ Bashira — Brawl Stars Analytics

Dashboard d'analytics compétitif pour Brawl Stars. Données synchronisées en temps réel depuis Google Sheets.

![HTML](https://img.shields.io/badge/HTML-Single%20File-e34c26?logo=html5&logoColor=white)
![Chart.js](https://img.shields.io/badge/Chart.js-4.4.1-ff6384?logo=chartdotjs&logoColor=white)
![License](https://img.shields.io/badge/License-Private-red)

---

## 🎮 Fonctionnalités

| Module | Description |
|--------|-------------|
| **Overview** | Stats globales, winrate, tendances par jour |
| **Battle Log** | Historique complet des matchs avec filtres |
| **Meta** | Tier list & classement des brawlers |
| **Brawlers** | Deep dive par brawler (matchups, synergies, maps) |
| **Maps** | Analytics par map avec top picks et meilleurs duos |
| **Draft** | Simulateur de draft avec recommandations |
| **Teams** | Analytics par équipe (roster, forme, H2H) |
| **Head 2 Head** | Heatmap de matchups brawler vs brawler |
| **Players** | Stats individuelles par joueur et picks favoris |

## 🏟️ Teams supportées

EMEA, NA, SA, APAC — inclut entre autres : Tribe Gaming, FUT Esports, Reply Totem, KDS Esports, REJECT, Crazy Raccoon, LOUD, SK Gaming, Team Heretics, Natus Vincere, HMBLE, STMN Esports, ZETA DIVISION, Papara SuperMassive, CMM, et plus.

## ⚙️ Stack

- **Single-file HTML** — aucun build, aucune dépendance serveur
- **Google Sheets** comme backend (sync automatique via JSONP)
- **Chart.js** pour les graphiques
- **Fonts** : Outfit + JetBrains Mono

## 🚀 Déploiement

### GitHub Pages

1. Fork ou clone ce repo
2. Va dans **Settings → Pages**
3. Source : branche `main`, dossier `/ (root)`
4. Le site est live sur `https://<pseudo>.github.io/<repo>/`

### Local

Ouvre simplement `index.html` dans un navigateur.

## 📊 Source de données

Les données sont lues depuis un Google Sheet public au format suivant :

| Colonne | Description |
|---------|-------------|
| `date` | Date du match |
| `mode` | Mode de jeu (Gem Grab, Brawl Ball, etc.) |
| `map` | Nom de la map |
| `result_team1` | Résultat (victory / defeat) |
| `team1_name` / `team2_name` | Noms des équipes |
| `team1_player1_brawler` ... | Brawlers joués |
| `team1_player1_name` ... | Noms des joueurs |
| `set_id` / `set_score` | ID et score du set |

La sync se fait automatiquement toutes les **10 minutes**.

---

> Bashira — Built for competitive Brawl Stars analysis.
