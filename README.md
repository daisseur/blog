[title]: <> (Blog Repository)
[tags]: <> (blog, portfolio, github, markdown, articles, open source, projects)
[pinned]: <> (true)

# Blog Repository

Ce dépôt GitHub sert à stocker publiquement les articles de mon blog personnel, intégré à mon portfolio. Il contient des publications sur divers sujets liés à mes projets, à la programmation, à la cybersecurité et autres hobbies. 
L'un des objectif est de créer une sorte de pont entre mes différents projets, le but est que chaque projet que je fait ait son article ici.

Pour une explication plus détaillée du projet, consultez [portfolio-blog.md](https://github.com/daisseur/blog/blob/main/portfolio-blog.md).

## Contenu
- Articles en Markdown
- Mises à jour régulières (plus ou moins)


## Metadata des articles
Pour permettre une meilleure organisation et recherche, chaque article peut inclure des métadonnées en haut du fichier Markdown via des sortes de commentaires (sans le !):
```markdown
![title]: <> (Titre de l'article)
![tags]: <> (tag1, tag2, tag3)
![pinned]: <> (true/false)
```
L'avantage c'est qu'avec cette syntaxe les metadata peuvent être écrites sans êtres affichés par le parser markdown de Github notamment.
### Redirection vers fichier externe de Github
Le but est de créer une redirection au niveau du blog https://daisseur.xyz pour mettre à jour directement sans copier manuellement le nouveau contenu dans le repo. C'est très pratique pour suivi de projet/repo Github.
Dans les tags j'utilise cette balise pour signaler la redirection : 
```md
![gitRedirect]: <> (https://raw.githubusercontent.com/daisseur/blog/main/portfolio-blog.md)
```
> Il faudrait aussi faire une fonction de sanitize pour ne pas partager une xss si le repo venait à être compromis.

Seul vrai point négatif: rien ne s'affiche sur Github lors de la visualisation de l'article de redirection qui pointe un autre markdown :(


## Contributions
On pourrait croire que ce repo est exclusif à moi, ce qui était un peu vrai au tout début. Mais maintenant je me dis, que si des personnes (plus particulièrement des amis) veulent faire leur propre article en lien avec mes intérêts ce serait cool aussi !
En tout cas n'hésitez pas à me le dire si vous avez des suggestions :p

***Et allez explorer les articles de ce repo !***
