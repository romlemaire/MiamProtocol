# MiamProtocol
Protocole d'échange pour messagerie instantanée permettant de coordonner un départ à la cantine.

## Manifeste
Ce protocole d'échange est conçu avec les recommandations suivantes :

- Parcimonie
  - Pour être efficace, le nombre de caractères requis pour l'émission d'un message doit être le plus faible possible
- Univocité
  - Chaque caractère doit rendre compte de manière non-ambiguë de l'action qu'il décrit
- Centralité
  - Un seul canal de communication est considéré valide pour l'usage de ce protocole, ceci afin de garantir que les messages seront envoyés à tous les participants. Les qualités nécessaires au canal de communication sont les suivantes :
    - *adoption* Seuls les canaux de communication partagés par au moins 90% des récipendaires sont éligibles à devenir canal du protocole
    - *many-to-many* Seuls les canaux de communications permettant l'envoi de messages à un groupe de personnes sont éligibles.
    - *timestamping* Seuls les canaux indicant l'heure d'envoi des messages sont éligibles (ceci permet de rendre optionnels l'heure des événements afin de garantir l'hypothèse de parcimonie)
  - Le canal de communication actuel est réputé être le groupe `Miam` de l'application `WhatsApp`
    - L'inclusion dans ce groupe est subordonnée à une demande à l'un de ses administrateurs.
      - Le nom de ces administrateurs n'est pas révélable publiquement, mais leurs initiales sont R. L. et J.-F. C.

## Commandes:

| Syntaxe           | Explications  |
|:----------------- |:------------- |
| 🔸                | Prêt pour partir, en attente d’un départ. |
| 🔹 [Hx] hh:mm / N | Départ effectif, heure et nombre de personnes. Destination optionnelle, H1 la plupart du temps. |
| 🔚 hh:mm          | Confirmation d’arrivée à destination. |
| 🔻                | Absent ou ne participant pas au repas collectif. |
| 🔜                |Présent mais départ différé ou indépendant. Déplacement à la destination de manière autonome. Place à réserver. |

## Destinations repertoriées:
- H1
- H2
- H3 (très rarement utilisée)
- Le Carré (🔲)
- Cousin Jojo (🐰)
