# Mini-projet: Déployez PayMyBuddy à l’aide de manifests ☺

## Contexte
Il s'agit de déployer l'application SpringBoot PayMyBuddy à l'aide de manifests yaml que vous allez écrire et non pas avec helm,
ce qui vous permettra de comprendre plus en détails la mise en place d'une application dans un cluster Kubernetes.

https://github.com/OlivierKouokam/PayMyBuddy/

## Etapes à réaliser

- Déployez PayMyBuddy en suivant les étapes suivantes
     - Créez un deployment mysql avec un seul replicat
     - Votre deployment devra stocker les données mysql de PayMyBuddy sur un voulme mounté dans le /data/mysql de votre nœud
     - Créez un service de type clusterIP pour exposer vos pods mysql
     - Créez un deployment paymybuddy avec les bonnes variables d’environnement pour se connecter à la base de données mysql. Vous trouverez les variables d'environnement nécessaire dans ce fichier: https://github.com/OlivierKouokam/PayMyBuddy/blob/main/Dockerfile
     - Créez un service de type nodeport pour exposer le déployment paymybuddy
- Nous vous conseillons d’utiliser les manifests pour réaliser cet exercice
- A la fin de votre travail, poussez vos manifests sur github et envoyez nous le lien de votre repo à
contact@eazytraining.fr et nous vous dirons si votre solution respecte les bonnes pratiques et si votre solution
bonne. Nous vous proposerons aussi notre solution/
