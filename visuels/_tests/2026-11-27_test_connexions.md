# Test des connexions — tâche planifiée du 27/11/2026 (MODE TEST)

Aucune publication, aucune programmation, aucun brouillon, aucune modification Metricool / Buffer / Instagram / TikTok / Systeme.io.

## 1. Outils présents

| Famille | Résultat | Détail |
|---|---|---|
| Metricool | OK | createScheduledPost, createScheduledPostForReview, getAnalyticsDataByMetrics, getBrandSettings, getScheduledPosts, sendScheduledPostForReview, updateScheduledPost, getAnalyticsAvailableMetrics, getBestTimeToPostByNetwork |
| Buffer | OK | get_account, list_channels, get_channel, list_posts, get_post, create_post, edit_post, delete_post, get_aggregated_post_metrics, ideas/templates/tags… |
| Claude_Docs | OK | batch, guide, update, read, query (+ create, delete, export différés) |
| claude-code-remote | PARTIEL | create_trigger, delete_trigger, fire_trigger, list_triggers, send_later, update_trigger. **add_repo / list_repos absents** (ToolSearch : « No matching deferred tools found ») |
| remote-devices | ABSENT | aucun outil (normal en tâche planifiée cloud) |

## 2. Metricool (lecture)

- getBrandSettings : **OK** — marque « mynra.io » (id 8380858), fuseau Europe/Paris, Instagram = mynra.io, TikTok = mynra.io.
- getAnalyticsAvailableMetrics (instagram, tiktok) : **OK** — connecteurs evolution / posts / reels / stories (IG) et evolution / posts (TikTok).
- getAnalyticsDataByMetrics, 28/10 → 27/11/2026 : **OK**

Instagram (compte) :
- Abonnés (IGEV01) : 35 (25 et 26/11)
- Portée (IGEV06) : valeurs quotidiennes, pics 103 (29/10) et 108 (08/11), total ≈ 243
- Interactions (IGEV09) : 6 (05/11) + 5 (08/11)
- Enregistrements posts (IGEV15) : 1 (08/11)
- Vues (IGEV05), partages (IGEV40), clics site (IGEV10), vues profil (IGEV07), abonnés gagnés (IGEV43) : **absents / null** (0 uniquement le 27/11)

Instagram par publication (IGPO) : **OK** — 3 carrousels
- 08/11 DfejzorDO_a : portée 6, vues 12, interactions 5, enregistrements 1, partages 0
- 05/11 DfXIpKwDBV- : portée 5, vues 12, interactions 3, enreg. 0, partages 0
- 05/11 DfXIUJsDBRR : portée 5, vues 8, interactions 3, enreg. 0, partages 0
- Clics (IGPO09) : null

TikTok (compte) :
- Abonnés (TKEV07) : 1 156 (25/11)
- Vues (TKEV02) : 1 823 (07/11) + 1 176 (08/11)
- Portée (TKEV11) : 566,7 (07/11), 549 (08/11)
- Interactions (TKEV06) : 7 + 15 ; partages (TKEV05) : 0 + 1
- Vues profil (TKEV09) : 1 (14/11), 0 ailleurs ; nouveaux abonnés (TKEV08) : 0

TikTok par vidéo (TKPO) : **OK** — 5 vidéos (07–08/11), vues 276 à 808, portée 252 à 760, likes 2 à 12, partages 0–1.

Absent : clics, enregistrements TikTok (non proposés par le connecteur).

## 3. Buffer (lecture seule)

- get_account : **OK** — cindy97329, organisation « My organization » (6b083bbeab9397692df597dc), fuseau Europe/Paris, limites 3 canaux / 10 posts programmés.
- list_channels : **OK** — mynra.io Instagram (business, 6b083d4b8541f09ecbb0098c, connecté) ; mynra.io TikTok (6b083c2a8541f09ecbaff1e4, connecté).
