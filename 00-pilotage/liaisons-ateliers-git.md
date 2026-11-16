# Module 04 — Liens entre ateliers et versionnement autonome

Ce dossier possède un historique Git distinct de celui de chaque atelier.

- Dépôt commun : https://github.com/elhisse-CLPrepas/mon-dossier-challenge-module04
- Site du module : https://elhisse-clprepas.github.io/mon-dossier-challenge-module04/
- Branche : `main` ; distant : `origin` ; publication Pages depuis `main`, à la racine `/`.

## Ouvrir les ateliers depuis cette copie située dans S13

| Séance | Atelier local | Dépôt GitHub vérifié |
|---|---|---|
| S13 | [Ouvrir l’atelier](../../OUVRIR-SEANCE-13.html) | [Dépôt S13](https://github.com/elhisse-CLPrepas/atelier-seance-13-ln-ia) |
| S14 | [Ouvrir l’atelier](../../../atelier-seance-14-ln-ia/OUVRIR-SEANCE-14.html) | [Dépôt S14](https://github.com/elhisse-CLPrepas/atelier-seance-14-ln-ia) |
| S15 | [Ouvrir l’atelier](../../../atelier-seance-15-ln-ia/OUVRIR-SEANCE-15.html) | [Dépôt S15](https://github.com/elhisse-CLPrepas/atelier-seance-15-ln-ia) |
| S16 | [Ouvrir l’atelier](../../../atelier-seance-16-ln-ia/OUVRIR-SEANCE-16.html) | Aucun dépôt Git local identifié lors de la préparation. |

Les liens locaux nécessitent de conserver les ateliers voisins dans `ATELIERS-MODULE-04`. Sur GitHub ou depuis une copie placée dans un autre atelier, utiliser les liens GitHub et le site commun ; ces chemins locaux sont propres à la copie S13.

## Relier les productions

Conserver dans ce dépôt commun les fiches S13 à S16 de `04-communication/`, les observations de `05-automatisation/` et le portfolio de `07-portfolio/`. Enregistrer les exports des ateliers dans les rubriques de la séance correspondante sans remplacer les preuves des séances précédentes.

Les copies du Module 04 présentes dans différents ateliers ne se synchronisent pas automatiquement. Le README distant consulté le 9 novembre 2026 désigne la copie située dans l’atelier S14 comme copie de travail active. La copie S13 contient aussi des modifications locales à intégrer. Éviter de travailler simultanément sur les mêmes fichiers dans ces deux copies.

## Vérifier le dépôt avant un commit

Dans le terminal ouvert à la racine de `mon-dossier-challenge-module04` :

```powershell
git rev-parse --show-toplevel
git remote -v
git status
git fetch origin
git log --oneline HEAD..origin/main
```

Le chemin racine doit finir par `mon-dossier-challenge-module04` et `origin` doit désigner le dépôt commun du module, plutôt que celui de l’atelier.

Si GitHub contient des changements, les intégrer avant de publier. Avec des modifications locales, les sauvegarder dans un commit local puis utiliser `git rebase origin/main` ; résoudre les éventuels conflits avant le push. Ne pas utiliser de push forcé pour synchroniser les copies.

```powershell
git add <fichiers-a-versionner>
git diff --cached --stat
git diff --cached --check
git commit -m "Actualiser les productions du Module 04"
git rebase origin/main
git push origin main
```

Dans une autre copie sans modifications locales, récupérer ensuite le résultat avec `git pull --ff-only`. Si elle contient déjà des changements, les examiner et les préserver avant toute intégration.

## Séparation des dépôts et état pédagogique

Un commit dans ce dossier ne crée aucun commit dans l’atelier parent. L’atelier S13 suit actuellement une copie des fichiers du module ; les ateliers conservent leurs propres réglages Git. Cette liaison par liens et dépôt commun ne nécessite ni sous-module ni déplacement des dossiers.

Les fichiers temporaires, les sauvegardes, les secrets et les caches sont exclus. Les traces pédagogiques restent des brouillons tant que les étapes et décisions humaines ne sont pas réellement attestées. Le notebook modifié contient une mention « VALIDÉE » qui ne correspond pas au statut non validé du guide source ; des sorties conservées peuvent correspondre à une ancienne version du code. Ces modifications de travail ne prouvent aucune validation ni exécution récente.
