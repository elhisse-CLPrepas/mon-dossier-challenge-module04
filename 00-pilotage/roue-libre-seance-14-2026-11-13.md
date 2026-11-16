# Roue libre séance 14 Comprendre et produire avec l’IA

**Vendredi 13 novembre 2026 · Module 04 · Approfondissement proposé de 90 minutes**

Support préparé par ORIA CODE à la demande du formateur. Les exemples sont fictifs et les productions restent des **BROUILLONS — À RELIRE**. Décision du pilote : **EN ATTENTE**.

Cette Roue libre explore une question : **comment passer d’une production accompagnée par l’IA à une automatisation progressive que l’on sait expliquer et contrôler ?** Le fil conducteur est le message court de S14 : conserver les faits, varier la formulation, mesurer certains critères et justifier une correction.

Le calendrier initial du dossier place S14 au 9 novembre et S15 au 13 novembre. Ce support correspond à la séance S14 demandée pour aujourd’hui ; il ne modifie pas le calendrier historique et prépare la continuité vers S15 et S16.

## Point de départ repris du prompt S14

Référence : [prompt maître S14](https://github.com/elhisse-CLPrepas/atelier-seance-14-ln-ia/blob/main/02-PROMPT/02-PROMPT-MAITRE-S14.md), étape 1 : « Reprendre les sources S13 ». Le prompt demande d’avancer une étape à la fois et d’attendre la contribution du participant. La présente préparation réalise la lecture des sources ; elle ne remplace pas les contributions attendues.

La [fiche S13](../04-communication/comprendre-processus-communication.md), datée du 6 novembre 2026, est partiellement remplie. Son cas est fictif ; sa première rédaction est un exemple fourni par l’atelier. Les champs de preuve et de répartition des rôles restent à compléter.

| Élément à confirmer | Appui accessible |
|---|---|
| Public : formateurs débutants en production assistée par IA | Fiche S13, « Les six questions », point 2 : « des formateurs qui débutent en production assistée par IA » |
| Fait 1 : le guide illustre le remplacement d’un terme technique pour les débutants | [Guide S12](../06-ressources/sources/guide-pratique-v2-a-relire.md), V2 — À RELIRE / NON VALIDÉE, « Étape 3 — Corriger en distinguant le fond et la forme », point 2 : « ce que l’IA sait ou ne sait pas vérifier » |
| Fait 2 : le journal donne la raison de cette correction | [Journal S12](../06-ressources/sources/journal-corrections-v1-v2.md), V1 → V2, ligne « Forme — accessibilité » : « Expliciter l’adaptation à un lecteur débutant » |
| Action unique proposée | Fiche S13, point 5 : « Souhaitez-vous voir un extrait du journal de corrections ? » |

La [fiche S14 existante](../04-communication/message-court-projet.md) conserve déjà trois variantes de l’assistant. La rédaction personnelle, le choix final et la correction motivée restent à compléter. Le cadrage y est noté comme confirmé dans une conversation antérieure ; pour cet approfondissement, demander s’il reste pertinent.

**Relance d’ouverture :** « Gardons-nous ce public, ces deux faits et cette seule action ? Si oui, écrivez vous-même deux ou trois lignes avant de demander de nouvelles variantes. »

## Comprendre ce que chacun apporte

| Acteur ou outil | Rôle dans cet atelier | Limite à expliquer |
|---|---|---|
| Participant | Définit le besoin, apporte les sources, rédige, choisit et corrige | Une intention doit être transformée en critères observables |
| IA | Propose des formulations, aide à expliciter des critères et à écrire du code | Une formulation plausible peut contenir un fait sans appui |
| Python | Exécute les règles écrites : compter, comparer, signaler un écart | Un programme peut appliquer correctement une règle insuffisante |
| Jupyter | Réunit consignes, code et sorties dans un notebook que l’on exécute par étapes | Une sortie visible peut provenir d’une ancienne exécution |
| Pilote humain | Examine le sens, les sources et le contexte ; décide de la validation | La décision ne se déduit pas d’un compteur ou d’une exécution réussie |

Python est le langage qui exprime les opérations. Un script `.py` les enchaîne à l’exécution. Jupyter est l’environnement de notebook ; un noyau Python exécute ses cellules de code. Les cellules de texte permettent d’expliquer l’hypothèse, la méthode et les limites près des résultats.

Dans ce cas, la démonstration n’appelle pas un modèle d’IA : les variantes sont déjà préparées. Python mesure ces textes. Jupyter permet d’observer et de discuter les opérations. L’IA peut aider à construire le dispositif, mais n’est pas nécessaire pour chaque exécution.

## Déroulement de la Roue libre

| Temps proposé | Activité | Trace attendue |
|---|---|---|
| 0 à 10 min | Lire le cadrage S13 et retrouver les deux passages sources | Public, faits et action confirmés ou corrigés |
| 10 à 25 min | Rédiger personnellement deux ou trois lignes ; observer les variantes existantes | Texte original conservé, propositions IA attribuées |
| 25 à 40 min | Expliquer la règle de comptage puis lancer le script | Commande, mesures et interprétation |
| 40 à 55 min | Examiner les trois pièges : répétition, autre invitation, promesse | Une règle utile et son contre-exemple |
| 55 à 75 min | Reprendre dans Jupyter, changer une seule entrée et réexécuter | Avant, modification, sortie et explication |
| 75 à 90 min | Choisir une correction, enregistrer et rouvrir la production | AVANT / APRÈS / POURQUOI et preuve à compléter |

Ces durées sont une proposition d’animation ; elles ne décrivent pas une séance déjà observée.

## Automatiser progressivement

On automatise d’abord une opération comprise et répétable. Avant d’écrire une règle, préciser son entrée, son résultat attendu et un cas où elle se tromperait sur l’objectif pédagogique.

1. **Faire et expliquer.** Lire le message et ses sources ; nommer les faits et l’action attendue.
2. **Stabiliser une règle.** Par exemple : compter les occurrences exactes de la phrase d’action. Cette règle répond à une question étroite.
3. **Exécuter sur plusieurs variantes.** Employer la même méthode pour A, B et C et conserver les sorties.
4. **Chercher les limites.** Ajouter une autre invitation ; observer que le compteur peut rester à 1.
5. **Préparer une production répétable.** Pour la suite du module, envisager un export dans un nouveau fichier, avec entrées, règle et résultat traçables. Le script S14 actuel affiche seulement les résultats.
6. **Décider après examen.** Relire les faits et le sens avant toute validation ou diffusion.

Le passage à l’étape suivante dépend de la compréhension et de la qualité des contrôles. Automatiser davantage n’est pas en soi un progrès si l’on reproduit plus vite une erreur.

## Expérience Python

Depuis la racine `atelier-seance-14-ln-ia`, exécuter :

```powershell
python mon-dossier-challenge-module04/06-ressources/seance-14/demo/comparer-variantes-s14.py
```

Ressources : [script](../06-ressources/seance-14/demo/comparer-variantes-s14.py) et [cas JSON](../06-ressources/seance-14/demo/cas-guide.json). Le script lit ce cas fictif et affiche les résultats sans modifier de fichier. Ne pas confondre ses textes préparés avec les variantes de la fiche personnelle S14.

Le cœur de la mesure est :

```python
len(texte), texte.count(action)
```

`len` compte ici les points de code Unicode de la chaîne, espaces et ponctuation compris ; ce n’est pas une mesure de la largeur visuelle. `count` recherche la chaîne exacte et distingue notamment la casse et la ponctuation. Une reformulation de l’action peut donc lui échapper.

### Résultats de l’exécution réalisée par ORIA CODE le 13 novembre 2026

| Texte du cas de démonstration | Longueur | Occurrences exactes de l’action |
|---|---:|---:|
| Exemple humain fourni | 144 | 1 |
| A | 149 | 1 |
| B | 195 | 1 |
| C | 166 | 1 |
| Répétition exacte ajoutée | 208 | 2 |
| Autre action ajoutée | 175 | 1 |
| Promesse sans source | 101 | 1 |
| C corrigée dans la démonstration | 159 | 1 |

Le script s’est terminé avec le code 0. Il s’agit d’une exécution technique de l’assistant, pas d’une observation de la pratique du participant.

### Trois questions à débattre

- **208 caractères, 2 occurrences :** la règle repère bien la répétition exacte. Faut-il supprimer la répétition ? Justifier selon le besoin.
- **175 caractères, 1 occurrence :** « Abonnez-vous à la lettre » ajoute une seconde invitation. Le comptage ne garantit donc pas une action unique.
- **101 caractères, 1 occurrence :** « Ce guide garantit un document sans erreur » respecte le comptage, mais la promesse n’est pas étayée. Vérifier les sources reste nécessaire.

Relance : « Quelle conclusion précise puis-je tirer du résultat, et quelle conclusion serait abusive ? »

## Expérience Jupyter

Ouvrir le [notebook S14 existant](../06-ressources/seance-14/demo/comparer-variantes-s14.ipynb) dans un environnement compatible avec Jupyter et sélectionner un noyau Python. S’il n’est pas disponible, poursuivre avec le script et lire le notebook comme support ; l’installation n’est pas une condition pour comprendre cette séance.

1. Enregistrer une copie de travail dans `05-automatisation/` avant de modifier le notebook source.
2. Lire les cellules avant de les lancer et prédire le résultat attendu.
3. Redémarrer le noyau et exécuter toutes les cellules dans l’ordre pour repartir d’un état connu.
4. Retrouver les trois mesures A, B et C puis les comparer au tableau ci-dessus.
5. Dans la copie, ajouter une invitation différente à un message. Réexécuter les cellules concernées, puis toutes les cellules depuis un noyau redémarré.
6. Consigner ce qui change et expliquer pourquoi une seule occurrence peut correspondre à deux invitations.
7. Enregistrer, fermer et rouvrir la copie. Distinguer les sorties enregistrées de celles réellement recalculées.

**Apport de Jupyter :** le participant peut placer une prédiction et une interprétation près du code, modifier une entrée et suivre les sorties par étapes. Le notebook garde ensemble le raisonnement et l’expérience. Son intérêt pédagogique dépend de ces explications, pas seulement de la présence de cellules exécutées.

**Piège à montrer :** modifier une variable puis ne relancer qu’une cellule dépendante peut laisser d’autres sorties anciennes à l’écran. Redémarrer et tout exécuter aide à contrôler la cohérence de l’ensemble. Le notebook n’a pas été exécuté par l’assistant dans cette préparation.

## Questions pour approfondir

- Que signifie « produire avec l’IA » si l’on ne sait pas expliquer la correction retenue ?
- Quelle différence entre demander trois variantes à l’IA et faire mesurer trois textes par Python ?
- Quel critère doit rester identique entre les variantes : faits, public, action ou longueur ? Pourquoi ?
- Si l’IA propose une règle Python, quel contre-exemple peut-on lui opposer avant de la réutiliser ?
- Qu’apporte un notebook à un partenaire qui souhaite comprendre le résultat ?
- Quelle partie du processus peut-on répéter sans intervention, et à quel moment doit-on s’arrêter pour décider ?

## Production à conserver et continuité du module

Compléter la [fiche message S14](../04-communication/message-court-projet.md) sans effacer l’existant : rédaction personnelle, variante et canal retenus, correction AVANT / APRÈS / POURQUOI, puis texte final entier. Conserver les propositions de l’assistant comme telles.

Pour la preuve S14, utiliser [le portfolio existant](../07-portfolio/preuves-module-04.md) après la pratique réelle. Ne pas transformer l’exécution technique de l’assistant en preuve personnelle. Conserver la preuve S13 et la décision du pilote en attente jusqu’à sa décision explicite.

À consigner après l’activité :

```text
Fichier produit : À COMPLÉTER
Entrées et sources utilisées : À COMPLÉTER
Règle exécutée et commande : À COMPLÉTER
Résultat réellement observé : À COMPLÉTER
Ce que la règle ne contrôle pas : À COMPLÉTER
Correction AVANT / APRÈS / POURQUOI : À COMPLÉTER
Date réelle de réouverture par le participant : À COMPLÉTER
Observation du partenaire ou formateur : À COMPLÉTER
Décision du pilote : EN ATTENTE
```

Pour S15, apporter deux variantes, leurs sources et une règle avec un contre-exemple. Pour S16, préparer un parcours de notebook reproductible et un export local à rouvrir et expliquer, selon les consignes de cette séance.

## Prompt de reprise après confirmation du cadrage

> Accompagne-moi dans la séance 14 à partir de mon dossier challenge Module 04. Utilise les sources accessibles et conserve les contenus existants. Nous avons confirmé le public, les deux faits sourcés et l’action unique. Demande-moi maintenant ma rédaction personnelle de deux ou trois lignes et attends ma réponse. Ensuite seulement, aide-moi à comparer trois variantes, choisir un canal et justifier une correction. Pour Python et Jupyter, distingue les règles exécutées, les résultats observés et les limites de leur interprétation. Ne présente aucun exemple de l’assistant comme ma rédaction, aucun compteur comme une validation, ni aucune sortie enregistrée comme une nouvelle exécution. Aucune diffusion. Décision du pilote : EN ATTENTE.
