#  README PFE#002

Suite aux NDA que nous avons signé, ce dépôt ne contient aucun code. Pour obtenir le code du projet vous devez vous rendre sur le lien Gitlab suivant  sur la branche 'enas') ->  [https://git-iutinfo.unice.fr/rey/m2-18-19-ados-outil](https://git-iutinfo.unice.fr/rey/m2-18-19-ados-outil)


# Installation et exécution

Pour installer et lancer notre projet, veuillez suivre les instructions présentes dans les sections suivantes.

## Prérequis

Pour assurer le bon fonctionnement du projet vous devez posséder les outils suivants, avec les versions précisées de préférence:
 - MongoDB (4.2.1)
 - Maven (3.6.2)
 - NodeJS (12.13.1)
 - Angular/CLI (8.3.20)
 - npm (6.13.1)

## Installation et exécution

Vous devez tout d'abord cloner le projet Gitlab sur votre PC. Une fois cette action effectuée vous allez devoir mettre en place le serveur et le client. Pour que le projet fonctionne correctement, assurez vous de lancer d'abord le serveur, puis le client.

###  Le serveur
Pour mettre en place le serveur vous devez vous rendre dans le dossier *"server"* et y ouvrir un invite de commande. A partir de cette invite, lancez la commande ***mvn install***. Patientez que les différents téléchargements et installations soient finis. Une fois l'installation terminée, toujours dans l'invite de commande, entrez la commande ***mvn spring-boot:run***, et patientez jusqu'à ce que le lancement du serveur soit effectué (celui-ci se lance par défaut sur le port 80 de votre PC).

###  Le client
Pour mettre en place le client rendez vous dans le dossier *"client"* du projet. A partir de ce dossier ouvrez un invite de commande, puis entrez la commande ***npm install***. Patientez que les différents téléchargements et installations soient finis. Une fois toutes les installations terminées, lancez la commande ***ng serve***. Patientez le temps que le client se mette en place. Au bout d'un certains temps celui-ci devrait s'ouvrir automatiquement dans votre navigateur internet. Si ce n'est pas le cas, assurez vous que la compilation se soit bien exécutée (le message "Compiled successfully" devrait être apparu dans votre invite de commande) et entrez l'adresse suivante dans le navigateur de votre choix: **http://localhost:4200/**.

## Changement des ports
Vous avez la possibilité de changer le port sur lequel se lance le serveur ainsi que la base de donnée. Pour se faire, allez dans le fichier *"application.properties"* situé dans le dossier *"server/src/main/resources"*, et modifiez la ligne *"server.port"* en indiquant le nouveau port que vous souhaitez attribuer au serveur. Veuillez néanmoins prêter attention à ce que le port utilisé par le client concorde avec celui du serveur. Pour changer l'hôte et le port sur lesquels démarre la base de donnée modifiez les lignes *"spring.data.mongodb.host"* et *"spring.data.mongodb.port"*.
