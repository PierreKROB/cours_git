Init

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