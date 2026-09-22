# Journal de prompts — Séance 1

> **GET 409 — Équipe CoutureDakar** — Master Prompt Engineer : Malick Faye Diagne
> Outil : Claude. Prompts issus de la *Bibliothèque de Prompts S1*, crochets remplacés par notre contexte.
> Transparence (Code de déontologie IA) : les livrables S1 ont été générés avec l'assistance de Claude à partir de ces prompts ; les champs « Retour critique » sont à compléter après ré-exécution et relecture humaine.

## S1 — Découverte

```
Tu es un expert en artisanat et commerce informel au Sénégal.
Identifie les 3 principaux problèmes que rencontrent les tailleurs de quartier
dans les ateliers de Dakar (Médina, HLM, Colobane) pendant la période de Tabaski.
Pour chaque problème, indique :
- La cause principale
- L'impact sur la vie quotidienne
- Une piste de solution technologique accessible
```
**Retour critique :** _à compléter_ — point de vigilance : vérifier si l'IA propose des outils en saisie texte, inadaptés à un utilisateur qui parle plus qu'il n'écrit (d'où le contexte « WhatsApp vocal, wolof » ajouté dans les prompts suivants).

## S2 — Guide d'interview

```
Tu es un UX Researcher spécialisé dans les usages numériques en Afrique de l'Ouest.
Je dois interviewer un tailleur-patron de 41 ans avec 3 apprentis
qui vit à Dakar (Médina) et fait face au problème suivant : pendant le rush
de Tabaski, il perd la trace de ses commandes et livre en retard.
Génère un guide d'interview d'empathie avec :
1. 3 questions d'ouverture
2. 5 questions d'exploration en profondeur (utilisant 'Pourquoi ?' et 'Racontez-moi...')
3. 2 questions sur les aspirations et les gains attendus
Format : questions numérotées, courtes, sans jargon technique.
```
**Résultat :** [guide-interview.md](guide-interview.md) — 10 questions ; la question 6 (décision d'accepter une commande) cible directement l'insight de surcharge.

## S3 — Générateur de HMW

```
Tu es un facilitateur en Design Thinking.
Voici les observations clés de notre interview avec Ousmane, tailleur à la Médina :
Observation 1 : mesures, tissus et acomptes notés sur papier ou mémorisés, perdus avant Tabaski
Observation 2 : il promet des dates sans connaître sa charge réelle
Observation 3 : les relances clients mangent son temps de production
La frustration principale identifiée est : il perd la trace de ses engagements
au moment où ils sont les plus nombreux.
Génère 5 énoncés 'Comment pourrions-nous...' (HMW).
Critères : ni trop vague, ni trop précis, ne propose pas encore de solution.
Format : liste numérotée, 1 phrase par énoncé.
```
**Résultat :** 3 énoncés conservés, sélection argumentée dans [hmw.md](hmw.md) ; critère d'élimination : tout énoncé qui impose déjà une solution (« via une application… »).

## S4 — Carte d'empathie Markdown

```
# ROLE
Tu es un UX Researcher expert en Design Thinking pour des projets d'innovation sociale en Afrique.
## PERSONA DE NOTRE EQUIPE
- Prénom, âge, profession : Ousmane, 41 ans, tailleur-patron
- Localisation : Médina, Dakar, Sénégal
- Problème principal : perd la trace de ses commandes pendant le rush de Tabaski
- Equipement digital : smartphone Android d'entrée de gamme, WhatsApp vocal, Wave
- Revenus approximatifs : très saisonniers, pic Tabaski/Korité
- Contexte familial : marié, 4 enfants, soutient sa mère
## OBSERVATIONS DE NOS INTERVIEWS
- Ce qu'il a dit : « Le problème ce n'est pas la couture, c'est de savoir qui m'a donné quoi, pour quand. »
- Ce qu'il a fait : répond au téléphone en cousant, note les acomptes au dos du cahier
- Emotion principale détectée : peur de perdre la face
## TACHE
Génère la Carte d'Empathie complète.
## FORMAT DE SORTIE STRICT
(sections 1 à 6 : Pense & ressent / Voit / Entend / Dit & fait / Pains / Gains)
```
**Résultat :** [carte-empathie.md](carte-empathie.md) — lignes marquées (H) = hypothèses à valider sur le terrain.

## Vigilance hallucinations

Aucune statistique chiffrée n'a été retenue dans les livrables : les chiffres proposés par l'IA (volumes de commandes, parts de chiffre d'affaires) n'ont pas de source et seront remplacés par les données des interviews terrain.
