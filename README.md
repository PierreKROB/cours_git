## Git est un outil de versioning du code.


### Les branches

Pour utiliser Git en équipe, il est essentiel d'exploiter le système de branches. Les branches dans Git permettent de séparer le développement de nouvelles fonctionnalités, la correction de bugs ou l'expérimentation, du code principal 

Chaque branche représente un flux de travail distinct, permettant aux membres de l'équipe de travailler de manière isolée sans affecter le code principal. Cela favorise la réalisation de tâches multiples et indépendantes telles que le développement de nouvelles fonctionnalités, les tests, ou les corrections d'erreurs.

L'utilisation des branches assure également une intégration fluide et contrôlée des changements dans le code principal, contribuant à maintenir la stabilité et la qualité du projet.

### Les merges
Le processus de fusion, ou "merge", est crucial dans le workflow Git. Lorsque le développement dans une branche est complet et que le code est prêt à être intégré dans la branche principale, un merge est effectué. Ce processus intègre les changements d'une branche (par exemple, une branche de fonctionnalité) dans une autre (souvent la branche main ou master).

Le merge peut être réalisé automatiquement par Git, mais il nécessite parfois une intervention manuelle en cas de conflits, c'est-à-dire lorsque les mêmes parties du code ont été modifiées dans les deux branches. La résolution de ces conflits est essentielle pour maintenir l'intégrité et la cohérence du code.

### Les pull requests

Les pull requests (PR) sont une fonctionnalité clé dans les plateformes de gestion de version comme GitHub ou GitLab, bien qu'elles ne fassent pas partie intégrante de Git lui-même. Une PR est une demande pour intégrer les changements d'une branche dans une autre, typiquement de la branche de développement dans la branche principale.