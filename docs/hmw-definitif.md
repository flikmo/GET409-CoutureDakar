# HMW Définitif — CoutureDakar

> **GET 409 — Lab Sprint S2 — Outil 3/3** · Construit avec le prompt P-HMW à partir de [chapeaux-bono.md](chapeaux-bono.md) et [vpc.md](vpc.md).

## HMW Draft S1

« Comment pourrions-nous aider les tailleurs de quartier à Dakar à suivre chaque commande — mesures, tissu, acompte, date promise — pendant le rush de Tabaski, afin de livrer à temps sans perdre la confiance de leurs clients ? »

## Entrées utilisées

| Source | Élément retenu |
|---|---|
| Chapeau Blanc | B1 — le suivi repose sur un cahier papier, des sachets marqués et la mémoire du patron |
| Chapeau Noir | N1 — tout outil à saisie texte sera abandonné dans le rush · N2 — le suivi seul ne stoppe pas la sur-acceptation |
| Chapeau Bleu | Qui tient le registre : le patron ou l'apprenti ? |
| VPC — Pain #1 | P1 perte de traçabilité → PS1 commande dictée + PS2 numéro de ticket |
| VPC — Pain #2 | P2 sur-promesse → PS4 compteur de charge |

## 3 versions proposées

### Version A
« Comment pourrions-nous aider les tailleurs de quartier de Dakar à enregistrer chaque commande sans avoir à écrire pendant le rush de Tabaski, afin de ne plus perdre mesures, tissus et acomptes ? »
- Plus précise car : intègre la contrainte d'usage réelle (pas de saisie texte).
- Risque Chapeau Noir intégré : N1.
- Évaluation : **trop étroite** — traite la traçabilité mais oublie la sur-acceptation (N2) ; on peut enregistrer parfaitement et livrer quand même en retard.

### Version B
« Comment pourrions-nous aider les tailleurs de quartier de Dakar à savoir, avant d'accepter une commande, s'ils pourront la livrer avant Tabaski ? »
- Plus précise car : cible le moment de décision (l'acceptation), vraie cause des retards.
- Risque Chapeau Noir intégré : N2.
- Évaluation : **trop étroite** — perd la traçabilité des acomptes et des mesures (P1, P5), ignore N1.

### Version C — ✅ retenue
« Comment pourrions-nous aider les tailleurs de quartier de Dakar à garder la trace de chaque commande — mesures, tissu, acompte, date promise — **sans avoir à écrire**, pendant le rush de Tabaski, afin qu'ils **n'acceptent que ce qu'ils peuvent livrer à temps** ? »
- Plus précise car : ajoute la contrainte d'usage (N1) et remplace un bénéfice vague (« ne pas perdre la confiance ») par un résultat observable (n'accepter que le livrable).
- Risques Chapeau Noir intégrés : N1 et N2.
- Évaluation : **bien calibrée** — une seule phrase, un persona, un moment, une contrainte, un résultat mesurable.

## HMW Définitif S2

> **« Comment pourrions-nous aider les tailleurs de quartier de Dakar à garder la trace de chaque commande — mesures, tissu, acompte, date promise — sans avoir à écrire, pendant le rush de Tabaski, afin qu'ils n'acceptent que ce qu'ils peuvent livrer à temps ? »**

## Ce qui a changé par rapport au draft S1

| Élément | Draft S1 | Définitif S2 | Pourquoi |
|---|---|---|---|
| Verbe | « suivre » | « garder la trace » | Plus concret : l'enjeu est de ne rien perdre, pas de « suivre » au sens abstrait |
| Contrainte d'usage | — | « sans avoir à écrire » | Chapeau Noir N1 : c'est ce qui fait échouer les outils existants |
| Bénéfice | « livrer à temps sans perdre la confiance » | « n'accepter que ce qu'ils peuvent livrer à temps » | Chapeau Noir N2 : la confiance est une conséquence ; la cause maîtrisable est l'acceptation |
| Solution imposée | aucune | aucune | « sans avoir à écrire » est une contrainte, pas une solution : vocal, photo, apprenti scribe ou ticket papier restent possibles |

## Pourquoi ce HMW ?

- **Ancrage** : tailleurs de quartier de Dakar (persona Ousmane, Médina), période précise (rush de Tabaski), objets concrets (mesures, tissu, acompte, date).
- **Actionnable — 3 solutions différentes possibles** :
  1. assistant WhatsApp vocal avec compteur de charge (piste retenue : Kayit) ;
  2. carnet à tickets pré-numérotés + photo WhatsApp de chaque ticket, capacité affichée au mur ;
  3. apprenti « scribe » équipé d'un formulaire simplifié, le patron ne faisant que valider à la voix.
- **Résiste au Chapeau Noir** : N1 (saisie texte) est dans la contrainte, N2 (sur-acceptation) est dans le résultat attendu.

## Validation — les 3 questions du cours

| Question | Réponse |
|---|---|
| Q1 — Contient-il le profil du persona ? | ✅ « tailleurs de quartier de Dakar » |
| Q2 — Peut-on imaginer 3 solutions différentes ? | ✅ voir ci-dessus (vocal / tickets + photo / apprenti scribe) |
| Q3 — Le risque du Chapeau Noir est-il intégré ? | ✅ N1 et N2 |

Critères de la slide 8 : utilisateur réel au Sénégal ✅ · frustration réelle ⚠️ *(observée en interview simulée — à confirmer terrain)* · assez large ✅ · assez précis ✅ · ne contient pas de solution ✅ · non transposable à une autre équipe ✅.

## Ce que ce HMW guide en S3

La fonctionnalité MVP prioritaire est la **commande dictée + relecture + compteur de charge** : toute fonctionnalité qui ne contribue ni à « garder la trace » ni à « n'accepter que le livrable » sort du périmètre S3.
