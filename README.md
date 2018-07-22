# Node.js [![Build Linux][ci-linux]](https://travis-ci.org/oncletom/nodebook) [![Build Windows][ci-windows]](https://ci.appveyor.com/project/oncletom/nodebook) [![Backers on Open Collective](https://opencollective.com/nodebook/backers/badge.svg)][backers] [![Sponsors on Open Collective](https://opencollective.com/nodebook/sponsors/badge.svg)][sponsors]

> Apprendre par l'exemple • Devenez autonome avec JavaScript, l'écosystème npm, le développement frontend, les applications web et en ligne de commande.

📖 **Journal de bord d'écriture** • [2018][journal-2018] • [2017][journal-2017].<br>
👀 **Lire l'ouvrage** • [sur papier](#sur-papier) • [sur le web](#sur-le-web) • [avec Node.js](#avec-nodejs).<br>
🎧 [Ce que j'écoute en boucle quand j'écris][playlist].


# Table des matières

**Légende** • 🚧 = pas fini • ✍️ = en cours d'écriture • ✅ = terminé.

| Statut | Chapitre                  | Objectif d'apprentissage | |
| -------|---------------------------|--------- |---|
| ✅      | **[Avant-propos][preamble]** | _pourquoi tu écris cet ouvrage ?_ | -
| ✅      | **[Histoire, écosystème et gouvernance][ch01]** | _ça marche comment la vie de Node et des gens qui le font ?_ | [issues][ch01-issues]
| ✅      | **[Installer, mettre à jour et développer][ch02]** | _ça marche comment Node sur une machine ?_ | [issues][ch02-issues]
| ✅      | **[Jouer avec JavaScript][ch03]** | _ça marche comment JavaScript ?_ | [issues][ch03-issues]
| ✅      | **[Jouer avec Node.js][ch04]** | _ça marche comment les modules ?_ | [issues][ch04-issues]
| ✅      | **[Jouer avec npm][ch05]** | _ça marche comment l'outil npm ?_ | [issues][ch05-issues]
| ✅      | **[Déployer notre code][ch06]** | _ça marche comment côté hosting ?_ | [issues][ch06-issues]
| ✅      | **[Créer une application web][ch07]** |  _ça marche comment HTTP ?_ | [issues][ch07-issues]
| ✅      | **[Créer un outil en ligne de commande][ch08]** | _ça marche comment du code métier dans le terminal ?_ | [issues][ch08-issues]
| ✅      | **[Créer une application frontend][ch09]** | _ça marche comment les modules Node dans les navigateurs web ?_ | [issues][ch09-issues]
| ✅      | Annexe : **[Sélection de modules npm][a01]** | _quel(s) module(s) npm choisir ou découvrir ?_ | [issues][appendix-issues]

# Lire l'ouvrage

## Sur le web

🌐 L’épreuve est consultable gratuitement à cette adresse : [https://oncletom.io/node.js/][livre-web].<br>

**Fonctionnalités** : exemples interactifs, vidéos, mise à jour en continu.

## Sur papier

⏳ À venir.

**Fonctionnalités** : confort de lecture, annotations libres, rémunère mon travail.

## Sur liseuse numérique

⏳ À venir.

**Fonctionnalités** : ne prend pas de place, rémunère mon travail.

## Avec Node.js

📦 Le livre est disponible en tant que **module npm** : [`nodebook`][livre-npm].

**Fonctionnalités** : apprendre Node.js avec Node.js, tous les exemples sont fonctionnels, lecture hors-ligne.

```bash
$ npm install --global nodebook
$ nodebook install all
```

Cette commande télécharge une copie du livre et les dépendances des exemples pour une utilisation hors-ligne.

Le manuel d'utilisation s'invoque avec l'argument `--help` :

```bash
$ nodebook --help

Commandes:
  nodebook chapters               Liste les chapitres de l'ouvrage.
  nodebook dir <chapter>          Affiche le chemin vers un chapitre.
  nodebook install <chapter|all>  Installe les dépendances d'un chapitre.
  nodebook read                   Démarre la lecture du livre au format HTML

Options:
  --version  Affiche le numéro de version                              [booléen]
  --help     Affiche de l'aide                                         [booléen]

Exemples:
  nodebook install chapter-04               Installe les dépendances du chapitre
                                            4
  nodebook install all                      Installe les dépendances de tous les
                                            chapitres
  cd $(nodebook dir chapter-04)             Place le terminal dans le répertoire
                                            d'exemples du chapitre 4
  cd $(nodebook dir chapter-04 --root)      Place le terminal dans le répertoire
                                            racine du chapitre 4
```

# Contribuer

Je vous invite à contribuer **de la manière de votre choix** — par e-mail, en ouvrant une _issue_ ou en contribuant du texte ou du code.

Si vous n'êtes pas sûr·e de votre coup mais que l'envie est là, c'est suffisant pour démarrer 🙂. Nous éclaircirons les choses ensemble si nécessaire.

## Installation

Il est possible de travailler sur une copie locale de l'épreuve en la dupliquant avec Git.

```bash
$ git clone --single-branch https:/github.com/oncletom/nodebok
$ cd nodebook
# Installe les dépendances de développement
$ npm ci
# Installe les dépendances des chapitres
$ npm run install:all
```

Cette commande facultative récupère les vidéos localement :

```bash
$ git lfs pull
```

Elle utilise l'extension [git-lfs](https://git-lfs.github.com/).

## Prévisualiser

Un serveur local est disponible pour prévisualiser les modifications sans être connecté à Internet.

```bash
$ npm start
```

L'épreuve est accessible sur [http://localhost:3000](http://localhost:3000).

## Tests

La bonne santé des exemples est vérifiée à l'aide d'[ESLint](http://eslint.org/) et de [tape-spawn](https://npmjs.com/tape-spawn).

```bash
$ npm test
```

## Génération des épreuves

### HTML

```bash
$ make build-html
$ open ./dist
```

### DocBook

```bash
$ make build-docbook
$ soffice ./dist/book.xml
```

### OpenDocument

```bash
$ make build-odt
$ soffice ./dist/book.fodt
```


## Contributrices et Contributeurs

Merci à vous pour avoir contribué à l'ouvrage grâce à vos relectures, corrections et demandes de clarification.

[![](https://opencollective.com/nodebook/contributors.svg?width=890&button=false)][contributors]

<!--
## Backers

Thank you to all our backers! 🙏 [[Become a backer](https://opencollective.com/nodebook#backer)]

<a href="https://opencollective.com/nodebook#backers" target="_blank"><img src="https://opencollective.com/nodebook/backers.svg?width=890"></a>


## Sponsors

Support this project by becoming a sponsor. Your logo will show up here with a link to your website. [[Become a sponsor](https://opencollective.com/nodebook#sponsor)]

<a href="https://opencollective.com/nodebook/sponsor/0/website" target="_blank"><img src="https://opencollective.com/nodebook/sponsor/0/avatar.svg"></a>
<a href="https://opencollective.com/nodebook/sponsor/1/website" target="_blank"><img src="https://opencollective.com/nodebook/sponsor/1/avatar.svg"></a>
<a href="https://opencollective.com/nodebook/sponsor/2/website" target="_blank"><img src="https://opencollective.com/nodebook/sponsor/2/avatar.svg"></a>
<a href="https://opencollective.com/nodebook/sponsor/3/website" target="_blank"><img src="https://opencollective.com/nodebook/sponsor/3/avatar.svg"></a>
<a href="https://opencollective.com/nodebook/sponsor/4/website" target="_blank"><img src="https://opencollective.com/nodebook/sponsor/4/avatar.svg"></a>
<a href="https://opencollective.com/nodebook/sponsor/5/website" target="_blank"><img src="https://opencollective.com/nodebook/sponsor/5/avatar.svg"></a>
<a href="https://opencollective.com/nodebook/sponsor/6/website" target="_blank"><img src="https://opencollective.com/nodebook/sponsor/6/avatar.svg"></a>
<a href="https://opencollective.com/nodebook/sponsor/7/website" target="_blank"><img src="https://opencollective.com/nodebook/sponsor/7/avatar.svg"></a>
<a href="https://opencollective.com/nodebook/sponsor/8/website" target="_blank"><img src="https://opencollective.com/nodebook/sponsor/8/avatar.svg"></a>
<a href="https://opencollective.com/nodebook/sponsor/9/website" target="_blank"><img src="https://opencollective.com/nodebook/sponsor/9/avatar.svg"></a>
-->

# Mentions légales

_Node.js • Apprendre par la pratique_ est un ouvrage rédigé par [Thomas Parisot](https://oncletom.io). Il est édité, publié et distribué en papier et e-book par [Eyrolles][].

L’épreuve est soumise à la licence [Creative Commons NC-BY-SA 4.0][cc-nc-by-sa] (_Attribution, Non-Commercial, Share Alike_).<br>
Les exemples de code sont placés sous la [licence MIT][].

[ci-linux]: https://travis-ci.org/oncletom/nodebook.svg?branch=master
[ci-windows]: https://ci.appveyor.com/api/projects/status/crewvvqeybl8f16c?svg=true&amp;branch=master
[journal-2018]: docs/JOURNAL.md
[journal-2017]: docs/JOURNAL-2017.md
[livre-web]: https://oncletom.io/node.js/
[livre-npm]: https://npmjs.com/nodebook
[Eyrolles]: http://www.eyrolles.fr
[playlist]: https://open.spotify.com/user/oncletom/playlist/4Ywqaz0XpFVNa5CKohuUN8?si=edpuGs_NRgapHyigrrwU3w
[licence MIT]: LICENSE
[cc-nc-by-sa]: https://creativecommons.org/licenses/by-nc-sa/4.0/deed.fr
[backers]: https://opencollective.com/nodebook#backers
[sponsors]: https://opencollective.com/nodebook#sponsor
[contributors]: https://github.com/oncletom/nodebook/graphs/contributors
[preamble]: foreword/preamble.adoc
[ch01]: chapter-01/index.adoc
[ch01-issues]: https://github.com/oncletom/nodebook/labels/:book:%20chapitre:1
[ch02]: chapter-02/index.adoc
[ch02-issues]: https://github.com/oncletom/nodebook/labels/:book:%20chapitre:2
[ch03]: chapter-03/index.adoc
[ch03-issues]: https://github.com/oncletom/nodebook/labels/:book:%20chapitre:3
[ch04]: chapter-04/index.adoc
[ch04-issues]: https://github.com/oncletom/nodebook/labels/:book:%20chapitre:4
[ch05]: chapter-05/index.adoc
[ch05-issues]: https://github.com/oncletom/nodebook/labels/:book:%20chapitre:5
[ch06]: chapter-06/index.adoc
[ch06-issues]: https://github.com/oncletom/nodebook/labels/:book:%20chapitre:6
[ch07]: chapter-07/index.adoc
[ch07-issues]: https://github.com/oncletom/nodebook/labels/:book:%20chapitre:7
[ch08]: chapter-08/index.adoc
[ch08-issues]: https://github.com/oncletom/nodebook/labels/:book:%20chapitre:8
[ch09]: chapter-09/index.adoc
[ch09-issues]: https://github.com/oncletom/nodebook/labels/:book:%20chapitre:9
[a01]: appendix-a/index.adoc
[appendix-issues]: https://github.com/oncletom/nodebook/labels/:book:%20chapitre:annexes
