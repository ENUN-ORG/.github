# Politique de sécurité

Ce document explique comment signaler une faille de sécurité de manière responsable.

---

## Périmètre

Cette politique s'applique à l'ensemble des dépôts de l'organisation et aux
applications déployées dans le cadre des universités.

Sont concernés : injection de code, contournement de l'authentification, contournement
des contrôles d'accès, exposition de données personnelles ou de documents restreints,
exécution de code à distance, stockage de mots de passe en clair.

N'est pas concerné : le signalement d'anomalies fonctionnelles ordinaires, qui passe
par une issue publique.

---

## Signalement

Une faille publiée est une faille déjà exploitable. Le signalement se fait donc par
message privé adressé à l'administration, en indiquant :

1. le dépôt ou l'application concernée
2. la description de la faille et son impact
3. les étapes de reproduction
4. les vérifications déjà effectuées

À défaut de contact direct, le
[formulaire d'adhésion](https://github.com/ENUN-ORG/.github/issues/new/choose?template=rejoindre-enun.md)
peut servir de point d'entrée en indiquant qu'il s'agit d'un signalement de sécurité.

---

## Conduite attendue

Pendant la vérification d'un signalement :

- ne pas accéder à des données sans rapport avec la faille ;
- ne pas rendre la faille publique avant la publication du correctif ;
- laisser le temps nécessaire au traitement ;
- ne pas perturber le fonctionnement du service.

Ces règles s'appliquent pendant toute la durée de la vérification.

---

## Traitement

| Étape | Engagement |
| --- | --- |
| Accusé de réception | sous 72 heures |
| Évaluation de la gravité | sous 7 jours |
| Correctif ou plan d'action | délai communiqué à la personne signalante |

La personne à l'origine du signalement est informée de la suite donnée. Si elle le
souhaite, sa contribution apparaît dans les remerciements associés au correctif.

---

## Versions

Seule la branche principale de chaque dépôt reçoit les correctifs de sécurité.
