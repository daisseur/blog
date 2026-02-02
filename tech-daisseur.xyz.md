# daisseur.xyz
Comment que ça marche mes sites web ? J'essaye de tout mettre en ordre...
**Je compte mettre ici principalement des références à des sections de Tech Talk etn développant certains points.**

## Ancien fonctionnement: tunnel cloudflare
Avant que je ne comprenne vraiment ce que faisait nginx, je faisais des tunnels couldflare, c'est-à-dire le service de reverse proxy de cloudflare, via son utilitaire [`cloudflared`](https://github.com/cloudflare/cloudflared).
Ces tunnels me permettait de n'exposer aucun port de ma box, et de simple faire un tunnel d'un de mes ports en localhost vers un sous-domaine que j'avais avec cloudflare.
<br>
## Nouveau fonctionnement: Nginx
En comprenant ce que faisait nginx, et que je pouvais l'appliquer à mon serveur local j'ai remplacé tous mes tunnels cloudflare (CNAME) par des enregistrement dns (A) direct vers mon ip public au port où nginx répartit quel requete va où en fonction du nom de domaine demandé.

Puisque je tiens à ne pas me faire DDOS, j'ai activé l'option gratuit qui fait de cloudflare l'un des leader de la protection anti-DDOS aujourd'hui: le PROXY !! En bref votre requete passe d'abord chez cloudflare qui envoie la requete à mon serveur, il fait un intermédiaire.

D'ailleurs bonne nouvelle j'ai un certificat SSL sur tous mes sites actuellement, enjoy !

```en cours de rédaction...```
