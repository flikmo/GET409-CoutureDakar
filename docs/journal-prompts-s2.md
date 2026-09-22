# Journal de Prompts — Séance 2

> **GET 409 — Équipe CoutureDakar** — Master Prompt Engineer : Malick Faye Diagne
> Format imposé (slide 14) : technique · prompt exact · résumé de la réponse · note /5 · itération si < 3/5 (ou si amélioration utile).
> **Transparence** : prompts exécutés avec Claude ; résumés et notes proposés par l'assistant IA — **notes à confirmer par l'étudiant** après relecture.

## Synthèse

| # | Technique | Objet | Note v1 | Itération | Note finale |
|---|---|---|:-:|:-:|:-:|
| P1 | Zero-Shot structuré | 3 problèmes du persona | 3/5 | oui | 4/5 |
| P2 | Zero-Shot formaté | 5 fonctionnalités MVP | 4/5 | non | 4/5 |
| P3 | Few-Shot | Situation → solution atelier | 5/5 | non | 5/5 |
| P4 | Chain-of-Thought | Cause → obstacle → solution → métrique | 4/5 | non | 4/5 |
| P5 | Libre — jeu de rôle | Acceptabilité du message « complet » | 3/5 | oui | 4/5 |

---

## P1 — Zero-Shot structuré

**Prompt v1**
```
Tu es consultant en organisation d'ateliers artisanaux à Dakar.
Contexte : un tailleur-patron de la Médina, avec 3 apprentis, reçoit beaucoup
plus de commandes que d'habitude pendant les 3 semaines avant Tabaski.
Tâche : identifie les 3 principaux problèmes qu'il rencontre pendant cette période.
Format : tableau | Problème | Cause | Impact | Piste numérique |
```
**Réponse (résumé)** : 1) surcharge et retards de livraison ; 2) perte d'informations (mesures, tissus) dans un cahier papier ; 3) tensions de trésorerie et litiges d'acomptes. Pistes proposées : application de gestion d'atelier, agenda partagé, tableur de suivi.
**Note : 3/5** — diagnostic juste, mais les pistes supposent toutes une **saisie texte**, incompatible avec le persona (Chapeau Noir N1).

**Prompt v2 (itération)** — ajout au contexte :
```
Il utilise un smartphone Android d'entrée de gamme, surtout WhatsApp en messages
vocaux, tape très peu de texte et travaille les mains occupées.
Les pistes numériques doivent respecter cette contrainte.
```
**Réponse (résumé)** : mêmes 3 problèmes ; pistes devenues : commande dictée par vocal WhatsApp, étiquette numérotée sur le sachet, reçu d'acompte automatique.
**Note : 4/5** — pistes ancrées dans le terrain ; il manque encore la question de la **capacité** de l'atelier (apportée en P3/P4).

---

## P2 — Zero-Shot formaté

**Prompt**
```
Tu es product manager spécialisé en outils no-code pour artisans en Afrique de l'Ouest.
Notre persona : Ousmane, 41 ans, tailleur-patron à la Médina (Dakar), WhatsApp vocal, tape peu.
Notre problème : pendant le rush de Tabaski, il perd la trace de ses commandes
et promet des dates qu'il ne peut pas tenir.
Propose 5 idées de fonctionnalités pour un MVP.
Format STRICT, sans introduction :
| Fonctionnalité | Pain adressé | Faisable en no-code (Dify / Bolt) ? | Effort (faible/moyen/élevé) |
```
**Réponse (résumé)** : 1) commande dictée → fiche structurée ; 2) numéro de ticket ; 3) compteur de places restantes avant la fête ; 4) notification « tenue prête » au client ; 5) récapitulatif vocal du soir (commandes, acomptes, livraisons du lendemain). Toutes jugées faisables avec Dify + WhatsApp, effort faible à moyen.
**Note : 4/5** — les 4 premières alimentent directement le VPC (PS1, PS2, PS4, PS5). La 5ᵉ (récap du soir) **n'est tracée à aucun pain prioritaire** → écartée du MVP (principe FIT).

---

## P3 — Few-Shot métier

**Prompt**
```
Tu es consultant en organisation d'ateliers de couture à Dakar.
Voici des situations réelles d'atelier et leurs solutions :

SITUATION : Un client conteste le montant de l'acompte qu'il a versé.
SOLUTION : Envoyer au client, dès le dépôt, un reçu horodaté avec le montant
et le moyen de paiement (espèces / Wave / Orange Money).

SITUATION : Deux clientes nommées Awa ont déposé des tissus similaires ;
les sachets sont confondus.
SOLUTION : Attribuer un numéro de ticket unique à chaque commande et l'écrire
sur le sachet ; la fiche est retrouvée par numéro, pas par prénom.

En suivant exactement le même raisonnement, propose une solution :
SITUATION : À 10 jours de Tabaski, le tailleur accepte une nouvelle commande
alors que l'atelier est déjà plein.
SOLUTION :
Contraintes : le tailleur tape très peu de texte ; il ne veut pas perdre le client.
```
**Réponse (résumé)** : « Tenir un compteur de capacité (tenues par jour × jours restants) ; quand il est atteint, envoyer au client un message poli proposant la première date réaliste après la fête ou une inscription en liste d'attente — c'est l'outil qui dit non, pas le tailleur. »
**Note : 5/5** — format imité parfaitement (une solution courte et opérationnelle), contraintes respectées, et l'idée « c'est l'outil qui dit non » a donné le Gain Creator G5 du VPC.

---

## P4 — Chain-of-Thought

**Prompt**
```
Tu es expert en transformation numérique des TPE artisanales en Afrique de l'Ouest.
Problème : les tailleurs de quartier de Dakar livrent en retard pendant le rush
de Tabaski, faute de suivi des commandes et de visibilité sur leur charge.
Analyse ce problème étape par étape. Développe chaque étape avant de passer à la suivante.
Étape 1 — Cause principale dans le contexte d'un atelier de la Médina.
Étape 2 — Obstacle qui empêche une solution classique (logiciel de gestion) de fonctionner.
Étape 3 — Solution technologique accessible à un tailleur qui tape peu.
Étape 4 — Un indicateur de succès mesurable à 30 jours, sans technologie complexe.
```
**Réponse (résumé)** : Étape 1 — pas de registre unique + saisonnalité extrême : la demande arrive en quelques semaines. Étape 2 — saisie texte, littératie numérique en français, absence de temps pendant le rush, coût des licences. Étape 3 — assistant WhatsApp vocal qui structure la commande et suit la capacité. Étape 4 — « part des commandes livrées à la date promise », mesurée par comparaison fiche / date de retrait.
**Note : 4/5** — raisonnement structuré et vérifiable à chaque étape, sans chiffre inventé. Point faible : l'étape 2 reste générique (« coût des licences ») et n'exploite pas le facteur le plus spécifique du terrain — le temps disponible pendant le rush. **Garde-fou appliqué** : toute donnée chiffrée proposée par l'IA est traitée comme hypothèse à mesurer, jamais comme fait.

---

## P5 — Prompt libre (jeu de rôle persona)

**Prompt v1**
```
Joue le rôle d'Ousmane, 41 ans, tailleur-patron à la Médina, à 10 jours de Tabaski.
Ton assistant WhatsApp te propose d'envoyer ce message à une cliente :
"Désolé, l'atelier est complet avant Tabaski."
Réagis honnêtement : l'enverrais-tu ? Pourquoi ?
```
**Réponse (résumé)** : Ousmane refuse de l'envoyer : trop sec, il a peur de perdre la cliente pour les fêtes suivantes ; il préférerait proposer une date ou une priorité pour la prochaine fête.
**Note : 3/5** — utile pour révéler un frein d'acceptabilité, mais une simulation IA **ne remplace pas** un tailleur réel (risque de projeter nos propres hypothèses).

**Prompt v2 (itération)**
```
Propose 3 formulations de ce message, en français simple et en wolof,
qui proposent une alternative (date après la fête, liste d'attente, priorité à la Korité)
et préservent la relation avec la cliente. 2 phrases maximum chacune.
```
**Réponse (résumé)** — 3 formulations en français :
1. « Awa, l'atelier est plein jusqu'à Tabaski. Je peux vous livrer le [date], et vous serez prioritaire pour la Korité. »
2. « Pour Tabaski nous sommes complets, mais je vous inscris en tête de liste : si une place se libère, je vous appelle. »
3. « Je préfère vous dire la vérité : avant la fête, je ne pourrai pas bien faire votre tenue. Je vous propose le [date]. »

Formulation **n° 1 retenue** pour le MVP (date + priorité = la relation est préservée).
**Note : 4/5** — directement exploitable dans PS4. Les versions wolof proposées par l'IA ne sont **pas reprises** ici : elles doivent être rédigées ou relues par un locuteur natif avant usage.

---

## Annexe — Prompts de production des livrables S2

| Livrable | Prompt du cours utilisé | Adaptation |
|---|---|---|
| [chapeaux-bono.md](chapeaux-bono.md) | P-Chapeau (promptChapeauEtu) | Sources marquées [S1] / [CG] / [É] pour distinguer hypothèses et faits |
| [vpc.md](vpc.md) | P-VPC depuis les 6 Chapeaux (promptVPCEtu) + P-VPC-1 / P-VPC-2 | Ajout d'une matrice de couverture FIT et d'une section hypothèses critiques |
| [hmw-definitif.md](hmw-definitif.md) | P-HMW (P-HMWEtu) | Ajout du tableau « ce qui a changé » draft S1 → définitif S2 |
