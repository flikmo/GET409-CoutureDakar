# Value Proposition Canvas — CoutureDakar

> **GET 409 — Lab Sprint S2 — Outil 2/3** · Construit à partir de [chapeaux-bono.md](chapeaux-bono.md) (règles de correspondance du cours : Blanc → Jobs · Rouge → Pains émotionnels · Noir → Pains fonctionnels + Pain Relievers · Jaune → Gains + Gain Creators · Vert → Produits & Services · Bleu → FIT Check).
> Chaque élément porte son chapeau d'origine. Tout élément sans origine est marqué **[Non tracé — à valider]**.
> Statut des données : hypothèses S1 (interview simulée) — **à confirmer par 2 interviews terrain avant S3**.

## HMW Définitif

« Comment pourrions-nous aider les tailleurs de quartier de Dakar à garder la trace de chaque commande — mesures, tissu, acompte, date promise — **sans avoir à écrire**, pendant le rush de Tabaski, afin qu'ils **n'acceptent que ce qu'ils peuvent livrer à temps** ? » → voir [hmw-definitif.md](hmw-definitif.md)

---

## 👤 Profil Client — Ousmane, 41 ans, tailleur-patron, Médina (Dakar)

*Android d'entrée de gamme · WhatsApp vocal · Wave / Orange Money · 3 apprentis + 1 brodeur · tape très peu de texte*

### 🔧 Jobs To Be Done

| # | Job | Type | Origine |
|---|---|---|---|
| JB1 | Enregistrer chaque commande (client, modèle, tissu, mesures) au moment où le client dépose son tissu | Fonctionnel | Blanc B1 |
| JB2 | Livrer toutes les tenues promises **avant le jour de la fête** | Fonctionnel | Blanc B2 |
| JB3 | Encaisser les acomptes et savoir, à tout moment, qui a payé combien | Fonctionnel | Blanc B3 |
| JB4 | Rester « l'atelier sérieux » du quartier, celui à qui on confie ses tenues de fête | Social / émotionnel | Rouge R1 |
| JB5 | Répartir le travail entre les apprentis selon les dates promises | Fonctionnel | **[Non tracé — à valider]** |

### 😣 Pains (classés par intensité)

| # | Pain | Intensité | Nature | Origine |
|---|---|---|---|---|
| P1 | Perd la trace des commandes (mesures, tissu, acompte, date) quand le volume explose | ★★★ | Fonctionnel | Blanc B1 · Noir N1 |
| P2 | Promet des dates sans connaître sa charge réelle → retards en cascade | ★★★ | Fonctionnel | Noir N2 · Rouge R2 |
| P3 | Les outils existants exigent de taper du texte en français, les mains occupées | ★★★ | Fonctionnel | Noir N1 |
| P4 | Peur de perdre la face le jour de la fête | ★★★ | Émotionnel | Rouge R1 |
| P5 | Litiges sur les acomptes, sans preuve d'un côté comme de l'autre | ★★ | Fonctionnel | Blanc B1 · Blanc B3 |
| P6 | Relances téléphoniques incessantes qui interrompent la couture | ★★ | Émotionnel | Rouge R3 |

### 🌟 Gains (classés selon le modèle requis / attendu / désiré / inattendu)

| # | Gain | Niveau | Origine |
|---|---|---|---|
| G1 | Toutes les commandes acceptées sont livrées à la date promise | Requis | Jaune J1 |
| G2 | Des acomptes traçables : zéro litige et une trésorerie visible avant d'acheter les fournitures | Attendu | Jaune J2 |
| G3 | Des heures de couture récupérées grâce à moins d'appels | Désiré | Jaune J3 |
| G4 | Des clients fidèles qui reviennent à chaque fête et recommandent l'atelier | Désiré | Jaune J1 |
| G5 | Pouvoir dire « complet » ou proposer une date réaliste **sans perdre la face** | Inattendu | Vert V3 · Rouge R2 |

---

## 💡 Proposition de Valeur — **Kayit**, le carnet de commandes vocal du tailleur

*Kayit (« papier » en wolof) est un assistant WhatsApp : le tailleur dicte la commande en vocal, reçoit une fiche numérotée à confirmer, et l'assistant tient à jour la charge de l'atelier jusqu'à la fête. Aucune application à installer, aucune saisie de texte.*

### 📦 Produits & Services (périmètre MVP)

| # | Fonctionnalité | Description | Origine |
|---|---|---|---|
| PS1 | **Commande dictée** | Un vocal WhatsApp (wolof / français mélangés) → fiche structurée : client, téléphone, modèle, tissu, mesures, acompte + moyen de paiement, date promise | Vert V1 |
| PS2 | **Numéro de ticket** | Chaque fiche reçoit un numéro court (ex. `T-047`) que l'apprenti écrit sur le sachet de tissu | Vert V2 |
| PS3 | **Relecture obligatoire** | La fiche est relue au tailleur ; elle n'est enregistrée qu'après « waaw » (oui). « Déedéet » (non) → correction vocale | Bleu Bl3 |
| PS4 | **Compteur de charge** | Capacité déclarée de l'atelier (tenues / jour) × jours restants avant la fête ; alerte « il reste X places », puis « complet », et propose la prochaine date tenable | Vert V3 · Bleu Bl2 |
| PS5 | **Messages client automatiques** | Reçu d'acompte envoyé au client dès la fiche validée ; message « votre tenue T-047 est prête » quand le tailleur le dicte | Vert V3 |

### 💊 Pain Relievers

| Pain | Pain Reliever | Fonctionnalité | Origine |
|---|---|---|---|
| P1 — perte de traçabilité | Chaque commande devient une fiche unique, retrouvable par numéro ou par nom ; le sachet de tissu porte le même numéro | PS1 · PS2 | Noir N1 → Vert V1/V2 |
| P2 — sur-promesse | L'assistant connaît la charge et refuse de confirmer une date intenable ; il propose la première date réaliste | PS4 | Noir N2 → Bleu Bl2 |
| P3 — saisie texte impossible | Entrée 100 % vocale, validation par un mot ; aucun menu, aucun formulaire | PS1 · PS3 | Noir N1 → Bleu Bl1 |
| P4 — peur de perdre la face | Les promesses faites sont tenables (PS4) et le client est informé proactivement (PS5) : l'échec public devient rare | PS4 · PS5 | Rouge R1 |
| P5 — litiges d'acompte | Le client reçoit un reçu horodaté avec le montant et le moyen de paiement : la preuve est partagée | PS5 | Jaune J2 (inverse) |
| P6 — relances incessantes | Le client est prévenu quand sa tenue est prête ; il n'a plus besoin d'appeler pour savoir | PS5 | Rouge R3 |

### 🎁 Gain Creators

| Gain | Gain Creator | Fonctionnalité | Origine |
|---|---|---|---|
| G1 — livrer à la date promise | Seules des dates compatibles avec la capacité sont promises ; la liste des livraisons du lendemain est lisible d'un coup d'œil | PS4 · PS1 | Jaune J1 · Bleu Bl2 |
| G2 — acomptes traçables | Chaque fiche porte l'acompte et son moyen de paiement ; le total est consultable en demandant « acomptes aujourd'hui » | PS1 · PS5 | Jaune J2 |
| G3 — heures récupérées | Moins d'appels entrants grâce aux messages proactifs | PS5 | Jaune J3 |
| G4 — clients fidèles | Expérience « atelier moderne » (reçu, notification) comparable aux ateliers Instagram cités par les clientes | PS5 | Jaune J1 · [S1 — Entend] |
| G5 — dire « complet » sans perdre la face | Message de refus poli et prêt à envoyer, avec date alternative : c'est l'outil qui dit non, pas le tailleur | PS4 | Vert V3 · Rouge R2 |

---

## ✅ FIT Check

**Matrice de couverture**

| | PS1 | PS2 | PS3 | PS4 | PS5 |
|---|:-:|:-:|:-:|:-:|:-:|
| P1 | ● | ● | | | |
| P2 | | | | ● | |
| P3 | ● | | ● | | |
| P4 | | | | ● | ● |
| P5 | | | | | ● |
| P6 | | | | | ● |
| G1 | ● | | | ● | |
| G2 | ● | | | | ● |
| G3 | | | | | ● |
| G4 | | | | | ● |
| G5 | | | | ● | |

**Combinaison synergique retenue (Chapeau Bleu) :** Bl1 + Bl2 + Bl3 → *commande dictée + relecture + compteur de charge* : c'est le cœur du MVP ; PS5 est la couche de valeur côté client.
**Pains sans Pain Reliever :** aucun — les 6 pains sont couverts.
**Pain Relievers sans Pain :** **PS3 (relecture)** ne répond à aucun pain *client* : c'est un garde-fou contre un risque *de la solution* (Noir N3 — transcription wolof non fiable). Conservé comme **contrainte qualité**, pas comme bénéfice vendu.
**Éléments non tracés :** JB5 (répartition du travail entre apprentis) → non couvert par le MVP, **à valider en interview S3** avant tout ajout.
**Conclusion :** FIT **fort sur le papier** (6/6 pains, 5/5 gains couverts, 0 fonctionnalité superflue), mais **conditionnel** : il repose sur deux hypothèses critiques non encore observées sur le terrain (ci-dessous).

---

## ⚠️ Hypothèses critiques à valider avant S3

| # | Hypothèse | Si elle est fausse… | Test le plus rapide |
|---|---|---|---|
| HC1 | Le tailleur (ou son apprenti) accepte de dicter chaque commande en vocal au moment du dépôt | PS1 s'effondre → revenir à la photo de la page du cahier | 2 interviews + test « dictez-moi votre dernière commande » |
| HC2 | Une transcription wolof/français est assez fiable pour extraire nom, montant et date | PS3 devient une corvée → saisie par l'apprenti ou menu vocal à choix | Tester 10 vocaux réels dans Dify en S3 |
| HC3 | L'atelier sait estimer sa capacité (tenues par jour) | PS4 donne de fausses alertes | Demander en interview : « combien de grands boubous pouvez-vous finir en une journée ? » |
| HC4 | Les clients acceptent de recevoir des messages WhatsApp de l'atelier | PS5 perçu comme intrusif | Demander le consentement au dépôt du tissu (note éthique) |

## Hors MVP (roadmap post-S6)

- Prise de mesures par photo / IA → trop risqué, hors HMW.
- Paiement intégré → Wave / Orange Money suffisent ; le MVP *trace*, il n'*encaisse* pas.
- Catalogue de modèles, gestion du stock de tissus → ne répondent à aucun pain prioritaire.
- Planning par apprenti (JB5) → en attente de validation terrain.

## Note éthique (Responsable Impact)

Kayit stocke des numéros de téléphone et des mesures corporelles de clients : collecte minimale, consentement explicite au dépôt du tissu, suppression des fiches après livraison + délai de réclamation. Cadre applicable au Sénégal : loi n° 2008-12 sur la protection des données à caractère personnel (CDP) **[CG — à vérifier]**.
