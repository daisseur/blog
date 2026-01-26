# Choix importants pour le blog...

**Tables des matières**:
  * [Le format fichier des articles](#le-format-fichier-des-articles)
  * [Un interpréteur de markdown](#un-interpréteur-de-markdown)
  * [Organisation du site](#organisation-du-site)

<br>

## Le format fichier des articles
  Actuellement je regardais les alternatives opensource qui se faisaient sur les portfolio en react/svelte et ce que j'ai remarqué c'est que certains utilisait le format mdx au lieu du simple markdown. Ce qui correspond exactement à ce que j'essayais de faire depuis le début du projet. C'est-à-dire avoir des tags au début des fichiers markdown, avoir des intégrations... Mais le problème c'est que si je transforme les fichiers en mdx, ils ne pourront plus être nativement lisible sur github, ce qui enlève un peu de fun au projet.
  
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
  ### Module de markdown
  Changer de language/format pour les articles m'ammène à me demander si je ne devrais pas délaisser le bon vieux module [`markedjs`](https://github.com/remarkjs/remark) 
  > bon exemple d'endroit où il serait sympa de juste mettre un {Integration('https://github.com/markedjs/marked')} ou un truc du genre pour afficher une preview de la page
  
  pour une alternative plus moderne comme [`remark`](https://github.com/remarkjs/remark) et qui lui supporte avec un plugin largement reonnu le mdx.

<br>

## Un interpréteur de markdown
  Un bon compromis pourrait être un interpréteur qui convertirait mon texte en mdx et en markdown classique en même temps (2 versions alternative) pour satisfaire les 2 points que je viens de citer plus l'accessibilité des articles en markdown simple et efficace sur github ou autre.

  Cet interpréteur serait une interface uniquement accessible à moi (à moins que j'ouvre le blog à d'autres) et qui me permettrait d'écrire plus vite et de rajouter des éléments graphique/intégrations de façons naturelle et automatique: En reprenant mdx ou alors avec un wrapper fait maison :p.


<br>

## Organisation du site
  Ce serait vraiment bien d'avoir une partie du site un peu plus rédigé (peut-être avec des sections directement issu d'article mais pas sous forme directe de card) à part de la section blog.
  ```rédaction en cours...```
