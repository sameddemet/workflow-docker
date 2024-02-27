
 ## Exercice 1 - Workflow d'assignation d'issue (5 points)
  
### Sujet

Ecrire un workflow pour assigner automatiquement une issue à un compte Github (par exemple le votre) (5 points).
    - Vous pouvez utiliser l’action du marketplace de votre choix
    - Ajoutez dans le readme du dépôt (au tout début de ce readme) un badge pour visualiser l’état d’exécution du workflow d’auto assignation d’issue

### Réponse
[![Auto Assign Issue Workflow Status](https://github.com/O-clock-Hati/examen-s10-final-sameddemet/actions/workflows/auto_assign.yml/badge.svg)](https://github.com/O-clock-Hati/examen-s10-final-sameddemet/actions/workflows/auto_assign.yml)


[X] Nom du workflow : `<auto_assign>`

## Exercice 2 - Workflow schedule (2 points)

### Sujet

Ecrire un workflow qui s’exécute à midi et affiche un message : `fin de l’examen` avec un cowsay. (2 points)

### Réponse

[X] Nom du workflow : `<fin_de_examen>`

## Exercice 3 - Workflow self-hosted

### Sujet

Ecrire un workflow qui s’exécute sur votre vm cloud serveur via un runner self-hosted, il doit enregistrer un fichier cow.txt dans `/home/student/cow.txt` et doit contenir un message en asciiart stylé avec une vache qui dit : `c'est le commit numéro : <idDuCommit>`Le workflow doit s’exécuter à chaque push sur la branche principale. (6 points)

### Réponse

[X] Nom du workflow : `<vache.yml>`

## Exercice 4 - Build and push, challenge de vendredi (7 points)

### Rappel du sujet

- Builder une image et l’uploader sur Docker hub
- L’image doit être originale : cowsay non classique, version python, js, go …
 - pourquoi pas un tuxsay avec un tux par défaut au lieu d’une vache.
 - il y a aura une note artistique
- L’image doit être la plus petite possible.
- L’image doit être documentée automatiquement et utiliser le readme.md de votre dépôt.
- Doit être disponible dans deux versions :
 - une complète (tag full)
 - une minimaliste (tag small)


### Réponse

- url dockerhub de votre image : https://hub.docker.com/r/sameddemet/tuxsay-full , https://hub.docker.com/r/sameddemet/tuxsay-small
- lien vers le workflow de déploiement : https://github.com/sameddemet/tuxsay/blob/main/.github/workflows/docker_build.yml
- lien vers le fichier Dockerfile : https://github.com/sameddemet/tuxsay/blob/main/Dockerfile




## Exercice 4 - Optionnel, Marketplace, challenge de ce lundi soir (3 points bonus)

### Rapppel du sujet

Ecrire votre propre Github action composite qui reprend de manière plus simple le docker build-and-push :
* Prise en compte des paramètres suivants :
  * nom de l'image
  * numéro de tag (par défaut nom de la branche)
  * context (par défaut .)
* Push directement sur la registry Github (sans paramètre en utilisant, github.actor et secrets.GITHUB_TOKEN)
* Publier l'action du le marketplace Github action
Ce challenge permettra d'avoir entre 1 et 3 points bonus pour l'examen de demain matin.

### Réponse

Mettez ici les informations concernant le challenge de ce lundi soir (3 points supplémentaires) :
- url du marketplace de votre action : `<TO COMPLETE>`
