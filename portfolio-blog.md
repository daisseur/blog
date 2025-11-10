[tags]: <> (github, profile, projects, open source, developer, portfolio, svelte, sveltekit, web development)

# Portfolio Blog
> En ligne (prod) sur [daisseur.xyz](https://daisseur.xyz/from/github) depuis le 19 octobre 2025 !!

Ce projet vise à créer un portfolio qui se présente comme un blog, avec une organisation inspirée de Git pour la gestion et la navigation des articles.

Le brouillon initial est disponible ici : [Blog Git-like](https://github.com/daisseur/blog/blob/61ff6cbfd5aa4d0b13c14a51a7abe54ef69b5f30/README.md).
Et la présentation du repo repo github du blog [ici](https://github.com/daisseur/blog/README.md) 


## Fonctionnalités principales

- **Affichage des projets**  
    Un bouton permet de trier les posts par tag, par exemple "project".

- **Navigation par branches Git**  
    Possibilité de sélectionner différentes branches du dépôt (ex : project, musique, jeux vidéo, IA, news tech...) pour filtrer les articles.

- **Base de données synchronisée**  
    Une petite base de données stocke les articles et vérifie régulièrement le dépôt Git pour rester à jour.  
    > Ajouter une colonne `tags` pour accélérer la recherche des posts.


## Organisation des articles

- **Structure Git-like**  
    Les articles sont annotés avec le nom du commit de création et de dernière mise à jour (ex : `Created ef34cE.. - Last updated FGheJ4kc..`).

- **Navigation inspirée de Git**  
    Parcours des articles avec des indicateurs du type `HEAD~1`, `HEAD~21`, etc.

## Les articles eux-mêmes

- **Article projet**
    Si j'ai travaillé sur un projet qui mérite d'être publié, je mettrai sa présentation sur le blog en tant qu'article `projet` dans dans la branche `project`. A voir si je met les mêmes README.md qur sur les projets en question mais je ne pense pas.

- **Article Web Intégré**
    Des articles qui intégre des pages web, comme des projets de jeux sur daisseur.xyz, des petites pages interactives


## Ouverture et collaboration

- **Dépôt GitHub public**  
    Le blog est hébergé sur GitHub pour permettre à tous de consulter les articles, soumettre des pull requests ou ouvrir des issues.



## Extensions et idées

- **Composants GitHub intégrés**  
    Syntaxe spéciale dans les posts Markdown pour intégrer un composant GitHub d’un autre repo, par exemple :  
    `{{type: "Github", "repoUrl": "https://github.com/permissionlesstech/bitchat-android"}}`

- **Traduction intelligente**  
    Utilisation de Groq pour traduire un post dans différents styles : français courant, français pro, anglais courant, anglais pro.

- **Thème markdown alternatifs**  
    Proposer des thèmes markdown alternatifs au niveau des couleurs mais aussi d'autres façons de rendre le markdown (style obsidian, vscode). -> le problème c'est que ce ne sera pas le rendu voulu mais ça reste intéressant 


- **Jouer de la musique à la lecture de l'article**  
    Grâce à une syntaxe particulière le client pourrait écouter la musique que l'article suggère, spotify/mp3. La syntaxe est encore à définir mais peut-être:  
    `{{type: "MusicPlayer", "musicUrl": "https://share.daisseur.xyz/joyca.mp3"}}`

