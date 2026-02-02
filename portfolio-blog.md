[tags]: <> (github, profile, projects, open source, developer, portfolio, svelte, sveltekit, web development)

# Portfolio Blog
> En ligne (prod) sur [daisseur.xyz](https://daisseur.xyz/from/github) depuis le 19 octobre 2025 !!

Ce projet vise à créer un portfolio qui se présente comme un blog, avec une organisation inspirée de Git (créé par notre bon vieux Linus Torvalds) pour la gestion et la navigation des articles.

Le brouillon initial est disponible ici : [Blog Git-like](https://github.com/daisseur/blog/blob/61ff6cbfd5aa4d0b13c14a51a7abe54ef69b5f30/README.md).
Et la présentation du repo Github du blog [ici](https://github.com/daisseur/blog/README.md).


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
    Parcours des articles avec des indicateurs du type `HEAD`, `HEAD~1`, `HEAD~21`, etc. 
    `Pas encore implémenté.`

## Les articles eux-mêmes

- **Article projet**
    Si j'ai travaillé sur un projet qui mérite d'être publié, je mettrai sa présentation sur le blog en tant qu'article `projet` dans dans la branche `project`. A voir si je met les mêmes README.md qur sur les projets en question mais je ne pense pas.

- **Article Web Intégré**
    Des articles qui intègrent des pages web, comme des projets de jeux sur daisseur.xyz, des petites pages interactives


## Ouverture et collaboration

- **Dépôt GitHub public**  
    Le blog est hébergé sur GitHub pour permettre à tous de consulter les articles, soumettre des pull requests ou ouvrir des issues.



## Extensions et idées
Dorénavant la majorité des suggestions et idées seront évoqués dans un premier temps dans un Tech Talk avant d'être cité ici. Je laisse ces idées ici le temps que je me décide sur une section ou un article où les mettre.

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
	
	Finalement une bonne idée serait de faire un wrapper [strudel.cc](https://strudel.cc/#c2V0Q3BtKDEyOC80KQoka2ljazogcygiYmQgfiBiZCB%2BIikuYmFuaygiUm9sYW5kVFI5MDkiKS5nYWluKDAuOTUpCiRzbmFyZTogcygifiBzZCB%2BIHNkIikuYmFuaygiUm9sYW5kVFI5MDkiKS5nYWluKDAuOCkucm9vbSgwLjIpCiRoYXRzOiBzKCJoaCo4IikuYmFuaygiUm9sYW5kVFI5MDkiKS5nYWluKCJbLjQgLjZdKjQiKS5wYW4oc2luZS5yYW5nZSgwLjMsIDAuNykpCiRiYXNzOiBub3RlKCJjMiBjMiB%2BIGMyIikucygic2F3dG9vdGgiKS5scGYoNjAwKS5nYWluKDAuNikKJHBhZDogbm90ZSgiPFtjMyxlMyxnMyxiM10gW2EyLGMzLGUzLGczXT4iKS5zKCJzdXBlcnNhdyIpLmxwZihzaW5lLnJhbmdlKDgwMCwgMjAwMCkuc2xvdygxNikpLmF0dGFjaygwLjUpLnJlbGVhc2UoMSkucm9vbSgwLjgpLmdhaW4oMC4yKQokbGVhZDogbigiMCB%2BIDIgMyB%2BIDUgNyB%2BIikuc2NhbGUoImMzOm1ham9yIikucygidHJpYW5nbGUiKS5scGYoMjAwMCkuZ2FpbigwLjM1KS5kZWxheSgwLjMpLmRlbGF5dGltZSgzLzgpLmRlbGF5ZmVlZGJhY2soMC4zKQo%3D) et mettre des musiques qui me plaisent grâce à un convertisseur midi to strudel, avec un llm pour améliorer le résultat brut ( il y a de grande chances que je passe derrière). 

    Ça pourrait être dingue de faire un article qui en fait est juste une page qui joue en temps réel ce que je fais sur mon host sur les clients, algorave en live ! (possible avec le wrapper strudel.cc)
	
    *Mais en tout cas il y aurait un player son assez discret, peut-être en flottant en centre bas ou alors dans la top bar...*

	

