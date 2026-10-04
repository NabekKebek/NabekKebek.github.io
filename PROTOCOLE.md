# PROTOCOLE NABEK - Version 2.0

## Règle fondamentale
- Quand l'utilisateur écrit `FINI` en majuscules, l'assistant met immédiatement à jour le protocole dans le dépôt.
- La mise à jour doit inclure :
  - le résumé du travail effectué,
  - l'état actuel du projet,
  - l'étape précise où l'on est rendu,
  - les fichiers modifiés,
  - les prochaines actions.
- Les confirmations inutiles doivent être évitées. Une confirmation directe et concise suffit.
- Si une action est demandée, elle est exécutée immédiatement, sans boucles de validation répétées.

## Workflow simplifié
1. L'utilisateur donne une demande.
2. L'assistant confirme brièvement et exécute.
3. L'utilisateur écrit `FINI`.
4. L'assistant met à jour ce fichier `PROTOCOLE.md` dans le dépôt.
5. L'assistant reprend ensuite directement à l'étape exacte où l'on est rendu.

## Format de mise à jour du protocole
```markdown
# PROTOCOLE NABEK - Suivi de session

## Session du [DATE]
**Utilisateur:** NabekKebek

### ✅ Travail effectué
- Point 1
- Point 2
- Point 3

### 📍 État actuel
- [Section 1]: [status]
- [Section 2]: [status]
- [Section 3]: [status]

### 🎯 Étape précise actuelle
**Localisation:** [fichier ou module]
**Action en cours:** [description détaillée]
**Prochaine étape:** [description claire]

### 📁 Fichiers modifiés
- `fichier.ext` — description

### 🔗 Résumé de la session
- Ce qui a été fait
- Ce qui reste à faire
- Où l'on reprend si l'utilisateur écrit `FINI`
```

## Règle de suivi après `FINI`
Quand `FINI` est écrit, la mise à jour doit être faite immédiatement dans le dépôt, conformément au format ci-dessus. L'objectif est de garder une trace exploitable pour reprendre sans perdre de temps.

## État actuel de la session
- Protocole activé
- Mise à jour automatique au signal `FINI`
- Confirmation directe prioritaire
- Pas de validation redondante

## Date d'activation
2026-10-04
