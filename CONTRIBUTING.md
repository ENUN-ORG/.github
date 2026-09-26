# Contribuer à ENUN

Ce document décrit les modalités de contribution aux dépôts de l'organisation.

---

## Accès

L'adhésion est ouverte et s'obtient par le
[formulaire d'adhésion](https://github.com/ENUN-ORG/.github/issues/new/choose?template=rejoindre-enun.yml).

| Niveau | Équipe | Périmètre |
| --- | --- | --- |
| Membre | `membres` | consultation, issues, pull requests |
| Modérateur | `moderateurs` | développement, relecture, fusion |

Le niveau de modérateur s'obtient par demande motivée, instruite au regard des
contributions déjà livrées.

---

## Avant de commencer

1. **Vérifier que le sujet n'est pas déjà traité.** Une issue ou une pull request
   ouverte peut le couvrir.
2. **Ouvrir une issue** pour décrire l'intention avant d'écrire le code, afin de
   cadrer le travail et de coordonner avec les autres contributeurs.
3. **Séparer les sujets.** Une pull request qui corrige un défaut et refond un module
   à la fois ne peut pas être relue correctement.

Les idées d'amélioration et les propositions de nouveaux modules sont attendues à tout
stade de maturité, via le
[formulaire de proposition](https://github.com/ENUN-ORG/.github/issues/new/choose?template=proposition.yml).

---

## Cycle de contribution

La branche principale de chaque dépôt est protégée : les contributions passent par
une pull request.

```bash
# 1. Forker le dépôt depuis l'interface GitHub, puis :
git clone https://github.com/<votre-identifiant>/<depot>.git
cd <depot>

# 2. Créer une branche dédiée
git checkout -b feat/filtre-par-matiere

# 3. Développer
#    ...les modifications...

# 4. Relire avant de pousser
git add .
git diff --staged

# 5. Pousser la branche
git commit -m "feat: ajoute le filtrage par matiere"
git push origin feat/filtre-par-matiere
```

Ouvrir ensuite la pull request depuis l'interface GitHub vers le dépôt de
l'organisation. Une approbation est requise avant fusion ; la branche est supprimée
automatiquement après celle-ci.

---

## Conventions de commit

Format : `<type> : <description en minuscules>`

| Type | Usage |
| --- | --- |
| `feat` | nouvelle fonctionnalité |
| `fix` | correction |
| `docs` | documentation |
| `refactor` | réorganisation sans changement de comportement |
| `test` | tests |
| `chore` | outillage, configuration, dépendances |
| `style` | formatage |

Exemples :

```
feat: ajoute la recherche par mot-clé
fix: corrige le calcul du niveau sur les filières à option
docs: précise les conditions de dépôt d'un document
chore: met à jour la configuration de build
```

---

## Relecture

- Une approbation est requise avant fusion.
- La discussion se tient sur la pull request, afin que la décision reste consultable.
- Les demandes de modification font partie du processus normal.

---

## Signalement

| Sujet | Emplacement |
| --- | --- |
| Bug, fonctionnalité | issue publique |
| Amélioration, nouveau module | [formulaire de proposition](https://github.com/ENUN-ORG/.github/issues/new/choose?template=proposition.yml) |
| Faille de sécurité | signalement privé, voir [SECURITY.md](SECURITY.md) |
| Conduite à tenir | signalement privé, voir [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) |

---

## Licence

Le code de l'organisation est distribué sous GNU Affero General Public License v3.0.
Toute contribution fusionnée est publiée sous la même licence. Voir [LICENSE](LICENSE).
