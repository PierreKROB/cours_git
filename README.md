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