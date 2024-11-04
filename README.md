# TechNext4CNAM - Codelab GitOps

:rocket: Bievenue dans ce codelab GitOps ! :rocket:

Aujourd'hui, nous allons explorer la manière de mettre en place le GitOps avec ArgoCD !

L'approche GitOps repose sur l'utilisation de référentiels Git comme unique source de vérité pour distribuer l'infrastructure en tant que code. Ainsi, l'approche GitOps apporte les avantages suivants : 

* <b>Audit et Traçabilité :</b> Chaque changement est versionné et traçable grâce à l'historique Git, ce qui facilite l'audit des modifications et l'identification de la source des problèmes.

* <b>Automatisation et Cohérence :</b> En automatisant les déploiements à partir des dépôts Git, GitOps réduit les erreurs humaines et assure une cohérence entre votre environnement de développement, de test et de production.

* <b>Temps de Récupération Réduit :</b> En cas de problème, vous pouvez rapidement restaurer un état précédent de l'application ou de l'infrastructure simplement en revenant à une version antérieure du dépôt Git.

* <b>Collaboration Facilitée :</b> Les développeurs et opérateurs peuvent collaborer plus efficacement via des pull requests et des revues de code, facilitant l'adoption de meilleures pratiques et la gestion des modifications.

* <b>Rapidité de Déploiement :</b> Les changements peuvent être déployés rapidement et fréquemment grâce à un processus automatisé, favorisant l'amélioration continue et l'innovation.

* <b>Alignement avec les Principes DevOps :</b> GitOps s’aligne parfaitement avec les principes DevOps en intégrant le contrôle de version, l’automatisation et la collaboration dans le processus de gestion de l’infrastructure.

## Objectifs du codelab

Passons aux choses sérieuses ! Dans ce codelab, vous allez :
* Créez votre première applications sous ArgoCD, et découvrir toutes les subtilités de configurations applicables sur une application ArgoCD
* Construire un déploiement pour déployer une application backend
* Construire un déploiement pour déployer une application frontend
* Jouer avec les capacités de self-healing d'ArgoCD
* Explorer comment le GitOps facilite les opérations de décomissionnement
* Explorer comment le GitOps peut nous aider en cas de mise en production qui se passe mal

Allez, c'est parti ! 🙂

## Présentation de l'environnement

Nous vous avons mis un disposition un cluster Kubernetes déployé sur le cloud public Azure ([Azure Kubernetes Services](https://azure.microsoft.com/fr-fr/products/kubernetes-service)).

Un <b>identifiant</b> vous est attribué à tous. Ce dernier est systématiquement composé de la manière suivante : <b>[premiere_lettre_de_votre_prenom][votre_nom]</b>. Voici deux exemples : 
* Rémi KAEFFER -> rkaeffer
* Jason BOURLARD -> jbourlard

Par défaut, ce cluster vous propose les services suivants : 
* Une instance commune d'ArgoCD, qui va vous permettre de déployer vos applications, et disponible à l'URL suivante : https://argo-cd.codelab.cloud-sp.eu/
    * Username : admin
    * Password : A REMPLIR LE JOUR DU LAB - ET A EFFACER APRES
* Un environnement de développement pour chacun d'entre vous, composés de deux namespaces : 
    * Un namespace, nommé kcl-[identifiant]-wk, portant un VScode et tout plein d'outils (kubectl, git, ...), et accessible à l'url [[identifiant]-kcl.codelab.cloud-sp.eu](tochange-kcl.codelab.sp.eu)
    * Un namespace, nommé kcl-[identifiant], où devra être déployé vos applications

## Pré-requis avant de démarrer

Pour pouvoir effectuer ce codelab, quatres pré-requis sont nécessaires (Pas de panique, rien à installer 😁) : 
* Etre connecté à notre réseau Wifi SSG-Guest (Normalement, on vous a autorisé ce matin, si ce n'est pas le cas, faites le nous savoir) !
* Disposer d'un compte Github, et avoir généré un [personal token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#creating-a-personal-access-token-classic) d'accès pour pouvoir push sur vos repositories
* Vérifier que vous avez bien accès à [ArgoCD](https://argo-cd.codelab.cloud-sp.eu/)
* Vérifier que vous avez bien accès à votre environnement de travail : [[identifiant]-kcl.codelab.cloud-sp.eu](tochange-kcl.codelab.sp.eu)

## Instructions du codelab

### Etape 0 - Préparation et exploration

### Etape 1 - Créer une application dans ArgoCD

### Etape 2 - Deploiement du backend

### Etape 3 - Deploiement du frontend

### Etape 4 - Jouons avec ArgoCD

### Etape 5 - Décomissionement du frontend

### Etape 6 - Rollback du décomissionement

### Etape 7 - Pour aller plus loin

## Tips pour le lab