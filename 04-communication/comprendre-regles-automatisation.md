# Comprendre les règles d’automatisation

S15 · vendredi 13 novembre 2026
Preuve : preuve-15-regles-adaptation-automatisation
Statut : BROUILLON — À RELIRE

## Source et repère
[À compléter]

## Variante S14 n° 1
[À compléter]

## Variante S14 n° 2
[À compléter]

## Fait invariant et appui
[À compléter]

## Variable et valeurs observées
[À compléter]

## Mon gabarit
[À compléter]

## Condition
[À compléter]

## Répétition
[À compléter]

## Tests aux bornes

Règle étalon du carnet : pour un texte renseigné, longueur > 400 donne « À raccourcir ». À 400 ou moins, la longueur est acceptable.

| Entrée | Ma prédiction | Observation après exécution |
|---|---|---|
| 400 caractères | [À compléter] | [À compléter] |
| 401 caractères | [À compléter] | [À compléter] |

Essais du carnet en attente.

## Interprétation des résultats
[À compléter]

## Contre-exemple avant correction
[À compléter]

## Correction humaine
[À compléter]

## Passage source et raison
[À compléter]

## Limite du contrôle automatique
[À compléter]

## Tableau à reprendre en S16

| Champ | Valeur | Source ou justification |
|---|---|---|
| projet | [À compléter] | [À compléter] |
| public | [À compléter] | [À compléter] |
| besoin | [À compléter] | [À compléter] |
| proposition | [À compléter] | [À compléter] |
| action | [À compléter] | [À compléter] |
| format | [À compléter] | [À compléter] |

## Autoévaluation
- [ ] Je retrouve mes deux variantes S14 et l’appui de l’invariant.
- [ ] Je distingue une variable de sa valeur et je peux lire mon gabarit.
- [ ] J’ai prédit puis observé les sorties à 400 et 401 caractères.
- [ ] J’explique pourquoi la promesse courte échoue à la relecture et je justifie ma correction.
- [ ] Mon tableau de données et ma règle de contrôle sont prêts à être repris en S16.

Observation et décision du pilote : en attente.

## Trace réelle S15 — 16 novembre 2026

Synthèse enregistrée par l’assistant à partir des choix confirmés dans le chat et des sorties Python réellement exécutées. Les rubriques modèles antérieures sont conservées ; cette synthèse constitue le relevé actuel.

### Source, variantes et gabarit

Guide : 01-exemple-sa-ia/guide-situation-actuelle-IA-publication-V5.pdf ; page 2 : « V5 — publication enrichie — Juillet 2026 » ; page 28 : « Prêt pour relecture humaine finale ».
Appui : page 2, sous-titre, « produire avec méthode » ; page 4, parcours pédagogique comprenant production et contrôle.
Les variantes A et B, proposées par IA puis acceptées par le participant, sont enregistrées dans ../08-accompagnement-S15-S16/01-SOURCES-ET-CADRAGE.md. Elles ne constituent pas des textes personnels S14 antérieurs à cet échange.
Invariant accepté : guide présenté et démarche de production et de contrôle.
Variable : titre ; valeurs comparées : « Comment garder le pilotage humain ? » et « Comment produire avec méthode ? ».
Gabarit : {titre} — {proposition} {action}.
Titre retenu : Comment produire avec méthode ?
Action : consulter https://elhisse-clprepas.github.io/mini-site-situation-actuelle-ia/

### Condition et répétition

Texte vide ou espaces seuls : À compléter ; sinon len(texte) > 400 : À raccourcir ; sinon : Longueur acceptable.
Le seuil est pédagogique ; Python len compte les points de code Unicode. Les espaces et le lien sont inclus dans les textes mesurés.
La boucle applique la même règle à chaque entrée.

| Entrée | Prédiction personnelle | Observation réelle | Outil |
|---|---|---|---|
| Vide | Non recueillie | 0 ; À compléter | Python 3.14.5 |
| Espaces seuls | Non recueillie | 3 ; À compléter | Python 3.14.5 |
| 400 lettres a et étalon fourni | Non recueillie | 400 ; Longueur acceptable | Python 3.14.5 |
| 401 lettres a et étalon fourni | Non recueillie | 401 ; À raccourcir | Python 3.14.5 |
| A | Non recueillie | 274 ; Longueur acceptable | Python 3.14.5 |
| B | Non recueillie | 270 ; Longueur acceptable | Python 3.14.5 |
| Message retenu | Non recueillie | 208 ; Longueur acceptable | Python 3.14.5 |

Prédictions non recueillies avant les tests : exécution directe explicitement demandée. Ne pas cocher la case « J’ai prédit puis observé » du modèle.
Le cas fictif a été retiré du suivi sur demande explicite du participant ; cette activité est écartée, pas validée. Aucune correction humaine sur ce cas ne fait partie de la trace retenue.
Limite : le contrôle de longueur ne vérifie ni la vérité des affirmations, ni leur adéquation au public. Les références et la relecture restent nécessaires.

### Fichiers et preuve

Rapport : ../08-accompagnement-S15-S16/04-RESULTATS-REELS-S15.md
Mesures et textes exacts : ../08-accompagnement-S15-S16/resultats-tests-s15.json
Script reproductible : ../08-accompagnement-S15-S16/executer-tests-s15.py
Les fichiers de résultats ont été relus techniquement par Python. Réouverture par le participant : À COMPLÉTER. Observation d’un tiers : À COMPLÉTER.
Décision du pilote sur la preuve : EN ATTENTE.
Notebook S16 : non exécuté. Six champs S16 : à confirmer à l’étape 7.

### Révision proposée

Les 12 flashcards et 8 questions du site S15 peuvent servir à réviser invariant, variable, condition, seuil, répétition et limite du contrôle. Révision et réponses du participant : non réalisées dans cet échange.
