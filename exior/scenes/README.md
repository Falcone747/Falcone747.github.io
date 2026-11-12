# Visuels de scène de l'accueil EXIOR — spécifications

Architecture hybride : un visuel d'arrière-plan sans texte, sans bouton et sans chiffre, sur lequel le site superpose des
composants React (démonstrateurs, cartes, contrôles). Les tableaux, textes et contrôles ne sont jamais intégrés à l'image.
Seuls des visuels validés par EXIOR sont utilisés ; aucune image n'est générée par le site ni par l'agent.

Déposer les fichiers ici, puis renseigner leurs chemins dans `lib/archi/scene-visuals.ts` (ex. `/exior/scenes/optimisation-desktop.png`).

| Scène | Fichier desktop | Fichier mobile | Ton | Zones réservées au HTML (à laisser calmes, sans détail fort) |
|---|---|---|---|---|
| Optimisation | `optimisation-desktop.png` 2688×1800 | `optimisation-mobile.png` 1170×2400 | sombre (graphite) | bande haute 22 % (titre) ; rectangle central 84 % × 70 % (démonstrateur). Le visuel s'exprime sur les bords et derrière le titre. |
| MetaCortex | `metacortex-desktop.png` 2688×1500 | `metacortex-mobile.png` 1170×1600 | clair | moitié gauche du bandeau haut (titre et flèches) ; bande basse 70 % (cartes du carrousel). Le visuel s'exprime dans le quart supérieur droit. |
| Meta-OS | `metaos-desktop.png` 2688×1700 | `metaos-mobile.png` 1170×2600 | clair | bandeau haut 25 % (titre, texte, action) ; colonnes gauche et droite (tuiles). Le visuel s'exprime au centre, derrière la tuile Meta-OS. |

Exigences : PNG ou WebP haute résolution (rapport 2×), palette graphite, argent et violet EXIOR (#080A10, #DCDFEA, #7029F5,
#9550FF), aucune typographie, aucun logo autre que le logo officiel, aucune photographie générique, aucune image générée
sans validation. Poids cible après compression : moins de 400 Ko par fichier (WebP qualité 80).
