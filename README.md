Init
# Guide d'utilisation Github 
## Introduction 
### Bien sûr, voici une présentation de GitHub :

---

**GitHub : La Plateforme d'Hébergement et de Collaboration pour le Développement de Code**

GitHub est bien plus qu'une simple plateforme d'hébergement de code ; c'est un écosystème complet dédié au contrôle de version, à la collaboration et à la gestion de projets logiciels. Lancé en 2008, GitHub est devenu un outil essentiel pour les développeurs du monde entier.

* **Hébergement de Code :** GitHub offre un espace en ligne pour stocker, gérer et collaborer sur des projets de développement logiciel. Les utilisateurs peuvent créer des dépôts (repositories) pour héberger leur code source, et ces dépôts peuvent être publics (accessibles à tous) ou privés (limités à une équipe spécifique).

* **Contrôle de Version :** Basé sur Git, le système de contrôle de version le plus populaire, GitHub permet de suivre les modifications apportées au code au fil du temps. Les développeurs peuvent créer des branches pour travailler sur des fonctionnalités spécifiques sans perturber le code principal, puis fusionner ces branches une fois les modifications terminées.

* **Collaboration Facilitée :** GitHub simplifie la collaboration en permettant aux développeurs de travailler ensemble sur des projets, que ce soit en ajoutant des commentaires, en signalant des problèmes (issues), ou en proposant des modifications via des pull requests. La gestion efficace des contributions devient ainsi une réalité.

* **Flux de Travail des Pull Requests :** Une caractéristique distinctive de GitHub est le flux de travail des pull requests. Les développeurs peuvent suggérer des modifications à un projet en créant une pull request, et ces modifications peuvent être examinées, discutées et intégrées avant d'être fusionnées dans le code principal.

* **Gestion de Projet :** GitHub propose également des fonctionnalités de gestion de projet, notamment des tableaux Kanban pour suivre les tâches, des intégrations avec des outils de suivi des problèmes, et des pages Wiki pour documenter les projets.

* **Communauté Active :** GitHub abrite une communauté dynamique de développeurs, d'entreprises et de projets open source. Les utilisateurs peuvent découvrir des projets, contribuer à des bibliothèques de code ou même trouver des opportunités d'emploi.

Que vous soyez un développeur solo ou que vous travailliez au sein d'une équipe, GitHub offre un environnement collaboratif puissant pour le développement de logiciels, favorisant l'innovation et la qualité du code.

## Installer Git

Avant de commencer à utiliser Git, vous devez l'installer sur votre machine.

### Windows
1. Téléchargez Git depuis [git-scm.com](https://git-scm.com/download/win).
2. Lancez l'installateur et suivez les instructions pour compléter l'installation.

### macOS
1. Vous pouvez installer Git via le terminal avec la commande `git` qui déclenchera une invite d'installation, ou
2. Utilisez Homebrew en tapant `brew install git` dans le terminal.

### Linux
1. Ouvrez un terminal.
2. Installez Git en utilisant le gestionnaire de paquets de votre distribution. Par exemple, sur Debian/Ubuntu, utilisez `sudo apt-get install git`.

## Configurer Git sur Votre Machine

Une fois Git installé, il est important de le configurer.

### Identité
Configurez votre nom et adresse e-mail, qui seront utilisés dans vos commits. Remplacez `Votre Nom` et `votre.email@example.com` par vos informations personnelles.

```bash
git config --global user.name "Votre Nom"
git config --global user.email "votre.email@example.com"
```
### Vérifier la Configuration

Vous pouvez vérifier votre configuration en exécutant :

```bash
git config --list
```

## Initialiser un Nouveau Dépôt

### Créer un Dépôt Local
1. Ouvrez un terminal.
2. Naviguez vers le dossier où vous souhaitez initialiser le dépôt.
3. Exécutez la commande suivante :

```bash
git init
```

## Les commandes de base
Une fois votre projet initialisé, vous pouvez maintenant travailler dans votre environnement local. Voici quelques commandes de base à connaître :

# git status
La commande git status permet de voir l'état de votre branche, indiquant si elle est à jour ou non. Les fichiers seront en rouge s'ils sont supprimés, en vert s'ils sont ajoutés et en jaune s'ils sont modifiés.

# git add <nom_de_fichier>
La commande git add permet d'ajouter des fichiers, dossiers ou modifications à votre branche locale. Vous pouvez utiliser la commande git add . pour ajouter toutes les modifications effectuées.

# git commit
La commande git commit permet de sauvegarder vos modifications dans la branche locale après les avoir ajoutées. Il doit toujours y avoir un message dans votre commit pour connaître le sujet de celui-ci. La commande git commit -m "Sujet_du_commit" permet d'ajouter directement le message pour gagner du temps.

# git pull
La commande git pull permet de récupérer les mises à jour d'une branche afin de les modifier.

# git push
La commande git push permet d'ajouter vos modifications dans votre dépôt distant.

# git checkout
La commande git checkout permet de naviguer entre les branches. La commande git checkout -b <Nom_de_branche> permet de créer directement une nouvelle branche.

# git branch
La commande git branch permet de voir la liste des branches.

# git log
La commande git log permet de voir les logs de votre local. C'est-à-dire tous les commits effectués, quand, par qui et le message du commit.

# git show
La commande git show permet de voir les informations du dernier commit effectué.

# git config
La commande git config permet de voir les informations de votre local. Par exemple, les commandes git config --global user.name "Votre Nom" et git config --global user.email "votre@email.com" vous permettent de modifier vos informations.

## Le fichier .gitignore
Le fichier .gitignore est un fichier texte utilisé par Git pour spécifier les fichiers et répertoires qui doivent être ignorés lors de la gestion de version. Ces fichiers et répertoires ignorés ne seront pas suivis par Git, ce qui signifie qu'ils ne seront ni inclus dans les commits ni envoyés au dépôt distant lors d'un git push. Ce dossier peut notamment être utilisé pour stocker le fichier .env ou le dossier node_modules.


## Git est un outil de versioning du code.


### Les branches

Pour utiliser Git en équipe, il est essentiel d'exploiter le système de 
branches. Les branches dans Git permettent de séparer le développement de nouvelles fonctionnalités, la correction de bugs ou l'expérimentation, du code principal 

Chaque branche représente un flux de travail distinct, permettant aux membres de l'équipe de travailler de manière isolée sans affecter le code principal. Cela favorise la réalisation de tâches multiples et indépendantes telles que le développement de nouvelles fonctionnalités, les tests, ou les corrections d'erreurs.

L'utilisation des branches assure également une intégration fluide et contrôlée des changements dans le code principal, contribuant à maintenir la stabilité et la qualité du projet.

Pour créer une nouvelle branche : 

#### Lancer la commande suivante : 

```feature

    git checkout -b nom_de_la_branche

```

### Les merges

Le processus de fusion, ou "merge", est crucial dans le workflow Git. Lorsque le développement dans une branche est complet et que le code est prêt à être intégré dans la branche principale, un merge est effectué. Ce processus intègre les changements d'une branche (par exemple, une branche de fonctionnalité) dans une autre (souvent la branche main ou master).

Le merge peut être réalisé automatiquement par Git, mais il nécessite parfois une intervention manuelle en cas de conflits, c'est-à-dire lorsque les mêmes parties du code ont été modifiées dans les deux branches. La résolution de ces conflits est essentielle pour maintenir l'intégrité et la cohérence du code.

Le merge s'effectue de la façon suivante : 

- Se placer dans la branche à laquelle on souhaite apporter les changements.

#### Lancer la commande suivante : 

```feature

    git merge nom_de_la_branche

```

### Les pull requests

Les pull requests (PR) sont une fonctionnalité clé dans les plateformes de gestion de version comme GitHub ou GitLab, bien qu'elles ne fassent pas partie intégrante de Git lui-même. Une PR est une demande pour intégrer les changements d'une branche dans une autre, typiquement de la branche de développement dans la branche principale.

Il est possible de lancer une pull request via l'interface graphique de github. 
