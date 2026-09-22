# 6 Chapeaux de Bono — CoutureDakar

> **GET 409 — Lab Sprint S2 — Outil 1/3** · Facilitateur : Chef de Produit · Scribe : Master Prompt Engineer (même personne — équipe à membre unique)
> **Légende des sources** : **[S1]** = carte d'empathie S1 (interview simulée, hypothèse) · **[CG]** = connaissance générale du contexte dakarois, non sourcée — à confirmer · **[É]** = analyse de l'équipe.

## HMW analysé

« Comment pourrions-nous aider les tailleurs de quartier à Dakar à suivre chaque commande — mesures, tissu, acompte, date promise — pendant le rush de Tabaski, afin de livrer à temps sans perdre la confiance de leurs clients ? » *(HMW draft S1, validé)*

## 🤍 Chapeau Blanc — Faits & Données

- **B1** — Le suivi des commandes repose sur un cahier papier (mesures), des sachets de tissu étiquetés au marqueur et la mémoire du patron pour les acomptes. **[S1]**
- **B2** — La demande se concentre sur quelques semaines avant Tabaski et Korité ; c'est la période où l'atelier accepte le plus de commandes et où les retards se produisent. **[S1][CG]**
- **B3** — Le tailleur utilise un smartphone Android d'entrée de gamme, surtout WhatsApp en messages vocaux, et reçoit une partie des acomptes par Wave / Orange Money ; il tape très peu de texte. **[S1]**

## ❤️ Chapeau Rouge — Émotions & Intuitions

- **R1** — Peur de « perdre la face » : une tenue non livrée le jour de la fête est vécue comme une humiliation publique et la perte définitive du client. **[S1]**
- **R2** — Culpabilité et pression à dire « oui » : refuser une commande, c'est laisser l'argent de la saison au concurrent. **[S1]**
- **R3** — Irritation et épuisement face aux relances : chaque appel « c'est prêt ? » interrompt la couture et rappelle l'échec possible. **[S1]**

## 🖤 Chapeau Noir — Risques & Critique

- **N1** — **Saisie impossible dans le rush** : tout outil qui exige de taper du texte (ou de lire des menus en français) sera abandonné dès la première semaine chargée. Les mains sont occupées, l'écran est petit. **[S1][É]**
- **N2** — **Sur-acceptation non détectée** : même avec un registre parfait, si l'atelier n'a aucune vision de sa capacité restante avant la fête, il continuera à promettre des dates intenables. Le suivi seul ne suffit pas. **[É]**
- **N3** — **Reconnaissance vocale en wolof peu fiable** : un message vocal mal transcrit (nom du client, montant de l'acompte) crée une fausse commande — pire que le cahier papier. **[CG][É]**

## 💛 Chapeau Jaune — Optimisme & Valeur

- **J1** — Chaque commande livrée à temps protège le client le plus précieux : celui qui revient à chaque fête et recommande l'atelier dans son quartier. **[S1]**
- **J2** — Un acompte tracé (montant, date, moyen de paiement) supprime les litiges et donne au patron une vision de sa trésorerie avant d'acheter fils, boutons et broderies. **[S1][É]**
- **J3** — Moins de relances entrantes = heures de couture récupérées au moment exact où elles valent le plus. **[S1][É]**

## 💚 Chapeau Vert — Créativité & Idées

- **V1** — Et si la commande se dictait en un message vocal WhatsApp (« Awa Ndiaye, grand boubou, bazin bleu, acompte 10 000 Wave, pour le 12 ») et revenait sous forme de **fiche numérotée** ? **[É]**
- **V2** — Et si ce numéro de fiche était écrit sur le sachet de tissu, reliant enfin l'objet physique au registre ? **[É]**
- **V3** — Et si l'outil **disait « complet »** : un compteur de charge qui prévient quand l'atelier ne peut plus livrer avant la fête, et le client recevait automatiquement un reçu d'acompte puis un message « votre tenue est prête » ? **[É]**

## 💙 Chapeau Bleu — Processus & Organisation

- **Bl1** — Priorité de conception : **zéro saisie texte** pour le tailleur (entrée vocale ou photo, confirmation par « waaw »/« déedéet »). Tout ce qui viole N1 sort du MVP.
- **Bl2** — Le MVP doit coupler **enregistrement** (N1) et **capacité** (N2) : suivre sans limiter ne résout pas le retard.
- **Bl3** — Garde-fou N3 : toute fiche générée depuis un vocal est **relue au tailleur** (vocal ou texte court) et n'est validée qu'après confirmation.

## 🔵 Synthèse Chapeau Bleu

**HMW révisé :** le draft S1 est confirmé sur le fond ; il doit intégrer la contrainte « sans avoir à écrire » (N1) et l'objectif « n'accepter que ce qui peut être livré » (N2) → voir [hmw-definitif.md](hmw-definitif.md).
**Risques prioritaires :** N1 — saisie texte impossible dans le rush / N2 — sur-acceptation non détectée.
**Question ouverte :** qui tient réellement le registre dans l'atelier — le patron ou l'apprenti le plus lettré ? *(à vérifier en interview terrain avant S3)*
