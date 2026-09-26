# Contribuer à ENUN

Merci de vouloir participer à l'écosystème numérique de l'Université Abdou Moumouni.

Ce document explique comment proposer une modification. Il s'applique à **tous** les
dépôts de l'organisation.

---

## Les trois niveaux

| Niveau | Droits |
| --- | --- |
| `membres` | lecture, ouverture d'issues et de pull requests |
| `moderateurs` | écriture sur les dépôts, développement et modération |
| **2 administrateurs** | gestion des accès, des dépôts et des réglages |

L'adhésion est automatique via [le formulaire](https://github.com/ENUN-ORG/.github/issues/new/choose?template=rejoindre-enun.yml).
Le passage au niveau `moderateur` se demande dans ce même formulaire.

---

## Avant de commencer

1. **Cherchez si le travail existe déjà.** Une issue ou une pull request ouverte peut
   déjà couvrir le sujet.
2. **Ouvrez une issue** pour décrire ce que vous voulez faire, avant d'écrire le code.
   Cela évite de coder quelque chose qui sera refusé, et permet de coordonner avec
   les autres contributeurs.
3. **Une seule modification par pull request.** Mélanger une correction de bug et
   une refonte rend la relecture impossible.

---

## Workflow : fork, branche, pull request

La branche principale de chaque dépôt est protégée : **personne ne pousse
directement dessus**. Le travail se fait par fork.

```bash
# 1. Forker le dépôt depuis l'interface GitHub (bouton Fork), puis :
git clone https://github.com/<votre-pseudo>/<depot>.git
cd <depot>

# 2. Créer une branche dédiée
git checkout -b feat/filtre-par-matiere

# 3. Développer
#    ...vos modifications...

# 4. Vérifier avant de pousser
git add .
git diff --staged

# 5. Pousser la branche
git commit -m "feat: ajoute le filtrage par matiere"
git push origin feat/filtre-par-matiere
```

Puis ouvrez la **pull request** depuis GitHub vers le dépôt de l'organisation.

---

## Conventions de commit

Format : `<type> : <description en minuscules>`

| Type | Usage |
| --- | --- |
| `feat` | nouvelle fonctionnalité |
| `fix` | correction de bug |
| `docs` | documentation uniquement |
| `refactor` | réorganisation sans changement de comportement |
| `test` | ajout ou correction de tests |
| `chore` | outillage, configuration, dépendances |
| `style` | formatage, sans impact logique |

Exemples :

```
feat: ajoute la recherche par mot-clé
fix: corrige le calcul du niveau sur les filières à option
docs: précise les règles de dépôt d'un document
chore: passe la configuration de build en Flutter 3.24
```

---

## Règles de relecture

- **Une approbation** est nécessaire avant fusion. Un modérateur relit.
- Les relecteurs peuvent demander des changements. C'est normal, ce n'est pas un refus.
- Les discussions se font sur la pull request, pas en message privé, pour que la
  décision reste traçable.
- Un auteur ne peut pas approuver sa propre pull request.

---

## Signalement d'un problème

- **Bug ou fonctionnalité** → une issue
- **Faille de sécurité** → ne pas ouvrir d'issue publique, voir [SECURITY.md](SECURITY.md)
- **Comportement inapproprié** → voir [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)

---

## Licence

Le code de l'écosystème est distribué sous **GNU Affero General Public License v3.0**.
Toute contribution Fusionnée dans un dépôt est publiée sous la même licence.
Voir [LICENSE](LICENSE).

---

## Aide

Une question ? [SUPPORT.md](SUPPORT.md)
