---
title: "Git"
date: 2022-09-27T19:54:33+02:00
draft: false
---

## DÉPÔT SUR GITHUB

## créer un nouveau référentiel et le lier au référentiel local

1. connectez-vous à github avec votre nom d'utilisateur et votre mot de passe.
2. Dans notre compte, nous créons un référentiel
3. il nous indique les commandes à exécuter localement. Les actions sont :
4. Nous allons en local dans le répertoire où se trouve notre projet
5. Exécuter : 

a.

```
git init 
```
>  Cette commande initialise notre répertoire comme un projet git. Vous aurez créé un répertoire appelé .git.


b. 

```
git add . 
```
>  avec cette commande nous ajoutons les fichiers de mon répertoire (tous à spécifier par .) au référentiel


c.

```
git comit -m "message du point de contrôle" 
```
>  avec cette commande nous spécifions un message pour les changements en cours


d. 

```
git branch -M main 
```
>  avec cette commande, créez une branche ou un répertoire de travail associé au référentiel local


e.

```
git add remote origin https://github.com/plabordab/ej_hugo 
```
>  Utilisez cette commande pour lier le référentiel local au référentiel distant.

f.

```
git push origin main  
```
>  Avec cette commande, nous ajoutons les fichiers ajoutés au fichier distant.


## copier un projet vers une autre destination

1. j'accède au hub git et je copie l'url du dépôt.

2. Je tape :

```
git clone https://github.com/plabordab/ej_hugo 
```
> créera un répertoire avec le nom du projet et tout le contenu (seulement fait la première fois).

3. je télécharge également le thème

4. Après le travail, pour le sauvegarder, nous faisons un push :

```
git add *
git commit -m "nuevos cambios"
git push -u origin main  
```
>  mettre à jour le projet sur github avec les dernières modifications


### mettre à jour un projet modifié ailleurs

```
git pull  
```
>  mettre à jour le projet local avec le projet distant

