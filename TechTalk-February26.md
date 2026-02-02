[pinned]: <> (true)
[title]: <> (Tech Talk 02/26)
[tags]: <> (blog, react, astro, svelte, portfolio)

# Deuxième TechTalk mensuel du blog ! 
Des idées du turfu pour faire un portfolio de dingue !

**Table des matières**:
* [Nouveau concept de page portfolio](#nouveau-oncept-de-page-portfolio)
* [Le référencement et l'accessibilité](#Le-référencement-et-l'accessibilité)
* [Traduction automatique et i18n](#Traduction-automatique-et-i18n)

<br>

# Nouveau concept de page portfolio
  Actuellement (début février) le blog est la partie majeure de mon site principal https://daisseur.xyz. J'aimerais changer ça comme je l'avais commencé à envisager ici: [Tech Talk 01/26](/blog/main/TechTalk-January26.md#organisation-du-site). Et pour ça je voudrais faire une page principale qui alternerait entre plusieurs versions de différents styles et créés avec plusieurs frameworks web javascript et donc des librairies d'ui/d'effets différentes elles aussi ! 
  
  La composition de la page ne sera pas fondamentalement différente mais je compte intégrer un défilement semi-automatique entre les différentes pages chargés par les frameworks (je pense à vue, react, svelte et astro) et tout ça en utilisant probablement Astro, qui de ce que j'en sais, permet d'utiliser plusieurs frameworks dans un même site, j'essaierai de faire en sorte que l'on ne se rende pas compte que c'est un autre frameworks qui fait la partie de la page que l'on voit. Je sais que c'est possible en sveltekit avec des pages en svelte mais je ne sais pas du tout avec Astro, on va espérer, je tiendrais cette section ou les suivantes à jour dès que je m'en occuperai ! 
<br>
# Le référencement et l'accessibilité
  Avoir un portfolio c'est bien, un blog c'est encore mieux, mais le top du top c'est d'avoir un site bien référencé sur google et des super ogtag/metadata à afficher dans les preview discord/instagram/telegram. 
  Et avoir un bon référencement c'est aussi avoir un site web qui respecte les règles et normes d’accessibilité dictées par mozilla/google et d'autres.
  Il va donc falloir que je fasse un petit taff sur tout ça, notamment les `aria-label`, `aria-role` et autres.
  
  On m'a aussi conseillé de suivre les méthodes/conseils du site [schema.org](https://schema.org) (merci Max le goat): c'est-à-dire typer une grande majorité des éléments html présent sur mes pages et établir des relations entre eux (on peut remarquer que c'est une tâche que ferait parfaitement un llm.. ). Hop un petit exemple ici:
  ```json
{
-   "@context": "https://schema.org/",  
-   "@type": "Thing",  
-   "name": "Schema.org Ontology",  
-   "subjectOf": {  
-     "@type": "Book",  
-     "name": "The Complete History of Schema.org"  
-   }  
}
  ```
*Pour un site qui prône l'accessibilité et la facilité de lecture je me permet de critiquer leur mode blanc inchangeable qui me brûle les yeux T-T (darkreader mon héro)*
<br>

# Traduction automatique et i18n
J'avais commencé à implémenter un support multilingue pour mon blog, mais la flemme m'a un peu rattrapé c'est vrai. 
*(Aux personnes qui veulent m'embaucher: la flemme est un problème qui arrive souvent quand je ne suis pas payé... et/ou occupé à faire mon bac/bac blanc. Sinon j'essaye vraiment d'être sérieux je vous promet.)*
Donc pour petit rappel mon projet était de traduire mon site en plusieurs langues en utilisant le principe/format i18n. Mais la deuxième partie était de traduire chaque article dans d'autres langues et tons d'écriture en utilisant un llm. Ce que j'avais développé mais que j'avais désactivé parce que ça ne me paraissait pas assez perfectionné et que chaque test me faisait gâcher des précieuses requêtes gratuites de mon provider (ici GroqCloud, non pas grok de X.). Je vais essayer de le réimplémenter sur le site, pour dire bonjour et faire des blagues dans d'autres langues sans rien faire (je suis curieux de voir comment le llm va traduire cet article en anglais ou en espagnol mais sur comment il va le traduire sur le ton professionnel).
