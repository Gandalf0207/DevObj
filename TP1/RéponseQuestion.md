# Développement Orienté Obj

### Suivis de TP et réponse aux questions

---

- Qu'est-ce qu'un _dépôt Git_ ? <br>
  Un dépot git est un endroit où est stocké du code. Sur ce dépot git nous pouvons ajouter du code, le modifier ou encore le supprimer. Plusieurs personnes peuvent avoir accès à ce dépot en fonction de leurs roles.

- Qu'est-ce qu'un _fork_ Git ? <br>
  Un fork git est une copie modifié du dépot qui peut etre proposé pour etre implémenté au sein du dépot git. Ce fork tout le monde peut le faire si le dépot est en public

- Quelle est la différence entre Git et GitLab/GitHub ? <br>
  Git est un outil de versioning en local de projet alors que Gitlba / GitHub sont des service en ligne qui se sont démocratisé plus tard qui permettent de faire travailler plusieurs personnes en meme temps sur un meme projet à travers internet.

- Que fait `git clone` ? <br>
  La commande git clone permet de récupérer le contenu du dépot quand il est suivis d'une adresse web. Cela va copier les fichier distant sur la machien à l'endroit où est exécuté la commande.

- Quelle est la différence entre `git add` et `git commit` ? Pourquoi avoir séparé les deux commandes ? <br>
  La commande git add permet d'ajouter les fichiers modifié pour les versionner. La commande git commit permet de pack c'est fichier modif et ajouter un description à ce package. Elles ont été séparé car cela nous permet de mieux versionner est sélectionner nos modification. On peut faire plusieurs commit en meme temps tout en sélectionnant nos ficiher qui sont pris par le commit en question.

- À quoi correspond le fichier `.gitignore` ? <br>
  Le fichier git ignore va comme son nom l'indique ignorer les fichiers qui se trouvent dedans. Cela permet de ne pas les versionner. Souvent des fichirs de config machine qui ne doivent pas apparaitre dans le code du projet.

- À quoi correspond le raccourci `git push` ? <br>
  Git push va envoyer les modifications faites dans le versioning du projet (web ou local). Cette commande vient conclure la modication après les commit. Elle envoie tout les commit en stand-by

- À quoi correspond le raccourci `git pull` ? <br>
  Un git pull est une commande qui permet de récupérer sur un dépot distant les modifications qui ont été réalisé et donc de syncroniser notre projet avec celui distant qui est le projet parent et main

- Qu'est-ce qu'un _conflit_ Git ? <br>
  Un git conflict est un soucis quand un meme fichiers à deux versions diff"rentes. Git ne peut pas toujours les résoudre seul. Il faut donc reprendre le code et le corriger nous meme.

Exercice 1 :

- Q4 : Entre le répertoire local est distant, le fichier.class crée avec javac n'est pas sur présent. En effet ce fichier est resté en local mais n'est pas sur le dépot distant. C'est un fichier créé pour la compilation, donc il ne doit pas etre pris en compte dans le versioning car c'est simplement un fichier compilé et donc non utilisable.

Exercice 2 :

- Q7 : On ne peut pas push car il y a une modification sur le dépot distant qui n'est pas syncronisé avec le dépot local.

- git fetch + git merge important pour modif des conflict

Exercice 3 :

- Notion pour écraser un contenu et forcer l'écrasement sur le dépot distant : git reset et --force
