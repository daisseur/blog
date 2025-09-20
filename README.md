# portfolio

### J'aimerai en faire un qui se présente comme un blog
- pour afficher mes projets: on a un bouttons qui trie les posts par tag "project"
- peut aussi sélectionner les "branches git" du repo blog pour les posts qu'on veut, comme par exemple le branche project, la branche musique, la branche jeux vidéo, ia, new de la tech...
- il faut une petite db qui stocke les articles et qui vérifie  régulierement le repo git des articles en markdown pour vérifier qu'elle (la db) est à jour

> grâce à ce systeme on peut créer une colonne tags dans la db pour avoir les posts plus rapidement

> les posts du blogs seraient en fait rangé et annoté à la façon d'un repo git, avec le nom du commit à partir duquel l'article a été ajouté mais aussi le nom du commit où il a été update pour la derniere fois par exemple "Created ef34cE.. - Last updated FGheJ4kc.."

> la façon de se balader dans les articles seraient organisé un peu comme git avec un indicateur HEAD~1 HEAD~21 etc

- le git du blog serait hebergé sur github pour permettre à tout le monde de voir de façon "brut" les articles et aussi de pouvoir soumettre des pull request ou des issues

> dans les posts markdown on rajoute une syntaxe spéciale pour render component Github d'un autre repo par exemple pour un projet à moi ou justement mettre celui d'une autre personne, par ex:  {{type: "Github", "repoUrl": "https://github.com/permissionlesstech/bitchat-android" }}

> avec groq, rajouter un moyen de traduire mon post original dans un français normal, en français pro, en anglais normal ou anglaisPro
