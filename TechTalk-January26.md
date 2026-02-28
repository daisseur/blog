[pinned]: <> (true)
[title]: <> (Tech Talk 01/26)
[tags]: <> (github, git, md, mdx, marked, remark, markdown, blog, react, jsx, integration, embed)
# Premier TechTalk mensuel du blog ! 
Quelque choix importants pour le futur de ce blog. Mais avant ça: C'est quoi un TechTalk sur le blog daisseur.xyz ?

**Table des matières**:
* [C'est quoi le TechTalk ?](#Le-Techtalk)
* [Le format fichier des articles](#Le-format-fichier-des-articles)
* [Un interpréteur de markdown](#Un-interpréteur-de-markdown)
* [Organisation du site](#Organisation-du-site)
* [Compteur de vues pour article](#Compteur-de-vues-pour-article)

<br>

# Le TechTalk <a id="Le-TechTalk"></a>
  Le TechTalk se présente sous la forme d'un petit article qui est en fait un point sur mes avancées et idées pour mes projets de dev en général mais notamment sur ce blog. Ce format me permet de partager mes idées, mais aussi de les mettre en ordres de façon un peu chronologique.
  
  >[!IMPORTANT]
  > **L'objectif est de reprendre les sections dans d'autres article de mon blog**<br>
  > Le TechTalk est un peu une manière d'organiser mes idées en les rédigeant par section: Si je veux avancer sur une idée (ex: projet/feature), je cite/fait une référence à la dernière section d'un TechTalk ou je parlais de l'idée.

Un bon exemple de l'utilité du TechTalk concerne ce blog, pour témoigner de l'évolution de celui-ci et des cheminement de pensées qui ont aboutit je peux juste faire référence à un section d'un TechTalk dans le [README.md](/blog/main/README.md) ou [portfolio-blog.md](/blog/main/portfolio-blog.md).

<br>

## Le format fichier des articles <a id="Le-format-fichier-des-articles"></a>
  Je regardais les alternatives opensource qui se faisaient sur les portfolio en react/svelte et ce que j'ai remarqué c'est que certains portfolios utilisaient le format mdx au lieu du simple markdown. Ce qui correspond exactement à ce que j'essayais de faire depuis le début du projet. C'est-à-dire avoir des tags au début des fichiers markdown, avoir des intégrations... Mais le problème c'est que si je transforme les fichiers en mdx, ils ne pourront plus être lisible nativement sur github, ce qui enlève un peu de fun au projet.
  
  >[!NOTE]
  **Mais le `mdx` c'est quoi ?** <br>
  >*Le mdx est un format qui mix le jsx/tsx avec le markdown avec un aspect 'component' pour une meilleure intégration dans les sites web type blog/porfiolio. Leur site peu être trouvé ici:*
  >https://mdxjs.com/
  
  
  >[!NOTE]
  >**Est-ce que le `mdx` est vraiment utile/plus pratique ?**<br>
  >*Une autre question qui se pose avant celle-là c'est: En écrivant un article de blog comme celui-ci, on privilégie la facilité d'écriture ou l'esthétique et l'aspect complet de l'article aux yeux du lecteurs ?*
  >- Facilité d'écriture : Une syntaxe pratique pour la mise en forme mais aussi des intégrations facile à introduire
  >- Facilité de lecture : Un aspect esthétique pour le lecture qui lui permet de mieux comprendre, mieux se representer et mieux comprendre la structure de l'article 
  >
  > Une solution à tout ça pourrait être un [Interpréteur](#un-interpréteur-de-markdown)
  >
  > Donc pour répondre à la question initiale: le format mdx est customizable et donc plus souple, ça permet une meilleure fluidité dans l'écriture de l'article.


  ### **Module de markdown**
  Changer de langage/format pour les articles m’amène à me demander si je ne devrais pas délaisser le bon vieux module [`markedjs`](https://github.com/remarkjs/remark) 
  > bon exemple d'endroit où il serait sympa de juste mettre un {Integration('https://github.com/markedjs/marked')} ou un truc du genre pour afficher une preview de la page
  
  pour une alternative plus moderne comme [`remark`](https://github.com/remarkjs/remark) et qui lui supporte avec un plugin largement reonnu le mdx.
<br>

## Un interpréteur de markdown <a id="Un-interpréteur-de-markdown"></a>
  Un bon compromis pourrait être un interpréteur qui convertirait mon texte en mdx et en markdown classique en même temps (2 versions alternative) pour satisfaire les 2 points que je viens de citer plus l'accessibilité des articles en markdown simple et efficace sur github ou autre.

  Cet interpréteur serait une interface uniquement accessible à moi (à moins que j'ouvre le blog à d'autres) et qui me permettrait d'écrire plus vite et de rajouter des éléments graphique/intégrations de façons naturelle et automatique: En reprenant mdx ou alors avec un wrapper fait maison :p.

  Actuellement j'utilise Obsidian ou tout simplement l'éditeur github.
<br>

## Organisation du site <a id="Organisation-du-site"></a>
  Ce serait vraiment bien d'avoir une partie du site un peu plus rédigé (peut-être avec des sections directement issu d'article mais pas sous forme directe de card) à part de la section blog.
  ```à développer...```
<br>

## Compteur de vues pour article <a id="Compteur-de-vues-pour-article"></a>
  Un compteur de vues permettrait de savoir combien de personnes ont vu l'article, et même possiblement trier sur certaines périodes: total, dernière semaine, aujourd'hui. Les "vues uniques" seraient établis avec l'ip de la personne qui accède a la page de l'article et un cooldown de 1h a peu près ou moins.

  Ça ne m'a pas l'air trop dur à implémenter...
