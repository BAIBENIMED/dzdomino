# DZ Domino

Le domino à l'algérienne (double-six), jouable dans le navigateur : **https://baibenimed.github.io/dzdomino/**

## Modes

- **Contre l'IA** : 2, 3 ou 4 joueurs (2 contre 2 ou chacun pour soi), trois niveaux (facile, moyen, difficile), pioche au choix, temps par coup.
- **En ligne avec des amis, sans compte** : créez une table, envoyez le lien ou le code de 4 lettres, chacun choisit sa place (places 1 et 3 contre 2 et 4). Les places vides peuvent être prises par l'IA.
- Sons, rappel des derniers coups et « Revoir la manche ».

## Règles

- 7 dominos chacun ; à 2 ou 3 joueurs, le reste forme la pioche.
- 1ʳᵉ manche : le plus gros double ouvre ; ensuite, le gagnant de la manche précédente ouvre.
- Celui qui pose son dernier domino marque les points restant dans les mains adverses.
- Partie bloquée : le joueur le plus léger gagne la manche.
- Première équipe, ou premier joueur, à 100 points.

## Technique

Un seul fichier `index.html`. Le jeu en ligne passe par un serveur MQTT public (`broker.emqx.io`) : chaque table y est gardée 24 h. C'est un serveur public et gratuit, donc sans garantie de disponibilité, et une personne technique pourrait lire l'état des tables. Ça convient pour jouer entre amis, pas pour de l'argent.
