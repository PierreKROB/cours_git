## Les commandes de base
Une fois votre projet initialisé, vous pouvez maintenant travailler dans votre environnement local. Voici quelques commandes de base à connaître :

### git status
La commande git status permet de voir l'état de votre branche, indiquant si elle est à jour ou non. Les fichiers seront en rouge s'ils sont supprimés, en vert s'ils sont ajoutés et en jaune s'ils sont modifiés.

### git add <nom_de_fichier>
La commande git add permet d'ajouter des fichiers, dossiers ou modifications à votre branche locale. Vous pouvez utiliser la commande git add . pour ajouter toutes les modifications effectuées.

### git commit
La commande git commit permet de sauvegarder vos modifications dans la branche locale après les avoir ajoutées. Il doit toujours y avoir un message dans votre commit pour connaître le sujet de celui-ci. La commande git commit -m "Sujet_du_commit" permet d'ajouter directement le message pour gagner du temps.

### git pull
La commande git pull permet de récupérer les mises à jour d'une branche afin de les modifier.

### git push
La commande git push permet d'ajouter vos modifications dans votre dépôt distant.

### git checkout
La commande git checkout permet de naviguer entre les branches. La commande git checkout -b <Nom_de_branche> permet de créer directement une nouvelle branche.

### git branch
La commande git branch permet de voir la liste des branches.

### git log
La commande git log permet de voir les logs de votre local. C'est-à-dire tous les commits effectués, quand, par qui et le message du commit.

### git show
La commande git show permet de voir les informations du dernier commit effectué.

### git config
La commande git config permet de voir les informations de votre local. Par exemple, les commandes git config --global user.name "Votre Nom" et git config --global user.email "votre@email.com" vous permettent de modifier vos informations.

## Le fichier .gitignore
Le fichier .gitignore est un fichier texte utilisé par Git pour spécifier les fichiers et répertoires qui doivent être ignorés lors de la gestion de version. Ces fichiers et répertoires ignorés ne seront pas suivis par Git, ce qui signifie qu'ils ne seront ni inclus dans les commits ni envoyés au dépôt distant lors d'un git push. Ce dossier peut notamment être utilisé pour stocker le fichier .env ou le dossier node_modules.