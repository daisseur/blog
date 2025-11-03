[title]: <> (Blog Repository)
[tags]: <> (blog, portfolio, github, markdown, articles, open source, projects)
[pinned]: <> (true)

# Blog Repository

Ce dépôt GitHub sert à stocker publiquement les articles de mon blog personnel, intégré à mon portfolio. Il contient des publications sur divers sujets liés à mes projets, à la programmation, à la cybersecurité et autres hobbies.

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

### Redirection vers fichier externe de github
L'implémentation de cette idée pourrait être très pratique pour le suivi de projet/repo github, sans avoir à modifier à chaque fois
Dans les tags je pourrais mettre une balise comme celle-ci: 
```md
![redirect]: <> (https://raw.githubusercontent.com/daisseur/blog/main/portfolio-blog.md)
```
> Il faudrait aussi faire une fonction de sanitize pour ne pas partager une xss si le repo venait à être compromis.


N'hésitez pas à explorer et à contribuer si vous avez des suggestions !
