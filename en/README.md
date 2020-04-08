<p align="center">
  <a href="https://github.com/github_username/repo">
    <img src="img/favicon.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center"><a href="https://covprehension.org" target="_blank">CoVprehension</a></h3>

  <p align="center">
    Informative website about the corona virus.
    <br />
    <br />
    <img src="https://img.shields.io/github/license/covprehension/covprehension" alt="License" />
    ·
    <img src="https://img.shields.io/github/issues/covprehension/CoVprehension" alt="GitHub issues" />
    ·
    <img src="https://img.shields.io/github/contributors/covprehension/covprehension" alt="GitHub contributors" />
    <br />
    <img src="https://github.com/covprehension/CoVprehension/workflows/Jekyll%20site%20CI/badge.svg?branch=master" alt="Jekyll site CI" />
    ·
    <img src="https://img.shields.io/discord/690125443952672780?label=Discord" alt="Discord" />
  </p>
</p>

This repository holds the Jekyll sources of the CoVprehension website!

> The following section will be in french, sorry 🤷

## Comment utiliser ce site ?

### Structure du repository

<details>
<summary>View contents</summary>

```
$ tree
.
├── assets
│   ├── <custom JS/CSS files>
│   │
│   └── vendor <default resources>
│       ├── bootstrap
│       ├── fontawesome-free
│       ├── jquery
│       └── template
│
├── img
│   └── <website images>
│
├── _includes
│   └── <Global part of website : Header/Footer/etc>
│
├── _layouts
│   └── <HTML pages template>
│
├── _posts
│   ├── ...
│   └── <All your questions>
│
├── posts
│   └── <IGNORE ME, I'm a trap 🙊>
│
├── _sass
│   ├── js
│   │   └── <JS simulation in sub-dir>
│   │
│   └── styles.scss
│
├── simulations
│   └── <Web NetLogo export simulations>
│
├── _config.yml
│
├── about.html
├── contact.html
├── index.html
├── ressources.md
├── simulateur.html <Don't touch me>
│
└── <others...>

<plenty> directories, <too many> files
```

</details>

### Créer un nouvel article

1. Aller dans le sous-dossier [`_posts`](https://github.com/RoiArthurB/CoVprehension/tree/master/_posts)
2. Créer un nouveau fichier au format suivant : `AAAA-MM-JJ-mots-clefs.md`
3. **Copier-coller** puis **Compléter** l'en-tête suivante :
```
---
layout: post

# Toutes les lignes commençant par un "#" sont ignorées, ce sont des commentaires pour les humains !

# Cette partie est réutilisé pour l'apperçu du post dans les pages principales
title: "Le titre de l'article. eg/ Question 1: Pourquoi je tousse ?"
subtitle: "Le sous-titre de l'article. eg/ blablabla. Démonstration !"

# Choisir une image d'illustration qui doit être un chemin relatif vers le dossier img/
# (si cette phrase n'a pas été comprise, demandez de l'aide :) ) 
# Par défaut image du masque 
#background: '/img/bg-index.jpg'

# Choisir les auteurs
# Ne s'affichera pas si vide
author_text : 
author_simulations : 
author_illustration : 
author_translation :

# Pour ne pas afficher la question dans le flux global
hidden: false

# Marque la question comme "traitée" ou "en traitement" si elle est, dans cette ordre, publiée ou non
publish: true
---
```
4. Remplir le contenu de l'article en écrivant un article au format [HTML](https://www.w3schools.com/html/) ou au format [MarkDown](https://www.markdownguide.org/).

### Configuration globale du site

Toute la configuration globale du site se trouve dans le fichier [`_config.yml`](https://github.com/RoiArthurB/CoVprehension/blob/master/_config.yml) qui a la structure suivante :
 - `baseurl` ⚠️ ne pas changer ⚠️
 - `url` ⚠️ ne pas changer ⚠️
 - `title` 
 - `email` (mail global utilisé un peu partout: contact, liens, etc)
 - `description` (page d'accueil)
 - `author` (valeur par défaut)
 - `twitter_username` (Optionel - Enlève l'icone en pied de page si vide)
 - `facebook_username` (Optionel - Enlève l'icone en pied de page si vide)
 - `github_username` (Optionel - Enlève l'icone en pied de page si vide)
 - `linkedin_username` (Optionel - Enlève l'icone en pied de page si vide)

## Technical part

> I'm switching back in english, hi again friends ! :D

### Local installation & Setup

1. Clone the repo `git clone git@github.com:RoiArthurB/CoVprehension.git`
2. Move in the folder `cd CoVprehension`
3. Install plugins: `bundle install`
4. Build your site: `bundle exec jekyll serve`
5. Connect to your running instance [http://127.0.0.1:4000/CoVprehension/](http://127.0.0.1:4000/CoVprehension/)

## Bugs and Issues

Have a bug or an issue with this template? [Open a new issue](https://github.com/RoiArthurB/CoVprehension/issues/new) here on GitHub!

## Made with

* Pipeline
  * Jenkyll
  * Github Pages

* Front-end
  * Bootstrap / jQuery
    * Theme from [Start Bootstrap](https://startbootstrap.com/)
  * [Particle.js](https://vincentgarreau.com/particles.js/)
  * [Charts.js](https://www.chartjs.org/)

* Simulations
  * NetLogo

## Copyright and License

This website is released under the [MIT](https://github.com/RoiArthurB/CoVprehension/blob/gh-pages/LICENSE) license.
