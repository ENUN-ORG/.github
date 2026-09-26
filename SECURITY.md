# Politique de sécurité

Signaler une faille de façon responsable aide à protéger les utilisateurs de
l'écosystème ENUN. Ce document explique comment.

## Périmètre

Cette politique couvre tous les dépôts de l'organisation `ENUN-ORG` et les
applications déployées dans le cadre de l'université.

Sont concernés : injection SQL, contournement de l'authentification, contournement des
contrôles d'accès, exposition de données personnelles, exécution de code distant,
stockage de mots de passe en clair.

Ne sont pas concernés : les bogues ordinaires et les demandes fonctionnelles, qui
passent par une issue publique.

## Comment signaler

N'ouvrez pas d'issue publique. Une faille publiée est une faille déjà exploitée.

Écrivez en privé à un administrateur en précisant :

1. le dépôt ou l'application concernée
2. la description de la faille et son impact
3. les étapes de reproduction
4. ce que vous avez déjà tenté

Si vous n'avez pas de contact direct, signalez-le via le formulaire d'adhésion en
indiquant qu'il s'agit d'un signalement de sécurité. Un administrateur vous répondra
en privé.

## Ce que nous attendons de vous

- ne pas accéder à des données qui ne vous concernent pas
- ne pas rendre la faille publique avant son correctif
- laisser le temps à la correction
- ne pas perturber le service pendant la vérification

Ces règles ne sont pas négociables pendant un test.

## Ce que nous nous engageons à faire

| Délai | Action |
| --- | --- |
| 72 heures | accusé de réception |
| 7 jours | évaluation de la gravité |
| délai communiqué | correctif ou plan de correction |

Nous vous tiendrons informé de la progression. Si vous le souhaitez, votre nom
apparaîtra dans les remerciements de la correction.

## Versions non maintenues

Seule la branche principale de chaque dépôt reçoit des correctifs de sécurité.
