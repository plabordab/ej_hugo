---
title: "Markdown"
date: 2022-09-23T16:59:13+02:00
draft: false
---

# h1 Titre 1
## h2 Titre 2
### h3 Titre 3
#### h4 Titre 4
##### h5 Titre 5
###### h6 Titre 6

<!--
commentaire
-->

Tout texte qui ne commence pas par un signe spécial sera écrit comme du texte normal, sans mise en forme, et sera enveloppé à l'intérieur des balises <p></p> dans le HTML rendu.

**bold**.

_italique_

*italique*

*****gras et italiques*****

~~strikethrough~~

~~***Marquage, gras et italique***~~

> Pour inclure des citations 
>
>> Vous pouvez inclure des citations dans des citations
> 
> Et continuer dans le précédent

*Notes de bas de page*

Cette année, nous visiterons la Giralda [^1]. Ce sera une visite importante.

*Définition des abréviations:* 

Le TAS a approuvé sa demande.

*[TAS] : Tribunal arbitral du sport.

Désormais, chaque fois que nous écrirons TAS, nous aurons toujours sa définition à disposition.

*Définition des mots:* 

Markdown
: un langage de balisage léger créé par John Gruber.
Gruber
: Il s'agit d'un mot anglais signifiant "démarquage".

#### **listes**


* énumération 1
    - énumération 2
        + énumération 3

1. Listes
4. où
2. le
12. commande
8. pas
99. est
21. important

..

Si vous n'utilisez que 1. 
1. pour chaque numéro, 
1. le numéro de Markdown sera automatiquement 
1. chaque élément



#### **Code**

Pour mettre en évidence le code dans une phrase: `sudo apt install libreoffice`.

Pour inclure l'indentation, nous mettons en retrait au moins deux espaces:
    ligne 1 du code
    ligne 2 du code
    ligne 3 du code


``` 
On utilise des guillemets pour écrire 
plusieurs lignes de code
```

Pour mettre en évidence la syntaxe, nous ajoutons l'extension du fichier de la langue que nous voulons utiliser après les guillemets.

```js
grunt.initConfig({
  assemble: {
    options: {
      assets: 'docs/assets',
      data: 'src/data/*.{json,yml}',
      helpers: 'src/custom-helpers.js',
      partials: ['src/partials/**/*.{hbs,md}']
    },
    pages: {
      options: {
        layout: 'default.hbs'
      },
      files: {
        './': ['src/templates/pages/index.hbs']
      }
    }
  }
};
```



#### **Tablas**

| Heure | Lundi | Mardi | Mercredi | Jeudi | Vendredi|
| ------: | ------ | ------ | ------ | ------ | ------ | 
| 1 | Client | Déploiement | ------ | Client | Serveur | 
| 2 | Client | Déploiement | ------ | Client | Serveur | 
| 3 | Client | Serveur | Interfaces | Client | Serveur | 
| 4 | Interfaces | Serveur | Interfaces | Serveur | Interfaces | 
| 5 | Déploiement | Serveur | ------ | Serveur | Interfaces | 
| 6 | Déploiement | ------ | ------ | Serveur | Interfaces | 

Le texte est justifié à droite en mettant : à droite des tirets dans la colonne correspondante.

**Liste de tâches 14-12-2019**.

- [X] emmener les enfants à la piscine
- [X] apprendre le markdown
- [] renouveler mon abonnement au club de gym


#### **Hyperliens**

[Syntaxe Markdown](https://geekland.eu/aprender-markdown-en-minutos/ "Vous pouvez ajouter une bulle avec des informations d'aide")


**Tables de contenu avec ancres au document** 

- [Listes](#Listes)
- [Code](#Code)
- [Tableaux](#Tableaux)
- [Hyperliens](#Hyperliens)


![Image introuvable](/image/img1.jpeg "titre optionnel")

Entre deux sections de texte, nous pouvons inclure une séparation physique. Pour ce faire, nous devons écrire 3 caractères de soulignement à la suite. 

___

> Il est important d'inclure dans les images la valeur alt (texte alternatif si l'image ne se charge pas).
>
> Créez un dossier d'images dans le dossier statique.
>
> Dans le dossier public, la structure entière est sauvegardée à partir du dossier statique.





[^1] : Nom donné au clocher de la cathédrale de Santa Maria de la Sede.